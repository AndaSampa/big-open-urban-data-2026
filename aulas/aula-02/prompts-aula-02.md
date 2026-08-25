# Roteiro de prompts — Aula 2

## Da tabela ao mapa em Santana de Parnaíba

Este roteiro é a trilha operacional paralela à apresentação. As lâminas sustentam a narrativa intelectual; o Work prepara arquivos, executa transformações verificáveis e registra decisões. Não é necessário sincronizar cada prompt com uma lâmina.

Os prompts da Aula 2 são deliberadamente mais curtos que os da Aula 1. Eles aproveitam a memória do mesmo Work e mostram que uma colaboração competente também pode acontecer por pedidos humanos, incrementais e corrigíveis.

## Arquitetura da prática

> **Kit garantido → QGIS básico → Censo como base agregadora → cardápio negociado → produto escolhido → reabertura no QGIS → crítica → ajuste → rodada extra, se houver tempo.**

### Percurso essencial

1. Preparar antes da aula o GeoPackage e o projeto QGIS.
2. Abrir o kit e apresentar o básico do QGIS.
3. Tematizar uma variável censitária ao vivo.
4. Negociar com a turma um produto do cardápio.
5. Pedir ao Work que produza o artefato escolhido.
6. Reabrir o resultado no QGIS, inspecionar e corrigir.
7. Registrar um achado, uma limitação e uma nova pergunta.

### Percurso elástico

Se houver tempo, voltar ao cardápio e executar um ou mais módulos adicionais. Cada rodada extra deve produzir algo que permaneça no mesmo GeoPackage e no mesmo projeto QGIS.

---

# ANTES DA AULA

## PROMPT −1 — Preparar o kit cartográfico garantido

Executar no mesmo Work da Aula 1, antes da aula.

```text
Vamos preparar o kit cartográfico da Aula 2 usando a investigação de Santana de Parnaíba que já está neste Work.

Localize o registro persistido do município e os arquivos produzidos na Aula 1. Não me peça novamente nome, UF ou código IBGE e não refaça aquisições que já estejam completas.

Crie `atividade-aula-02/` sem alterar os arquivos da Aula 1. Prepare um GeoPackage e um projeto QGIS que eu possa abrir no início da aula.

Antes de concluir, procure os arquivos em toda a estrutura da Aula 1, inclusive originais, derivados, pacotes compactados, manifestos e exportações. O kit mínimo deve conter obrigatoriamente:
- limite oficial do município;
- feições censitárias intramunicipais e atributos documentados que permitam ao menos uma tematização demográfica ou socioeconômica;
- POIs do Overture;
- ao menos uma camada de pontos verificável;
- tabelas de auditoria para registros que não puderam ser espacializados corretamente.

Inclua também, quando tecnicamente verificáveis:
- escolas como pontos a partir de uma fonte que realmente forneça coordenadas ou geometrias, sem geocodificação silenciosa;
- equipamentos e vias do OpenStreetMap com geometria, fazendo uma nova consulta somente se a consulta anterior tiver preservado apenas identificadores e tags.

Se as feições censitárias intramunicipais não forem encontradas no Work, não declare o kit concluído: informe exatamente o que procurou e proponha a aquisição oficial necessária. Ausência de coordenadas escolares ou de geometria OSM deve ser registrada, mas não impede a conclusão quando Censo, limite e POIs estiverem espacializados.

Use SIRGAS 2000 geográfico, EPSG:4674, para preservar ou intercambiar dados quando adequado. Crie também camadas de trabalho em SIRGAS 2000 / UTM 23S, EPSG:31983, para operações locais em metros. Não altere apenas a etiqueta do SRC: reprojete quando necessário e preserve os originais.

Produza:
- `atividade-aula-02/dados/processados/santana-de-parnaiba-aula-02.gpkg`;
- `atividade-aula-02/qgis/santana-de-parnaiba-aula-02.qgz`;
- `atividade-aula-02/registro/manifesto-camadas.csv`;
- `atividade-aula-02/registro/diario-cartografico.md`;
- scripts reproduzíveis e checksums.

Crie também `atividade-aula-02/entrega/kit-cartografico-aula-02-santana-de-parnaiba.zip`, reunindo o QGZ, o GeoPackage, o manifesto, o diário e as instruções mínimas de abertura. O pacote não deve duplicar originais pesados desnecessariamente.

No QGZ, organize as camadas em grupos com nomes legíveis, use caminhos relativos e aplique apenas estilos neutros. Não produza ainda um argumento cartográfico pronto: quero demonstrar a tematização ao vivo.

Ao concluir, valide que o QGZ abre, que as camadas existem, que as tabelas têm registros e que os SRCs estão declarados. Mostre uma tabela curta com camada, geometria, quantidade, fonte, período e SRC.

Na resposta final, não mostre apenas caminhos internos. Entregue links clicáveis para baixar:
1. o pacote ZIP completo;
2. o projeto QGZ;
3. o GeoPackage;
4. o manifesto de camadas.

Se a interface não permitir disponibilizar algum arquivo diretamente, diga isso explicitamente e exporte ao menos o ZIP como arquivo para download. Depois aguarde.
```

