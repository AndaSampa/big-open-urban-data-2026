# Prompts da atividade prática — Aula 4

## A cidade em muitas dimensões

> O Prompt −1 deve ser executado antes da aula. Ele retoma os arquivos das aulas anteriores, calcula as dimensões necessárias e prepara um laboratório verificável. Em sala, os prompts são curtos e progressivos: não pretendem concluir como Santana de Parnaíba é, mas demonstrar o que se torna possível quando objetos recebem uma, duas, três ou muitas coordenadas.

> **Regra de continuidade:** trabalhe no mesmo Work e reutilize os projetos e dados já produzidos. Preserve originais, projetos-base e resultados das aulas anteriores. Não refaça aquisições concluídas e não substitua silenciosamente uma fonte ou variável.

---

# ANTES DA AULA

## PROMPT −1 — Preparar o laboratório multidimensional

```text
Vamos preparar o laboratório da Aula 4 usando os projetos e arquivos de Santana de Parnaíba produzidos nas aulas anteriores.

Localize e reutilize o limite municipal, as geometrias de edifícios do Google Open Buildings V3, os rasters de presença e altura do Open Buildings Temporal 2.5D e os dados censitários já disponíveis. Não refaça aquisições que estejam completas e verificáveis. Crie `atividade-aula-04/` sem alterar os projetos-base ou os produtos anteriores.

Prepare duas unidades de análise relacionadas, mas conceitualmente distintas:

1. EDIFÍCIOS
Crie uma camada de trabalho em SIRGAS 2000 / UTM 23S, EPSG:31983, contendo, quando calculável:
- identificador persistente;
- área de implantação em m²;
- perímetro em metros;
- compacidade, calculada como 4πA/P² e limitada ao intervalo de 0 a 1;
- orientação do eixo principal;
- confiança do footprint, quando disponível;
- presença média do Open Buildings Temporal dentro do polígono;
- altura mediana;
- percentil 90 ou outra síntese superior robusta da altura;
- quantidade e proporção de pixels válidos usados na associação;
- número aproximado de pavimentos, com a altura por pavimento explicitada;
- volume construído aproximado, calculado como área de implantação × altura mediana.

Não trate altura, pavimentos ou volume como informação cadastral exata. Diferencie atributos da fonte, inferências do produto e cálculos realizados agora. Preserve valores ausentes e crie indicadores de qualidade em vez de descartá-los silenciosamente.

2. UNIDADES ESPACIAIS DE CONTEXTO
Reutilize as menores feições censitárias intramunicipais verificáveis já disponíveis. Se população e renda não estiverem ambas disponíveis, procure fontes oficiais compatíveis e documentadas. Se renda não puder ser obtida ou relacionada com segurança, registre a ausência e mantenha população; não invente aproximações.

Para cada unidade espacial, prepare:
- área territorial;
- população total e densidade populacional;
- renda total, média ou per capita, apenas quando o significado e o denominador estiverem documentados;
- número de edifícios;
- soma da área de implantação;
- proporção da unidade coberta por edifícios;
- altura mediana dos edifícios;
- diversidade ou dispersão das alturas;
- compacidade média;
- volume construído aproximado total e por área territorial.

Se for criada uma redistribuição espacial de população ou renda usando edifícios, células ou outro suporte, trate-a como estimativa modelada. Preserve os totais das unidades de origem, explique o peso adotado — área, volume ou outro — e não atribua a média do setor a cada edifício ou morador. Produza também uma versão sem redistribuição para comparação.

Crie uma tabela analítica de edifícios e outra de unidades espaciais. Use nomes curtos e legíveis para os campos e produza um dicionário com: nome, significado, unidade, origem, fórmula, limitações e quantidade de valores ausentes.

Antes de concluir, examine distribuições e valores extremos apenas para validar os dados. Não execute PCA, agrupamentos, taxonomias ou interpretações substantivas e não produza mapas temáticos finais.

Organize:
- `atividade-aula-04/dados/processados/santana-de-parnaiba-aula-04.gpkg`;
- `atividade-aula-04/qgis/santana-de-parnaiba-aula-04-base.qgz`;
- `atividade-aula-04/tabelas/edificios-dimensoes.csv`;
- `atividade-aula-04/tabelas/unidades-espaciais-dimensoes.csv`;
- `atividade-aula-04/registro/dicionario-de-dimensoes.csv`;
- `atividade-aula-04/registro/manifesto-camadas.csv`;
- `atividade-aula-04/registro/diario-metodologico.md`;
- scripts reproduzíveis e checksums.

No projeto QGIS, deixe as camadas organizadas e disponíveis, mas use estilos neutros. Salve caminhos relativos. Valide geometrias, SRCs, unidades, contagens, chaves, valores ausentes e coerência das estatísticas zonais.

Ao concluir, informe o caminho do projeto, resuma as duas unidades de análise e apresente uma tabela curta com cada dimensão preparada, unidade, origem e cobertura válida. Aponte explicitamente o que não foi possível produzir. Depois aguarde.
```

