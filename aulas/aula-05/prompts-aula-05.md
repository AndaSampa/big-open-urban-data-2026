# Prompts da atividade prática — Aula 5

## Ler Santana de Parnaíba com o QGIS

> O Prompt −1 prepara o GeoPortal antes da aula. Os demais prompts registram experiências já executadas, cujos resultados serão apresentados e discutidos em sala. A aula não depende de reexecutá-los ao vivo.

> **Regra de continuidade:** trabalhe no mesmo Work e reutilize os projetos e dados já produzidos. Preserve originais, projetos-base e resultados das aulas anteriores. Não refaça aquisições concluídas e não substitua silenciosamente fontes, variáveis ou métodos.

---

# ANTES DA AULA

## PROMPT −1 — Construir o GeoPortal de Santana de Parnaíba

```text
Retome todos os produtos válidos das atividades anteriores sobre Santana de Parnaíba e prepare a base da Aula 5 sem modificar nem sobrescrever os projetos já existentes.

Crie uma nova pasta `atividade-aula-05` e um novo projeto QGIS que funcione como um pequeno GeoPortal local do município: visualmente organizado, navegável durante uma aula e capaz de reunir as diferentes formas de representação trabalhadas no curso.

Carregue tudo o que estiver disponível e metodologicamente documentado: limite municipal, setores censitários, população, densidade, rendimento, sistema viário, hidrografia, equipamentos e pontos de interesse, DEM ou MDT, relevo sombreado, declividade, edifícios, presença e altura estimada, métricas morfológicas, resultados de PCA, agrupamentos, vizinhanças geográficas e por atributos e demais produtos das aulas anteriores.

Organize as camadas em grupos temáticos claros, aproximadamente nesta ordem:

- LEIA-ME, fontes e limitações;
- limites e referências;
- pontos e equipamentos;
- linhas, conexões e barreiras;
- polígonos, setores e ocupação;
- terreno e rasters;
- edifícios e morfologia;
- visualização 3D;
- dimensões, PCA, grupos e vizinhanças.

Use nomes legíveis em português, ordenação cartográfica coerente, estilos visualmente consistentes, transparências, aliases de campos, dicas de mapa e visibilidade dependente da escala. As camadas devem poder ser ligadas e desligadas sem destruir a leitura do projeto.

Crie temas de mapa que permitam alternar rapidamente entre algumas leituras urbanísticas:

1. estrutura geral do município;
2. relevo, rios e barreiras;
3. população e rendimento;
4. ocupação e cobertura edificada;
5. alturas e verticalização;
6. morfologia dos edifícios;
7. PCA e agrupamentos;
8. vizinhança geográfica versus vizinhança por atributos.

Configure também uma vista 3D simples e funcional, usando o terreno e extrudando somente os edifícios com altura válida. Alturas ausentes devem permanecer ausentes, nunca transformadas em zero. Evite exageros verticais que distorçam completamente a paisagem.

O projeto deve parecer um sistema preparado para exploração, e não uma coleção de arquivos. Preserve, porém, a distinção entre dado de origem, dado inferido, variável calculada e escolha metodológica.

Priorize o desempenho: caminhos relativos, índices espaciais, pirâmides para rasters, visibilidade por escala e estilos leves. Não duplique arquivos grandes sem necessidade.

Inclua uma camada ou tabela inicial chamada `LEIA-ME`, explicando brevemente:

- o que existe no projeto;
- de onde vieram os dados;
- o que foi calculado;
- quais informações são estimativas;
- quais perguntas urbanísticas o projeto permite formular;
- o que não pode ser concluído com esses dados.

Abra o projeto numa extensão municipal legível e deixe visível uma composição inicial bonita e sóbria. Valide ao final todos os caminhos, camadas, grupos, temas e a vista 3D. Entregue o projeto QGIS, o GeoPackage consolidado quando fizer sentido, um manifesto das camadas e um breve registro das decisões tomadas.

Ao concluir, informe o caminho do projeto, apresente a estrutura dos grupos e temas de mapa, registre eventuais dados ausentes ou camadas problemáticas e depois aguarde.
```

### Critérios de aprovação