### Critérios de aprovação do kit

- O QGZ abre sem procurar arquivos manualmente.
- A resposta oferece um link clicável para baixar o pacote completo.
- O GeoPackage contém as camadas prometidas.
- O Censo possui geometria intramunicipal e chave verificável para os atributos.
- As camadas originais e reprojetadas são distinguíveis.
- Nenhum registro problemático desapareceu silenciosamente.
- Os estilos são neutros e não antecipam a conclusão da aula.
- O Work não escolheu sozinho variáveis, classes ou mensagens finais.

### Plano de contingência

Se o Work não conseguir gerar um QGZ funcional, pedir um `.qgs` equivalente e compactá-lo no QGIS depois da inspeção. O GeoPackage continua sendo o produto indispensável.

---

# ABERTURA AO VIVO — SEM PROMPT

Abrir primeiro o QGZ já validado. Antes de pedir qualquer nova operação ao Work, mostrar:

- painel de camadas e grupos;
- ligar e desligar camadas;
- selecionar uma feição e encontrar sua linha;
- selecionar uma linha e encontrar sua geometria;
- consultar atributos;
- propriedades e SRC da camada;
- diferença entre o SRC da camada e o SRC do projeto;
- simbologia simples e graduada;
- salvar o projeto.

## Demonstração censitária garantida

Escolher uma variável censitária segura e produzir uma tematização no QGIS. A demonstração deve explicitar:

1. o que cada polígono representa;
2. o significado da variável;
3. se usamos total, proporção, taxa ou densidade;
4. método e quantidade de classes;
5. paleta sequencial, divergente ou qualitativa;
6. principal limitação da leitura.

O Censo funciona como **contexto socioespacial agregador**, não como descrição individual de cada morador. A associação de um ponto a um setor não transfere automaticamente as características médias do setor para aquele estabelecimento ou pessoa.

---

# ENTRADA DO WORK AO VIVO

## PROMPT 0 — Conferir o kit que acabamos de abrir

```text
Confira o kit cartográfico preparado para Santana de Parnaíba. Não refaça aquisições nem transformações.

Diga quais camadas estão no GeoPackage, quais aparecem no projeto QGIS e se os arquivos continuam íntegros. Resuma também os SRCs: quais camadas preservam EPSG:4674 e quais versões de trabalho estão em EPSG:31983.

Se encontrar algum problema, explique antes de corrigir. Se estiver tudo certo, apenas confirme e aguarde nossa escolha.
```

### Função didática

Mostrar que o Work pode retomar um ambiente existente e inspecionar artefatos, em vez de produzir tudo novamente.

---

# CARDÁPIO NEGOCIADO

Apresentar oralmente quatro caminhos seguros. A turma escolhe um primeiro produto; os demais permanecem disponíveis para rodadas extras.

| Módulo | Material principal | Produto possível | Ideia que ensina |
|---|---|---|---|
| **Censo** | setores e atributos censitários | coroplético documentado | agregação, denominador, classes e contexto |
| **Escolas** | pontos escolares do OSM e Overture + tabela oficial do Censo Escolar | representação de uma fonte e comparação de coberturas | unidades diferentes, cobertura e impossibilidade de junção automática |
| **POIs** | Overture Places | categorias, seleção ou contagem | classificação, cobertura e fragmentação cadastral |
| **Relação** | setores + pontos do OSM ou Overture | pontos contextualizados por setores | dentro, perto, contagem e associação territorial |
| **Saúde — extra** | pontos de saúde do OSM e Overture + tabela CNES | representação de uma fonte e comparação de coberturas | cadastro oficial sem geometria versus fontes espaciais não exaustivas |

## PROMPT 1 — Pedir ao Work um cardápio executável

Este prompt é opcional. Use-o se for interessante mostrar que a IA também pode avaliar o material disponível.

```text
Com as camadas que já existem no kit, apresente quatro produtos que conseguimos produzir agora: um com Censo, um com escolas do OSM ou Overture, um com POIs e um relacionando setores censitários a uma camada pontual. Se houver uma quinta opção segura usando saúde, apresente-a como extra.

Para cada opção, escreva em uma linha: operação, arquivos gerados, tempo provável e principal cuidado interpretativo. Não execute nada ainda.
```

O professor pode ignorar sugestões inviáveis e negociar a escolha apenas entre os caminhos previamente simulados.

---

# MÓDULOS DE PRODUÇÃO