### Critérios de aprovação

- O projeto-base da Aula 4 abre sem alterar os projetos anteriores.
- Edifícios e unidades espaciais permanecem como unidades de análise distintas.
- Altura e presença possuem estatísticas por edifício e indicadores de cobertura válida.
- População e renda conservam fonte, significado, denominador e suporte espacial.
- Qualquer ponderação ou redistribuição espacial é identificada como estimativa modelada.
- O dicionário distingue fonte, inferência e cálculo.
- PCA, agrupamentos e conclusões não foram antecipados.

---

# EM SALA

## PROMPT 1 — Uma dimensão: produzir uma distribuição

```text
Abra o laboratório da Aula 4 e preserve o projeto-base.

Antes de representar as alturas, separe e quantifique os edifícios com altura válida e qualidade `ok`, altura válida com cobertura baixa, sem pixel geométrico e sem altura após o limiar. Mostre a área mediana de cada grupo e verifique se a ausência se concentra nos footprints menores. Não preencha alturas ausentes.

Depois produza:

1. Um histograma da presença média para todos os edifícios que possuem esse valor. Use eixo X de 0 a 1, marcas a cada 0,1 e intervalos de 0,05. Identifique os extremos como “menor resposta do modelo” e “maior resposta do modelo” e deixe explícito que o escore não é a probabilidade de o edifício existir.

2. Um histograma da altura mediana usando todos os edifícios com altura válida e intervalos de 2 m.

3. O mesmo histograma usando somente os edifícios classificados como `ok`, com os mesmos intervalos e escalas para comparação.

4. Uma comparação lado a lado do histograma de todas as alturas válidas em duas representações: à esquerda, eixo Y linear; à direita, eixo Y logarítmico. Preserve os mesmos dados, intervalos e eixo X. Destaque quantos edifícios possuem pelo menos 20, 30, 40, 50 e 60 m. Indique com clareza que somente o eixo Y mudou.

Mostre em cada gráfico a quantidade de edifícios utilizada. Preserve toda a faixa de alturas e não remova os valores extremos. Salve também os gráficos separadamente e uma cópia do projeto.

Explique brevemente: o que presença e altura medem; quem não conseguiu receber uma coordenada de altura; o que a escala linear tornou quase invisível; e o que apareceu quando mudamos apenas a representação do eixo Y. Não interprete os histogramas como explicação da cidade.

Depois aguarde.
```

### Perguntas para reabertura

- O que a ordem das alturas permite enxergar?
- Presença mede o edifício ou a confiança/intensidade de uma inferência?
- Quem ficou sem coordenada no eixo da altura?
- Por que os edifícios altos existem nos dados, mas desaparecem na escala linear?
- Na escala logarítmica, quais distâncias iguais passaram a representar multiplicações iguais?
- Um limiar separaria grupos reais ou apenas criaria uma decisão operacional?

---

## PROMPT 2 — Duas dimensões: desenhar uma relação

```text
Com os mesmos edifícios válidos, crie um gráfico de dispersão relacionando área de implantação e altura mediana.

Mostre primeiro os valores nas escalas originais. Examine concentração, assimetria e valores extremos. Se a maior parte dos edifícios ficar comprimida perto da origem, produza também uma segunda vista com transformação logarítmica adequada, sem substituir ou esconder a primeira.

Use transparência ou amostragem somente se necessário para tornar a distribuição legível e registre a decisão. Não selecione, rotule ou nomeie edifícios como exemplos neste momento: queremos primeiro compreender a forma geral da distribuição. A ligação entre pontos do gráfico e edifícios no mapa será feita em uma etapa posterior.

Não calcule correlação como conclusão automática e não atribua causalidade. O objetivo é mostrar que dois atributos criam um espaço no qual distância, direção, vizinhança e agrupamentos visuais passam a existir.

Salve as duas vistas, quando houver, e a cópia do projeto. Depois aguarde.
```

### Alternativa negociável

Se área × altura não produzir uma distribuição didaticamente útil, testar **altura × compacidade** ou **área × presença**, preservando o primeiro ensaio e explicando por que a troca dos eixos mudou o desenho do problema.

---

## PROMPT 3 — Três dimensões: girar também pode enganar

