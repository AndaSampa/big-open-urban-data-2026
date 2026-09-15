# Aula 5 — QGIS como sistema de leitura da cidade

A última aula reúne as representações construídas ao longo do curso num GeoPortal local de Santana de Parnaíba. Em vez de reexecutar processos longos, percorremos resultados já produzidos e perguntamos o que cada operação permite perceber — e o que continua sem resposta.

> **Uma pergunta sobre a cidade → um resultado produzido com dados → uma leitura possível e seus limites.**

## Materiais

- [Apresentação em PDF](apresentacao/aula-05.pdf)
- [Prompts da atividade prática](prompts-aula-05.md)
- [Vídeo do percurso solar](materiais/percurso-solar.mp4)
- [Fontes e créditos](fontes-e-creditos.md)

## Arco da aula

> **GeoPortal → geometrias → raster → rede → 3D → tempo → classificação → interpretação**

O QGIS aparece como um sistema capaz de reunir pontos, linhas, polígonos, rasters, atributos e modelos numa mesma leitura territorial. O projeto permite ligar e desligar temas, comparar representações e retornar continuamente da abstração ao município.

A hidrologia experimental mostra como uma rede pode emergir das relações entre alturas do terreno. Direção e acumulação de fluxo são convertidas em cursos d'água candidatos por meio de um limiar de contribuição escolhido. O resultado não é apresentado como mapa de inundação: ele formula uma pergunta que exigiria chuva, drenagem urbana, verificação de campo e modelagem hidráulica para ser respondida.

O GTFS apresenta o transporte público como um sistema relacional de rotas, viagens, formas, paradas e horários. A proximidade euclidiana de 500 metros é comparada a população, rendimento, relevo e ocupação, sem ser confundida com caminhabilidade, frequência ou acesso efetivo.

O modelo tridimensional leva um recorte do município do QGIS ao Blender. Terreno, edifícios e vias ganham volume, câmera, materiais e luz. Um percurso solar de 21 de junho acrescenta o tempo à representação, mas permanece uma demonstração visual, não um estudo de insolação de precisão.

## Uma pendência da Aula 4

A aula retorna aos agrupamentos morfológicos porque os edifícios altos não formaram uma categoria espacialmente evidente. Três formulações são comparadas:

1. agrupamento original;
2. agrupamento com maior peso para altura;
3. regra explícita para edifícios com pelo menos 20 metros.

Os mesmos dados produzem organizações diferentes quando mudamos a geometria do problema. Um notebook curto apresenta as distribuições de altura, área e compacidade em cada grupo, permitindo descrever suas assinaturas sem atribuir automaticamente uso, idade, renda ou qualidade arquitetônica.

## Fechamento

O QGIS não encerra a interpretação. Ele organiza representações e permite colocá-las em relação. Os prompts não escolhem o que merece atenção: essa escolha continua sendo urbanística, metodológica e humana.

> **Qual pensamento fica fora dos dados e dos modelos?**
