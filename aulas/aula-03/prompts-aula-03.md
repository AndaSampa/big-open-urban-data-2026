# Prompts da atividade prática — Aula 3

## Terreno, forma edificada e altura em Santana de Parnaíba

> O Prompt −1 é executado antes da aula porque envolve descoberta, aquisição e validação de arquivos pesados. Em sala, os prompts seguintes são curtos e incrementais: o objetivo é aprender a formular o que se deseja investigar, conferir o resultado e ajustar o pedido — não decorar comandos nem produzir um mapa final automático.

> **Regra de continuidade:** reutilize a cidade e os arquivos produzidos nas aulas anteriores sempre que estiverem íntegros. Preserve originais e não altere os projetos-base. Toda nova representação deve ser salva como cópia verificável.

---

## PROMPT −1 — Preparar o laboratório antes da aula

```text
Prepare um projeto de geoprocessamento para estudar a morfologia urbana de Santana de Parnaíba.

1. Obtenha ou reutilize o limite municipal oficial.
2. Procure o melhor modelo aberto de terreno disponível para o município, na menor resolução adequada. Priorize um MDT, isto é, uma representação do terreno com edifícios e vegetação removidos. Se não houver levantamento local aberto e verificável, use o FABDEM, com resolução aproximada de 30 m, e registre essa decisão.
3. Recorte o modelo pelo limite municipal e organize produtos que permitam explorar hipsometria, curvas de nível e declividade.
4. Baixe as geometrias de edificações do Google Open Buildings V3 para o município. Preserve a geometria e os atributos úteis, incluindo área e confiança.
5. Obtenha a estimativa de altura de edifícios do Open Buildings Temporal 2.5D, escolhendo um período comum e documentado.
6. Verifique sistemas de referência, unidades, resolução, extensão e sobreposição entre todas as camadas. Para cálculos locais, use SIRGAS 2000 / UTM 23S, EPSG:31983.
7. Organize um GeoPackage com limite, curvas, edificações e metadados. Mantenha os rasters em formato apropriado e use caminhos relativos.
8. Salve um projeto QGIS limpo. Deixe visíveis apenas o limite e o modelo de terreno; mantenha as demais camadas disponíveis, mas desligadas.

Preserve os arquivos originais, registre fontes, datas, licenças, transformações e limitações e valide programaticamente a entrega. Não produza um mapa temático final nem antecipe conclusões: o projeto deve abrir espaço para a exploração em aula.

Ao concluir, indique o caminho do projeto QGIS, resuma as camadas disponíveis e explique qualquer substituição ou limitação importante.
```

### Resultado do ensaio

O preparo completo levou cerca de 28 minutos e produziu um projeto utilizável com limite municipal, FABDEM, declividade, curvas de nível, geometrias do Open Buildings V3 e rasters de presença e altura do Open Buildings Temporal 2.5D. O dado LiDAR do GeoSampa não foi usado porque sua cobertura oficial se restringe ao Município de São Paulo.

---

## PROMPT 1 — Entender e representar o terreno

```text
Abra o projeto de morfologia urbana de Santana de Parnaíba e trabalhe com o modelo de terreno já preparado.

Crie uma cópia do projeto para a exploração topográfica, sem alterar o projeto-base. Faça uma representação hipsométrica clara e acrescente uma leitura derivada que ajude a entender a forma do relevo: curvas de nível, declividade ou relevo sombreado.

Mostre a faixa de altitudes, a resolução do dado e pelo menos duas observações espaciais que possam ser feitas a partir da representação. Explique também o que esse modelo de aproximadamente 30 m não permite afirmar.

Salve a nova versão do projeto e, se possível, exporte uma imagem simples para conferência. Não transforme o resultado em mapa final nem esconda as decisões de representação.
```

### Reabertura no QGIS

1. Conferir se o projeto-base permaneceu intacto.
2. Alternar hipsometria, relevo sombreado, declividade e curvas.
3. Inspecionar os valores mínimo e máximo do raster.
4. Perguntar: **as curvas de nível revelam algo que a matriz não revelava, ou apenas traduzem a superfície para outra linguagem?**

---

## PROMPT 2 — Mapear a forma edificada

```text
No projeto de morfologia urbana de Santana de Parnaíba, carregue as geometrias de edificações do Open Buildings e represente-as de modo legível sobre o município.

Calcule medidas simples que ajudem a descrever a ocupação construída, como número de polígonos, área de implantação de cada edifício, área total ocupada, distribuição por classes de tamanho e densidade de área edificada em uma divisão espacial adequada.

Escolha uma ou duas dessas medidas para tematizar no mapa. Mostre os resultados e formule duas observações sobre a morfologia urbana. Lembre que cada polígono é uma inferência de edifício e não equivale automaticamente a imóvel, domicílio ou uso.
```

### Reabertura no QGIS

1. Conferir a sobreposição entre polígonos e imagem de referência.
2. Examinar uma amostra de confianças e áreas.
3. Identificar omissões, comissões e divisões estranhas de footprints.
4. Separar o que o mapa mostra do que ele apenas sugere sobre o tecido urbano.

---

## PROMPT 3 — Introduzir a altura dos edifícios

```text
Associe a melhor estimativa disponível de altura do Open Buildings Temporal 2.5D às geometrias de edificações de Santana de Parnaíba.

Verifique primeiro se resolução, presença de edifício, unidades e sobreposição permitem essa associação. Depois explore algumas medidas possíveis: distribuição das alturas, classes de altura no mapa, número aproximado de pavimentos — deixando explícita a altura média adotada por pavimento — e volume edificado aproximado, combinando implantação e altura.

Produza uma representação e um gráfico ou resumo numérico simples. Diferencie dado observado, inferência do produto e estimativa criada por você. Não apresente pavimentos ou volume como informação cadastral exata.
```

### Reabertura no QGIS

1. Verificar como o raster de 4 m foi resumido dentro de cada polígono.
2. Conferir edifícios sem valor ou com valores implausíveis.
3. Comparar altura estimada, pavimentos inferidos e volume aproximado.
4. Manter explícita a diferença entre altura relativa ao terreno e elevação absoluta.

---

## PROMPT 4 — Compor uma leitura da morfologia urbana

```text
Faça uma composição que relacione o terreno a pelo menos dois atributos da forma edificada de Santana de Parnaíba, por exemplo implantação, tamanho, densidade ou altura.

O resultado deve permitir responder:
1. Que relações espaciais aparecem quando terreno e edificações são vistos juntos?
2. Quais três observações podem ser formuladas a partir do mapa?
3. Que nova pergunta a representação produz?
4. Que informação importante sobre a cidade continua ausente ou mal representada?

Priorize legibilidade e comparação. Não tente colocar todas as variáveis no mesmo mapa e não trate correlação visual como explicação causal.
```

---

# Fechamento crítico da prática

Ao final, separar coletivamente:

- o que veio diretamente de uma fonte;
- o que foi inferido por um modelo;
- o que foi calculado durante a aula;
- o que dependeu de uma escolha de representação;
- o que continua invisível.

A atividade não busca concluir como Santana de Parnaíba “é”. Ela testa o que passa a existir visual e analiticamente quando a cidade recebe terreno, superfície, altura e volume.
