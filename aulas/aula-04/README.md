# Aula 4 — A cidade em muitas dimensões

A aula retorna à afirmação de que a cidade é um problema complexo e pergunta como a computação consegue operar sobre relações que não cabem numa única imagem. A resposta começa pelas dimensões: graus de liberdade, coordenadas, espaços de atributos, distância e transformação.

> **Complicado é ter muitas peças. Complexo é quando as peças mudam de comportamento por causa das relações entre elas.**

## Materiais

- [Apresentação em PDF](apresentacao/aula-04.pdf)
- [Prompts da atividade prática](prompts-aula-04.md)
- [Fontes e créditos](fontes-e-creditos.md)

## Arco da aula

> **complexidade → dimensão → coordenada → distância → projeção → muitas dimensões → redução → agrupamento → retorno ao mundo**

A aula parte da dificuldade humana de representar fenômenos complexos. A computação consegue habitar espaços multidimensionais, mas não encontra sozinha os eixos do problema: pessoas escolhem dados, unidades, distâncias, classificações, objetivos e aquilo que será descartado.

Uma escada dimensional introduz linha, plano, espaço e espaços de atributos. Descartes aproxima geometria e álgebra; Pitágoras reaparece na distância euclidiana; *Flatland* ajuda a imaginar os limites de uma percepção presa a poucas dimensões. Bellman apresenta a explosão combinatória e a maldição da dimensionalidade. Mandelbrot e a fractalidade urbana aparecem como fronteira, não como centro da aula.

A redução dimensional é introduzida geometricamente. Na PCA, os pontos não mudam: mudam as direções usadas para descrevê-los. Autovetores indicam as direções dos novos eixos; autovalores indicam quanta variação cada direção carrega.

O percurso culmina numa pergunta crítica: modelos multidimensionais descobrem estruturas da cidade ou tornam visíveis as consequências das dimensões que escolhemos?

## Arquitetura da prática

> **1D distribuir → 2D relacionar → 3D girar → ND reduzir → mundo comparar**

O Prompt −1 retoma o laboratório de Santana de Parnaíba e prepara duas unidades de análise: edifícios e setores censitários. Calcula dimensões morfológicas, associa presença e altura estimadas, organiza população e rendimento como contexto setorial e registra cobertura, ausências e limitações.

Durante a aula:

1. histogramas mostram como uma dimensão produz ordem e como escalas linear e logarítmica tornam diferentes partes da distribuição visíveis;
2. área e altura formam um espaço bidimensional;
3. a compacidade acrescenta uma terceira dimensão e a rotação do gráfico revela também o poder enganador da câmera;
4. duas PCA permitem comparar uma entrada ingênua com uma seleção consciente de dimensões;
5. agrupamentos recebem uma taxonomia explicitamente humana;
6. vizinhos geográficos são comparados a vizinhos no espaço de atributos.

O fechamento retira uma dimensão e recalcula a vizinhança. Se os vizinhos mudam, a semelhança não estava apenas nos edifícios: estava também no espaço construído para compará-los.

## Cuidado central

Redução, distância, agrupamento e classificação ampliam nossa capacidade de operar, mas não são neutros. A prática separa o que veio das fontes, o que foi inferido, o que foi calculado, o que foi escolhido e o que continua ausente.

> **Para operar, a computação precisa reduzir. Toda redução apaga. A violência começa quando esquecemos o apagamento e chamamos a representação de realidade.**