Executar um módulo no percurso essencial. Repetir outros apenas se houver tempo.

Em todos os módulos:

- use somente campos e geometrias que existam no kit;
- preserve a versão anterior do QGZ e das camadas derivadas;
- ao concluir, exporte o QGZ atualizado e, quando houver alteração de dados, o GeoPackage e um ZIP versionado;
- disponibilize links clicáveis para os arquivos produzidos, não apenas caminhos internos.

## MÓDULO A — Censo como base agregadora

```text
Vamos aprofundar o Censo.

Inspecione as variáveis já relacionadas às feições censitárias e proponha até três que façam sentido representar em Santana de Parnaíba. Para cada uma, diga se é total, proporção, taxa, média ou densidade e qual cuidado exige.

Use apenas as variáveis efetivamente disponíveis no kit: população total, totais de domicílios, domicílios particulares, domicílios coletivos, média de moradores em domicílios particulares ocupados, percentual de domicílios imputados, domicílios particulares ocupados, densidade populacional derivada e percentual de domicílios particulares ocupados derivado. Não proponha renda, raça, idade, escolaridade ou outra variável que não esteja na camada.

Não produza o mapa ainda. Aguarde nossa escolha da variável.
```

Após a negociação:

```text
Escolhemos [VARIÁVEL]. Prepare uma camada temática no GeoPackage e uma versão do projeto QGIS com essa representação.

Use [MÉTODO] com [NÚMERO] classes e uma paleta adequada à relação nos dados. Para as variáveis atuais, prefira uma paleta sequencial; use uma divergente somente se existir uma referência central substantivamente justificável. Registre o denominador, os limites das classes, a fonte, o período e os setores sem informação.

Não trate a característica agregada do setor como atributo individual de seus moradores. Ao terminar, diga o que devo conferir quando abrir o QGZ.
```

### Possíveis alterações curtas

```text
Agora mantenha os dados e troque apenas o método de classificação para [MÉTODO]. Salve como outro estilo para compararmos no QGIS.
```

```text
Mantenha a classificação e teste uma paleta adequada para daltonismo. Não substitua o estilo anterior.
```

---

## MÓDULO B — Escolas

```text
Vamos explorar as escolas.

Inspecione separadamente:
- os 54 objetos escolares filtrados do OSM;
- os 112 Places escolares filtrados do Overture;
- a tabela oficial com 106 escolas do Censo Escolar, que não possui geometria.

Proponha até três representações verificáveis usando como pontos apenas OSM ou Overture. Para cada opção, informe a fonte, o campo realmente disponível e o que não pode ser concluído. A tabela do Censo Escolar pode entrar como comparação de universo e atributos, mas não deve ser espacializada nem ligada aos pontos por semelhança de nome.

Não execute ainda. Aguarde nossa escolha.
```

Após a escolha:

```text
Produza a opção [OPÇÃO ESCOLHIDA] no mesmo GeoPackage e atualize uma cópia do projeto QGIS.

Preserve os pontos originais, documente filtros e valores ausentes e use uma legenda legível. Não conclua qualidade, atendimento ou acesso apenas pela presença da escola ou por seus atributos cadastrais.

Não transfira matrículas, dependência administrativa ou infraestrutura do Censo Escolar para pontos OSM ou Overture sem uma chave oficial verificada. Se a opção depender desses atributos, interrompa e explique por que ela não é executável com o kit atual.

Ao terminar, diga o que devo conferir no QGIS.
```

---

## MÓDULO C — POIs

```text
Vamos explorar os POIs do Overture.

Inspecione categorias, nomes e possíveis fragmentações. Sugira até três recortes que sejam informativos sem fingir que a base é um cadastro completo da cidade.

Não execute ainda. Aguarde nossa escolha.
```

Após a escolha:

```text
Produza o recorte [RECORTE ESCOLHIDO] no mesmo GeoPackage e atualize uma cópia do projeto QGIS.

Preserve as categorias originais, documente agrupamentos, separe registros ambíguos e não interprete ausência de POI como ausência real de atividade.

Ao terminar, apresente contagens e diga o que devo conferir no QGIS.
```

---

## MÓDULO D — Primeira relação espacial

Começar por uma relação simples e visualmente verificável. Evitar, nesta aula, transformar proximidade em acessibilidade ou associação territorial em causalidade.

```text
Vamos relacionar [CAMADA DE PONTOS] com as feições censitárias.

Use como camada de pontos somente uma camada geométrica existente: `overture_pois_4674`, `osm_equipamentos_4674` ou uma de suas visualizações filtradas de educação ou saúde. Não use as tabelas `auditoria_escolas_sem_geometria` ou `auditoria_cnes_sem_geometria` em operações espaciais.

Proponha uma operação espacial simples que possamos compreender e conferir no QGIS, como identificar em qual setor cada ponto está ou contar pontos por setor. Explique em duas frases o que a operação produz e o que ela não demonstra.

Não execute ainda. Aguarde nossa confirmação.
```