- O projeto abre sem caminhos quebrados e sem alterar produtos anteriores.
- As camadas estão organizadas por tema e podem ser ligadas e desligadas.
- Os temas de mapa oferecem leituras urbanísticas distintas.
- A vista 3D funciona e não converte alturas ausentes em zero.
- Fonte, inferência, cálculo e decisão metodológica permanecem distinguíveis.
- O projeto é suficientemente leve para navegação ao vivo.

---

# EXPERIÊNCIAS DA AULA

## PROMPT 1 — Fazer a água aparecer no relevo

```text
Usando o DEM de Santana de Parnaíba já carregado no projeto da Aula 5, produza uma demonstração hidrológica curta e visual.

Corrija apenas as depressões necessárias para garantir o escoamento e calcule direção e acumulação de fluxo. Mostre a acumulação também em escala logarítmica para revelar simultaneamente os pequenos e os grandes valores.

A partir dela:

- extraia uma rede de drenagem experimental;
- gere microbacias;
- calcule a distância de fluxo até a drenagem;
- se possível, calcule também a altura relativa acima da drenagem;
- cruze os corredores de maior acumulação com os edifícios.

Produza estilos bonitos e contrastantes e acrescente os resultados ao grupo `Hidrologia experimental` do projeto.

Teste mais de um limiar de contribuição e explique como ele altera a densidade da rede extraída. Não apresente os edifícios selecionados como imóveis sujeitos a inundação. Trate-os somente como edifícios próximos a caminhos topográficos preferenciais de escoamento, pois o DEM não representa adequadamente a microdrenagem urbana.

Encerre explicando, em linguagem simples, a transformação:

terreno → direção → acumulação → curso d’água → microbacia → possível exposição.

Depois aguarde.
```

### Perguntas para reabertura

- Como uma rede de drenagem emerge apenas das relações entre as alturas dos pixels?
- O que muda quando alteramos o limiar de contribuição?
- Distância geométrica e distância percorrida pela água são a mesma coisa?
- Que informações seriam necessárias para transformar essa triagem em estudo de inundação?

---

## PROMPT 2 — A cidade como rede de transporte público

```text
Acrescente ao projeto da Aula 5 as linhas e paradas de transporte público que atendem Santana de Parnaíba.

Procure primeiro uma fonte oficial e atual em formato GTFS. Caso não exista uma fonte pública utilizável, consulte no OpenStreetMap as relações de transporte `type=route`, incluindo linhas de ônibus que atravessem o município mesmo quando tenham origem ou destino fora dele.

Preserve, quando disponíveis, número ou referência da linha, nome, operador, modalidade, origem, destino e paradas. Não transforme automaticamente toda via percorrida em uma linha operacional e registre eventuais relações incompletas ou descontínuas.

Organize os resultados no grupo `Transporte público`, com:

- itinerários;
- paradas;
- terminais;
- operadores ou modalidades;
- uma área simples de proximidade às paradas, apresentada apenas como aproximação de cobertura espacial.

Crie um tema de mapa chamado `Mobilidade e acessibilidade` e compare visualmente a rede com população, rendimento, relevo e ocupação urbana.

Deixe claramente separado o que veio de fonte oficial, o que veio do OpenStreetMap e o que foi calculado. Registre a data da consulta e não apresente a rede como completa sem verificar cobertura, continuidade e atualidade.

Depois aguarde.
```

### Perguntas para reabertura

- A rede acompanha onde as pessoas vivem?
- O relevo ajuda a explicar alguns percursos e ausências?
- Proximidade de uma parada é suficiente para falar em acessibilidade?
- O mapa representa infraestrutura, itinerários ou a experiência real de viajar?

---

## PROMPT 3 — Revisitar a classificação dos edifícios

