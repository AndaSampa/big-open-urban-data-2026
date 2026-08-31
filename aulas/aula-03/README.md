# Aula 3 — O que passa a existir quando conseguimos olhar mais de perto?

A aula acrescenta o eixo Z à investigação. Parte da Blue Marble e da aparente lisura da Terra para discutir escala, forma terrestre, geoide e referências verticais; aproxima-se do terreno por meio de modelos de elevação; distingue terreno, superfície e altura de objetos; e chega à cidade como nuvem de pontos, edifícios, cobertura, volume e mudança no tempo.

> **Material em revisão local.** A apresentação e os prompts já foram organizados na estrutura do curso, mas esta versão ainda não deve ser publicada antes da conferência do professor.

## Materiais

- [Apresentação em PDF](apresentacao/aula-03.pdf)
- [Prompts da atividade prática](prompts-aula-03.md)
- [Fontes e créditos](fontes-e-creditos.md)

## Arco da aula

> **planeta → referência vertical → terreno → superfície → edifício → nuvem de pontos → excesso do mensurável → problema de representação**

A primeira parte trabalha a diferença entre olhar a Terra de longe e perceber sua profundidade. O terreno aparece como uma superfície modelada e amostrada: DEM, MDT e MDS não são sinônimos perfeitos, e toda altura depende de uma referência.

Santana de Parnaíba aproxima o problema da escala municipal. Um MDT aberto de aproximadamente 30 m permite tematizar a hipsometria, derivar declividade e extrair curvas de nível, mas também permite perguntar se a curva ainda é necessária quando cada célula já possui um valor Z.

Depois, a aula passa do terreno à superfície construída. O Google Open Buildings oferece geometrias inferidas de edifícios; o Open Buildings Temporal 2.5D acrescenta presença e altura estimada. A transição para São Paulo e para o LiDAR amplia deliberadamente o número de coisas mensuráveis: retornos, classes, terreno, superfície, altura acima do solo, objetos, métricas e mudança no tempo.

Essa overdose desemboca na pergunta que orientará a seção conceitual ainda em desenvolvimento:

> **Como representar essa nova escala e essa nova profundidade?**

O fechamento previsto retorna a John Snow: poucos dados, uma relação espacial visível e a abertura para associações entre morfologia arquitetônica e saúde, saúde mental, clima, violência, conforto térmico, risco e eventos extremos.

## Arquitetura da prática

> **preparo prévio → terreno → forma edificada → altura → composição e pergunta**

O Prompt −1 prepara antecipadamente o projeto QGIS, o GeoPackage e as fontes mais demoradas. Durante a aula, quatro prompts curtos permitem conduzir a investigação sem transformar o encontro num tutorial técnico. O LiDAR permanece na exposição e na demonstração direta do professor; não integra a sequência de prompts.

O ensaio completo do Prompt −1 levou aproximadamente **28 minutos**. O Prompt 1, dedicado ao terreno, levou aproximadamente **3 minutos**. Os demais foram intencionalmente deixados abertos para negociação e gestão durante a aula.

## Passagem para a Aula 4

Depois de registro, X/Y e Z, a investigação poderá relacionar representações diferentes e perguntar quando uma associação espacial começa — ou não — a constituir evidência.