Após a confirmação:

```text
Execute a operação combinada. Preserve as camadas de entrada, salve o resultado no mesmo GeoPackage e atualize uma cópia do projeto QGIS.

Registre pontos sem correspondência, setores sem pontos, SRC usado na operação e campos criados. Não atribua automaticamente a cada ponto as características individuais dos moradores do setor.

Ao terminar, diga como conferir o resultado no QGIS.
```

---

## MÓDULO E — Saúde como rodada extra

```text
Vamos explorar saúde como uma rodada extra.

Inspecione separadamente os 25 objetos de saúde filtrados do OSM, os 109 Places de saúde filtrados do Overture e a tabela com 118 estabelecimentos do CNES sem geometria.

Proponha até duas representações usando como pontos apenas OSM ou Overture e uma comparação tabular entre as três fontes. Não trate as contagens como equivalentes, não espacialize o CNES e não conclua cobertura real de atendimento.

Não execute ainda. Aguarde nossa escolha.
```

Após a escolha:

```text
Produza a opção [OPÇÃO ESCOLHIDA] preservando as camadas originais. Documente categorias, filtros, unidade de registro, período e ausências de cada fonte.

O CNES deve permanecer como tabela oficial sem geometria. Não vincule seus registros aos pontos OSM ou Overture por nome ou proximidade sem uma chave verificável.

Ao terminar, atualize uma cópia do QGZ, exporte os arquivos produzidos e disponibilize links clicáveis.
```

---

# REABERTURA CRÍTICA NO QGIS

Depois de cada módulo, abrir o QGZ produzido e verificar:

1. A camada existe e tem a quantidade esperada de feições?
2. A tabela corresponde ao que aparece no mapa?
3. O SRC é conhecido e adequado à operação?
4. A simbologia representa a variável escolhida?
5. Classes, ausências e denominador aparecem claramente?
6. Alguma decisão foi tomada silenciosamente?
7. O resultado sustenta um achado ou apenas uma suspeita?

## PROMPT 2 — Uma correção negociada

Este prompt deve ser escrito com a turma e permanecer curto.

```text
Ao abrir o resultado no QGIS, percebemos que [PROBLEMA OU DECISÃO]. Corrija apenas isso, preserve a versão anterior e registre a mudança.
```

Exemplos: trocar paleta, rever classes, filtrar uma categoria, renomear legenda, corrigir título, separar valores ausentes ou rever um agrupamento.

---

# FECHAMENTO

## PROMPT 3 — Registrar o que o mapa acrescentou

```text
Sem fazer novas aquisições ou análises, consolide o que produzimos hoje.

Liste os arquivos e camadas criados e escreva quatro blocos curtos:
1. o que ficou observável depois da espacialização;
2. o que mudou em relação às tabelas da Aula 1;
3. o que continua ausente ou ambíguo;
4. quais perguntas dependem de relações entre camadas e devem seguir para a Aula 4.

Separe observação, interpretação e limitação. Atualize o diário cartográfico e o manifesto de camadas.
```

## Frase de passagem

> **Na Aula 1, a cidade apareceu como registro. Na Aula 2, ganhou X e Y. Na Aula 3, ganhará superfície, altura e volume. Na Aula 4, colocaremos essas representações em relação.**

---

# ROTEIRO DE VALIDAÇÃO DA SIMULAÇÃO

Registrar os tempos e ocorrências numa tabela:

| Etapa | Tempo | Arquivo utilizável? | Intervenção necessária | Decisão para a aula |
|---|---:|---|---|---|
| Prompt −1: kit | | | | |
| Abertura do QGZ | | | | |
| Tematização manual do Censo | | | | |
| Prompt 0: conferência | | | | |
| Prompt 1: cardápio | | | | |
| Primeiro módulo | | | | |
| Reabertura no QGIS | | | | |
| Prompt 2: correção | | | | |
| Segundo módulo, se houver | | | | |
| Prompt 3: fechamento | | | | |

### Perguntas que a simulação precisa responder

- O Prompt −1 produz um GeoPackage e um QGZ realmente portáteis?
- Quanto tempo leva a preparação completa?
- Qual variável censitária é mais segura para a demonstração inicial?
- Os alunos conseguem distinguir EPSG:4674 de EPSG:31983 pela operação realizada?
- Qual módulo produz o melhor resultado dentro do tempo disponível?
- O QGZ gerado pelo Work preserva fontes, estilos e caminhos relativos?
- Quantas rodadas adicionais cabem sem comprometer a discussão?
- Que decisões do Work precisam ser obrigatoriamente conferidas no QGIS?