```text
Abra o projeto mais recente da Aula 5 e preserve todas as versões anteriores.

Retome exatamente a amostra, as dimensões padronizadas, a PCA e o agrupamento de edifícios produzidos na Aula 4. O problema a investigar é conhecido: edifícios que reconhecemos como verticalizados ficaram espalhados entre vários grupos.

Primeiro reproduza o resultado original e mostre onde estão os edifícios com altura válida de pelo menos 20 m. Esse limiar é uma definição operacional escolhida para o experimento, não uma verdade tipológica. Informe também os resultados para 15 m e 30 m, apenas para mostrar a sensibilidade dessa escolha.

Compare três formulações, mantendo a mesma amostra sempre que possível:

1. classificação original;
2. classificação com maior peso para a altura padronizada, testando pesos 2 e 3;
3. taxonomia em duas etapas: separar explicitamente os edifícios com altura de pelo menos 20 m e agrupar somente os demais com as dimensões morfológicas já utilizadas.

Não escolha a solução apenas porque o mapa parece mais convincente. Para cada formulação, apresente:

- quantidade de edifícios por grupo;
- distribuição de altura, área e compacidade;
- proporção dos edifícios com pelo menos 20 m em cada grupo;
- mudanças de grupo em relação à classificação original;
- efeito sobre separação interna, valores extremos e distribuição espacial.

Mostre lado a lado os três mapas e crie uma tabela simples acompanhando alguns edifícios verticalizados nas diferentes formulações.

Explique claramente a diferença entre:

- deixar o agrupamento procurar variações sem dizer quais importam;
- ponderar uma dimensão porque consideramos essa diferença relevante;
- escrever uma regra que cria previamente uma categoria.

Acrescente os resultados ao projeto no grupo `Classificação revisitada` e crie temas de mapa para alternar entre `Original`, `Altura ponderada` e `Verticalidade explícita`.

Não substitua a classificação anterior nem declare que uma das novas soluções revelou os tipos verdadeiros da cidade. Encerre respondendo: o que mudou nos dados, o que mudou apenas na formulação e qual ideia de morfologia urbana cada solução passou a privilegiar?

Depois aguarde.
```

### Perguntas para reabertura

- O algoritmo deixou de errar ou nós mudamos a pergunta?
- A verticalidade deve dominar todas as outras diferenças morfológicas?
- Um limiar de 20 m encontra um tipo ou produz uma categoria?
- Qual solução ajuda mais a pergunta urbanística que queremos fazer?

---

## PROMPT 3B — Qual é a assinatura morfológica dos grupos?

```text
Retome os resultados do Prompt 3 sem modificar os projetos e tabelas anteriores.

Crie um notebook Jupyter em Python muito curto, visual e didático para responder à pergunta:

QUAL É A ASSINATURA MORFOLÓGICA DE CADA GRUPO DE EDIFÍCIOS?

No mapa, os grupos aparecem misturados e não formam regiões contínuas. Em vez de procurar um desenho espacial inexistente, mostre de maneira simples como os atributos usados na classificação se distribuem dentro de cada grupo.

Use somente três atributos:

- altura mediana do edifício, em metros;
- área de implantação, em metros quadrados;
- compacidade, entre 0 e 1.

Use a mesma amostra e a mesma classificação examinadas no Prompt 3. Preserve valores ausentes e informe apenas quantos edifícios existem em cada grupo.

Estruture o notebook como uma história de cinco passos:

1. Mostre a pergunta e explique em duas frases que um grupo pode reunir edifícios semelhantes mesmo quando eles estão distantes no mapa.

2. Mostre uma tabela pequena com a quantidade de edifícios por grupo.

3. Produza três gráficos de violino com um boxplot simples no interior: um para altura, um para área e um para compacidade. Use sempre as mesmas cores para os grupos.

Antes dos três gráficos, inclua uma única figura explicativa indicando apenas:

- a parte larga mostra onde se concentram mais edifícios;
- a linha central mostra a mediana;
- a caixa mostra a metade central dos valores;
- pontos muito afastados indicam valores extremos.

Não ensine densidade de probabilidade, quartis ou estatística formalmente. Use linguagem cotidiana.

Se área ou altura ficarem comprimidas por valores muito grandes, mostre primeiro o gráfico original e depois uma cópia com escala logarítmica, explicando somente que a nova escala abre espaço visual para os valores menores. Não remova extremos.

4. Abaixo dos gráficos, produza uma tabela muito curta contendo apenas a mediana de altura, área e compacidade de cada grupo, nas unidades originais.

5. Escreva uma frase simples para cada grupo, baseada somente nesses três atributos. Exemplo: “este grupo reúne principalmente edifícios baixos, pequenos e relativamente compactos”. Não invente uso, renda, período de construção ou tipo arquitetônico.

Encerre respondendo somente:

- qual atributo mais separou os grupos;
- quais grupos continuam muito parecidos;
- por que grupos morfológicos podem ficar espalhados no mapa.

Entregue o notebook `.ipynb` já executado, uma versão HTML e uma imagem PNG com os três gráficos. Use títulos e explicações em português. Deixe o código visível, curto e organizado, mas não transforme o material numa aula de programação. Depois aguarde.
```