```text
Usando os mesmos edifícios com altura válida, crie uma visualização 3D interativa com:
- X: área de implantação;
- Y: altura mediana;
- Z: compacidade.

Use transparência e permita girar, aproximar e consultar os valores de cada ponto. Se área ou altura comprimirem a distribuição, permita alternar seus eixos entre escala linear e logarítmica, indicando claramente o que mudou.

Ao lado, produza as três projeções bidimensionais do mesmo espaço: área × altura, área × compacidade e altura × compacidade.

Escolha duas posições de câmera para o mesmo gráfico 3D: uma em que alguma separação pareça evidente e outra em que ela desapareça ou fique ambígua. Preserve exatamente os mesmos dados, escalas e cores.

Não crie grupos, rótulos ou classes e não destaque edifícios individuais. Salve a visualização interativa em HTML e exporte imagens das duas câmeras e das três projeções.

Explique brevemente: o que a rotação permitiu enxergar, o que ficou oculto pela sobreposição e como o ponto de vista pode sugerir uma estrutura que os dados não demonstram. Depois aguarde.
```

### Perguntas para reabertura

- A estrutura estava nos dados ou na posição da câmera?
- Que relações só apareceram quando giramos o espaço?
- O que permaneceu oculto pela sobreposição dos pontos?
- Por que uma projeção 2D pode contradizer a impressão do gráfico 3D?

---

## PROMPT 4 — Muitas dimensões: reduzir e agrupar

```text
Crie uma cópia da tabela e use inicialmente os edifícios com altura válida e qualidade `ok`.

Faça uma primeira PCA com todas as dimensões numéricas analíticas disponíveis, excluindo apenas identificadores, códigos e coordenadas. Antes de interpretar, mostre correlações e pesos dos componentes e identifique dimensões redundantes, derivadas ou relacionadas à qualidade do dado. Explique quais aspectos receberam peso repetido.

Depois construa uma seleção consciente com uma dimensão para cada aspecto que queremos representar:
- tamanho: log da área;
- verticalidade: log da altura;
- forma: compacidade;
- orientação: codificação adequada para ângulos axiais;
- contexto: densidade edificada da unidade espacial.

Padronize essas dimensões, execute uma nova PCA e mostre a variância explicada, os pesos e a projeção nos dois primeiros componentes.

Use os componentes necessários para preservar aproximadamente 80% da variação e teste agrupamentos não supervisionados entre 3 e 6 grupos. Explique o critério usado para escolher uma solução, sem tratá-la como a divisão verdadeira da cidade.

Para cada grupo, mostre quantidade, perfil das dimensões e distribuição no mapa. Somente depois crie um nome provisório e descritivo para cada grupo, deixando explícito que a taxonomia foi construída por nós, não descoberta pelo algoritmo.

Salve as duas PCA, os gráficos, a tabela com grupos e uma nova versão do projeto. Depois aguarde.
```

### Cuidado central

O algoritmo produz partições. A taxonomia é uma interpretação humana. Os nomes devem descrever perfis mensuráveis e permanecer provisórios.

---

## PROMPT 5 — Voltar ao mundo: vizinhos de quê?

```text
No mapa, deixe que eu escolha um edifício. Não selecione o exemplo automaticamente.

Usando as dimensões conscientes e padronizadas do Prompt 4, encontre:
- os cinco edifícios geograficamente mais próximos;
- os cinco edifícios mais próximos pela distância euclidiana no espaço de atributos.

Mostre os dois conjuntos no mapa com cores diferentes e apresente uma tabela com área, altura, compacidade, orientação, contexto e posição nos agrupamentos. Não compare numericamente metros com distância padronizada; compare apenas as ordens de vizinhança.

Depois retire uma dimensão escolhida por nós, recalcule as distâncias e mostre quais vizinhos permaneceram, desapareceram ou surgiram.

Se houver tempo, agregue a proporção dos grupos morfológicos por setor e compare-a visualmente com densidade populacional e rendimento. Trate população e renda somente como contexto setorial, sem atribuí-las aos edifícios nem sugerir causalidade.

Encerre separando:
- o que veio das fontes;
- o que foi inferido pelos produtos;
- o que foi calculado;
- o que foi escolhido por nós;
- o que continua ausente.

Termine respondendo: o modelo encontrou uma estrutura da cidade ou encontrou as consequências das dimensões que escolhemos?
```

---

# Fechamento crítico da prática

A sequência não procura produzir uma análise urbana completa. Ela demonstra uma passagem:

> **distribuir → relacionar → acrescentar dimensões → reduzir → agrupar → devolver ao mapa → desconfiar**

Ao final, perguntar coletivamente:

- O que ganhou existência quando criamos cada eixo?
- Que relações só apareceram depois da normalização?
- O que a PCA preservou e apagou?
- Quem escolheu a quantidade de grupos?
- Quem nomeou os tipos?
- Quais pessoas, experiências e relações urbanas continuam do lado de fora da tabela?