### Sequência narrativa sugerida

> **No mapa eles se misturam. Nos gráficos conseguimos enxergar o que fez cada grupo ficar diferente.**

### Perguntas para reabertura

- Onde cada grupo concentra a maior parte de seus edifícios?
- Qual atributo separa melhor os grupos?
- Dois grupos diferentes ainda podem possuir muitos edifícios parecidos?
- Por que edifícios parecidos podem estar distantes na cidade?

---

## PROMPT 4 — Levar Santana de Parnaíba ao Blender

```text
Use o projeto mais recente da Aula 5 para preparar uma demonstração visual de Santana de Parnaíba no Blender. Preserve os projetos QGIS e produtos anteriores.

O objetivo é simples: escolher um trecho interessante do município e transformar terreno e edifícios numa cena 3D bonita, iluminada e fácil de compreender.

Escolha um recorte territorial manejável que possua relevo perceptível e edifícios com diferentes alturas. Mostre num pequeno mapa onde esse recorte fica dentro de Santana de Parnaíba. Não tente colocar o município inteiro na cena se isso deixar o arquivo pesado ou a imagem confusa.

Leve para o Blender somente:

- o terreno produzido a partir do DEM ou MDT;
- os edifícios com altura válida;
- a hidrografia e algumas vias principais, somente se ajudarem a reconhecer o lugar.

Resolva internamente projeção, origem das coordenadas, escala e desempenho, documentando essas decisões sem transformá-las no centro da demonstração.

Construa a cena com:

- uma malha de terreno;
- edifícios extrudados com suas alturas estimadas;
- materiais simples para distinguir terreno, edifícios e água;
- luz solar, sombras e iluminação ambiente;
- uma câmera oblíqua que mostre simultaneamente relevo e verticalização.

Configure também o sol pela posição geográfica real do recorte. Use a extensão oficial `Sun Position`, se estiver disponível na versão instalada do Blender, informando latitude, longitude, orientação do norte, fuso horário, data e hora locais. Se a extensão não puder ser instalada, reproduza o mesmo cálculo por script e documente o método.

Escolha uma data didaticamente clara e prepare três estados da mesma câmera, por exemplo 9h, 12h e 16h, para mostrar a mudança das sombras sem alterar terreno, edifícios ou materiais. Crie também uma animação curta do percurso solar ao longo desse dia, com a data, o horário e o norte visíveis de maneira discreta.

Não invente altura para edifícios sem esse dado. Mantenha inicialmente a mesma escala nos eixos horizontal e vertical. Se uma segunda imagem usar exagero vertical, indique claramente o fator utilizado.

Procure uma linguagem visual próxima de uma maquete urbana contemporânea: bonita, sóbria e com sombras capazes de revelar a forma do terreno e dos edifícios. Evite excesso de textura, vegetação ou efeitos cinematográficos que escondam os dados.

Entregue:

- o arquivo `.blend` pronto para abrir;
- uma imagem renderizada em alta resolução;
- uma segunda vista do mesmo lugar;
- uma comparação do sol em três horários;
- um vídeo curto do percurso solar ao longo do dia;
- o pequeno mapa de localização;
- os arquivos ou scripts necessários para reproduzir a cena;
- uma explicação curta do que veio do QGIS e do que foi criado no Blender.

Encerre respondendo em linguagem simples: o que conseguimos analisar melhor no QGIS e o que conseguimos comunicar melhor no Blender? Depois aguarde.
```

### Critérios de aprovação

- O recorte mostra relevo e diversidade de alturas.
- Terreno e edifícios mantêm escala coerente.
- Alturas ausentes não recebem valores inventados.
- A iluminação ajuda a ler a forma urbana.
- A posição do sol corresponde à localização, data, hora, fuso e orientação do norte registrados.
- O arquivo Blender abre com câmera e luz configuradas.
- A preparação permanece reproduzível.

---

# Fechamento possível

O projeto não pretende concluir Santana de Parnaíba. Ele permite formular perguntas, combinar representações e observar como cada operação torna algumas relações visíveis enquanto mantém outras fora do mapa.

> **O QGIS não é apenas onde exibimos os dados: é onde ensaiamos maneiras de perguntar à cidade.**
