# Prompts da investigação ao vivo — Aula 1

## Quem produz a cidade que aparece nos dados?

> Versão reproduzível para uso em sala e estudo posterior. A cidade é escolhida e registrada uma única vez no PROMPT 0; os prompts seguintes reutilizam esse registro. Nesta aula, mesmo as fontes espaciais serão apresentadas apenas como números, tabelas e gráficos; os mapas entram na Aula 2.

> **Regra de entrega:** caminhos internos não bastam. Ao final de cada etapa, além de preservar os arquivos na estrutura do projeto, disponibilize como arquivos clicáveis os principais CSVs e gráficos produzidos e mostre os gráficos diretamente na conversa quando o ambiente permitir. Não exporte novamente as bases nacionais pesadas.

---

## PROMPT −1 — Preparar o ambiente e as bases nacionais

```text
Estamos iniciando um projeto didático de investigação urbana para a disciplina Big Open Urban Data.

A pergunta central da aula é: “Quem produz a cidade que aparece nos dados?”

Atue como assistente operacional e crítico. Você pode descobrir fontes, obter arquivos, escrever e executar código, documentar procedimentos, organizar tabelas e produzir gráficos. Você não deve escolher sozinho o que é relevante, tratar resultados como verdade automática nem substituir o julgamento do professor e da turma.

Princípios:
- rastro não equivale ao fenômeno;
- mais dados não produzem automaticamente mais verdade;
- ausência de registro não significa ausência do fenômeno;
- toda fonte possui produtor, finalidade, unidade, temporalidade, classificação e condições de acesso;
- toda transformação deve ser documentada;
- não produziremos mapas nesta aula;
- perguntas espaciais serão guardadas para a Aula 2.

Fontes principais: IBGE/Censo, OpenStreetMap, Overture Places e Censo Escolar. O CNES será uma extensão opcional.

Antes da escolha da cidade, prepare integralmente os recursos nacionais estáveis e reutilizáveis cuja aquisição durante a aula produziria espera improdutiva. Esta mensagem já autoriza os downloads e processamentos necessários; não aguarde nova aprovação.

Adquira e prepare:
- cadastro nacional de municípios, UFs e códigos IBGE;
- população municipal do Censo 2022;
- malha municipal nacional oficial mais recente, preservando o arquivo original e produzindo também um derivado eficiente para selecionar qualquer município após o PROMPT 0;
- pacote oficial mais recente do Censo Escolar, incluindo dicionário e documentação, convertido também para um formato aberto e eficiente que permita filtragem municipal;
- dicionários, notas técnicas, licenças e metadados correspondentes.

Antes de cada aquisição, confirme em fonte oficial a URL direta, o período ou versão, o tamanho real, o conteúdo, o formato e as condições de uso. Se uma fonte estiver indisponível, ambígua ou tiver sido substituída, não invente uma alternativa silenciosa: registre o problema e adote apenas uma fonte oficial equivalente claramente documentada.

Nesta aula, a malha municipal será usada somente para identificar e filtrar o território da cidade escolhida. Não produza nem exiba mapas; guarde as perguntas espaciais para a Aula 2.

Não prepare o CNES neste momento; ele será uma extensão opcional. Não faça previamente consultas municipais ao OSM ou ao Overture Places; essas aquisições integram a investigação ao vivo. Prepare apenas os procedimentos e a documentação necessários para executá-las depois da escolha da cidade.

Crie a estrutura:
atividade-aula-01/
  bases-nacionais/
  cidade-escolhida/
  resultados/
  graficos/
  prompts/
  registro/

Crie em registro/ um manifesto-bases.md e um diario-investigacao.md. Para cada base registre instituição, URL, data de acesso, versão/período, licença, tamanho, início e término da aquisição, transformação, formato final, integridade e limitações.

Use formatos abertos e eficientes. Preserve os arquivos originais e produza derivados separados. Ao terminar, apresente uma tabela curta dos arquivos efetivamente criados, com caminhos e tamanhos, e informe qualquer aquisição interrompida ou incompleta. Não escolha uma cidade nem inicie as quatro investigações. Aguarde o PROMPT 0.
```

---

## PROMPT 0A — Reunir cidades candidatas

```text
Ajude a turma a reunir cidades brasileiras candidatas para a investigação. Ainda não recomende uma vencedora nem processe as quatro fontes principais.

Critérios obrigatórios:
- pelo menos 50.000 habitantes no Censo 2022;
- não ser capital estadual;
- possuir código IBGE inequívoco;
- operação atual da Uber confirmada em página oficial;
- presença verificável no Airbnb;
- dados municipais disponíveis no IBGE;
- potencial de registros no OSM, Overture Places, Censo Escolar e CNES;
- combinação interessante de funções ou conflitos urbanos.

Desejável: cidade pequena ou média, fora do núcleo contínuo de grande metrópole, com diversidade interna, econômica, ambiental, turística, universitária, industrial ou regional.

Procedimento:
1. receba até três candidatas da turma;
2. se ainda faltarem opções, proponha no máximo três cidades adicionais;
3. verifique os critérios em fontes atuais e cite links diretos;
4. apresente cidade/UF, população 2022, Uber, Airbnb, diversidade potencial e riscos técnicos;
5. marque cada critério como confirmado, incerto ou não atendido;
6. encerre com uma tabela curta, sem classificar uma vencedora;
7. aguarde os critérios que a turma desejar acrescentar ou modificar.

Não escolha automaticamente a cidade com mais dados. Neste momento, apenas torne as alternativas comparáveis.
```

---

## PROMPT 0B — Comparar e decidir com a turma

```text
Estamos avaliando as seguintes cidades para uma investigação ao vivo: Santana de Parnaíba/SP, Lauro de Freitas/BA, Santo André/SP

A turma definiu estes critérios: [CRITÉRIOS NEGOCIADOS EM AULA]. Considere também os critérios técnicos confirmados no PROMPT 0A.

1. Produza uma tabela comparativa curta, adequada para projeção em uma aula online.
2. Para cada cidade, mostre potencial investigativo, contrastes esperados entre fontes, riscos técnicos e incertezas.
3. Explique quais critérios favorecem cada alternativa; não esconda conflitos entre eles.
4. Recomende a cidade que possa produzir a investigação pedagogicamente mais interessante — não simplesmente aquela com maior disponibilidade de dados.
5. Apresente a recomendação como argumento aberto à contestação da turma.
6. Aguarde a decisão coletiva antes de baixar ou processar recortes municipais.

Depois da decisão humana, receba apenas o nome da cidade escolhida — e a UF quando necessária para eliminar homônimos. Resolva e confirme internamente nome oficial, UF e código IBGE no cadastro já preparado. Registre esses identificadores em `registro/municipio-escolhido.json`, registre escolha, alternativas e critérios no diário, prepare as pastas da cidade e aguarde o PROMPT 1. Nos prompts seguintes, reutilize esse registro sem pedir novamente nome, UF ou código ao usuário.
```

---

## PROMPT 1 — Retrato censitário

```text
Leia nome oficial, UF e código IBGE em `registro/municipio-escolhido.json`. Usando prioritariamente fontes oficiais do IBGE, construa um retrato numérico conciso do município já escolhido. Não produza mapas. Se o registro não existir ou for ambíguo, interrompa e peça que o PROMPT 0 seja concluído; não peça ao usuário que procure o código IBGE.

1. Confirme nome, UF e código IBGE do único município estudado.
2. Obtenha população no Censo 2022, trajetória censitária, domicílios, densidade oficial e até três variáveis adicionais claras.
3. Produza uma tabela com valor, ano, unidade e fonte; no máximo dois gráficos; composição interna por categorias ou evolução temporal quando metodologicamente possível; três achados descritivos; três ressalvas.
4. Não misture Censo e estimativas sem rotulá-los.
5. Não use “alto”, “baixo”, “jovem”, “pobre” ou “denso” sem uma referência explícita. Prefira descrever valores, proporções e evolução sem criar comparação com outros municípios.
6. Atualize o diário e salve dados processados em CSV ou Parquet e gráficos em PNG ou SVG.

Encerre com: o que se tornou observável; o que permaneceu difícil; o que os dados não permitem concluir.
```

---

## PROMPT 2 — Inventário colaborativo do OpenStreetMap

```text
Leia nome oficial, UF e código IBGE em `registro/municipio-escolhido.json`. Consulte o OpenStreetMap para o município já escolhido. Não produza mapas. Se o registro não existir ou for ambíguo, interrompa e peça que o PROMPT 0 seja concluído; não peça ao usuário que procure o código IBGE.

1. Identifique a relação administrativa municipal do OSM e verifique conjuntamente `name`, UF, `admin_level=8` e o código IBGE registrado. Procure primeiro a chave `IBGE:GEOCODIGO` com esse código; teste também `ref:IBGE`, pois a convenção pode variar entre relações. Não suponha que uma única chave seja universal.
2. Se nenhuma relação inequívoca for encontrada pelas etiquetas, use o limite oficial municipal já extraído no PROMPT 0 para realizar o filtro espacial e registre essa mudança de método. Não escolha uma relação apenas pela semelhança do nome.
3. Preserve a identificação da relação, a consulta inicial, eventuais tentativas sem resultado e a consulta efetivamente utilizada. Quando empregar uma relação, converta-a em área de consulta pelo procedimento apropriado, como `map_to_area`, e documente a operação.
4. Evite baixar indiscriminadamente um volume excessivo; explique qualquer recorte ou amostragem.
5. Produza contagens por grandes famílias: vias e caminhos, edifícios, equipamentos, comércio e serviços, saúde, educação, religião, lazer e espaços públicos.
6. Para as famílias principais, informe quantidade, presença de nome, categoria útil e ausências frequentes.
7. Não some nós, caminhos e relações como se fossem necessariamente objetos independentes; explique como tratou duplicações e sobreposições entre famílias.
8. Gere uma tabela, no máximo dois gráficos e um resumo de sinais de detalhamento ou incompletude.
9. Não conclua que uma atividade inexiste porque não está registrada. Ausência de uma etiqueta indica falta de registro daquele atributo, não ausência urbana comprovada.
10. Guarde as consultas, os dados processados e o registro das transformações.

Encerre com: o que o OSM tornou observável; o que pode refletir a comunidade de mapeamento; o que não pode ser concluído apenas pelas contagens.
```

---

## PROMPT 3 — Atividades reconhecidas no Overture Places

```text
Leia nome oficial, UF, código IBGE e limite municipal nos registros produzidos pelo PROMPT 0. Usando a versão atual documentada do Overture Maps e o tema Places, extraia os registros do município já escolhido. Não produza mapas. Se o registro não existir ou for ambíguo, interrompa e peça que o PROMPT 0 seja concluído; não peça ao usuário que procure o código IBGE.

1. Informe release, documentação, origem do limite, campos, método de consulta, custos e limites.
2. Produza total de registros, grandes famílias, dez categorias mais frequentes, indicador explicado de diversidade e preenchimento de nomes/campos relevantes.
3. Preserve uma tabela entre categorias originais e famílias criadas.
4. Identifique possíveis duplicações, registros sem categoria e limites de atualização.
5. Mostre a cauda de categorias raras, sem confundir raridade na base com raridade urbana.
6. Não compare diretamente as contagens com outra base: preserve as unidades e categorias próprias do Overture.
7. Produza no máximo dois gráficos e três hipóteses para padrões ou inconsistências internas.
8. Atualize o diário e salve os dados, correspondências e resultados.

Encerre com: o que a integração tornou observável; quais decisões de esquema participaram; qual divergência merece investigação.
```

---

## PROMPT OPCIONAL — Perseguir um número estranho

> Use depois de qualquer fonte quando uma contagem parecer surpreendente, implausível ou ambígua. A escolha do número pertence ao professor e à turma.

```text
Antes de prosseguir, investigue somente este resultado que a turma decidiu estranhar: [RESULTADO OU CATEGORIA].

1. Abra as unidades que compõem a contagem e preserve seus identificadores e categorias originais.
2. Mostre uma tabela curta com os atributos necessários para compreender o que está sendo contado.
3. Verifique rótulos repetidos, nomes normalizados, vínculos organizacionais aparentes, unidades diferentes reunidas na mesma classe e possíveis fragmentações.
4. Não suponha que nomes distintos representam organizações independentes nem que nomes semelhantes representam a mesma entidade.
5. Explique em até três parágrafos qual parece ser a unidade de representação e por que o número não deve ser interpretado literalmente.
6. Não produza mapas, não altere o resultado anterior e não amplie a investigação para outras fontes.

Registre no diário a pergunta formulada pela turma, a evidência examinada e como a interpretação da contagem foi modificada. Depois aguarde a próxima instrução.
```

---

## PROMPT 4 — Retrato do Censo Escolar

```text
Leia nome oficial, UF e código IBGE em `registro/municipio-escolhido.json`. Usando os microdados oficiais mais recentes do Censo Escolar/INEP, construa um retrato do município já escolhido. Não produza mapas. Se o registro não existir ou for ambíguo, interrompa e peça que o PROMPT 0 seja concluído; não peça ao usuário que procure o código IBGE.

1. Declare ano, data de referência, unidade observada, situação de funcionamento e arquivo utilizado.
2. Conte escolas e matrículas por dependência administrativa, urbano/rural, etapas, tempo integral e dimensões de infraestrutura selecionadas com base no dicionário.
3. Calcule no máximo dois indicadores populacionais somente com denominadores compatíveis e documentados.
4. Descreva a composição interna do município por etapas, dependência administrativa e dimensões de infraestrutura selecionadas.
5. Não converta número de escolas ou matrículas em qualidade, vagas ou acesso efetivo.
6. Produza tabela, no máximo dois gráficos, três achados e três ressalvas.
7. Atualize o diário e salve os derivados.

Encerre com: o que o cadastro mede; o que seria necessário para falar de atendimento e acesso; que pergunta exige localização na Aula 2.
```

---

## PROMPT EXTRA — CNES

```text
Leia nome oficial, UF e código IBGE em `registro/municipio-escolhido.json`. Usando dados oficiais do CNES/DATASUS, construa um retrato dos estabelecimentos de saúde do município já escolhido. Não produza mapas nesta etapa. Se o registro não existir ou for ambíguo, interrompa e peça que o PROMPT 0 seja concluído; não peça ao usuário que procure o código IBGE.

1. Declare competência, situação cadastral, unidade observada e arquivo.
2. Conte estabelecimentos ativos por grandes tipos e, quando seguro, por esfera/natureza e atendimento ao SUS.
3. Calcule no máximo dois indicadores populacionais, explicitando diferenças de ano.
4. Audite latitude e longitude: ausentes, repetidas, centroide municipal, fora do limite ou incompatíveis.
5. Não converta presença cadastral em capacidade, qualidade ou acesso.
6. Produza tabela, no máximo dois gráficos, achados e ressalvas.
7. Atualize o diário e preserve um arquivo pronto para espacialização na Aula 2.

Encerre com: o que o CNES mede; o que falta para falar de acesso; quais problemas de localização precisam ser verificados.
```

---

## PROMPT 5 — Síntese crítica

```text
Sem novas aquisições e sem mapas, reúna os resultados validados das quatro fontes centrais: IBGE/Censo, OpenStreetMap, Overture Places e Censo Escolar. Se o CNES opcional já tiver sido executado, apresente-o somente em um apêndice curto, sem transformá-lo numa quinta fonte obrigatória da narrativa principal.

1. Crie uma tabela para as quatro fontes centrais com: produtor, finalidade, unidade, período, acesso/licença, transformação, dimensão observável, ausência esperada, afirmação defensável e afirmação não sustentada.
2. Liste convergências e divergências sem resolvê-las automaticamente.
3. Retome as expectativas iniciais e classifique-as como confirmadas, tensionadas, não testadas ou mal formuladas.
4. Formule de cinco a oito novas perguntas; pelo menos metade deve exigir localização, distribuição, distância, vizinhança, escala ou agregação espacial.
5. Atualize o diário e produza um índice de arquivos com fonte e finalidade.
6. Disponibilize `sintese-quatro-fontes.md` e `indice-arquivos.csv` como arquivos clicáveis e confirme a quantidade real de entradas do índice a partir do próprio CSV exportado.

Termine com uma síntese curta: “A cidade que apareceu nos dados foi produzida por…”
```

---

## Regra de interrupção

Se uma fonte falhar, não invente substitutos silenciosamente. Registre a falha, explique se ela é técnica, institucional, semântica ou temporal e ofereça três opções: corrigir ao vivo, usar o plano B documentado ou seguir sem a fonte.

---

## PROMPT FINAL — Exportar, encerrar e limpar o Work

> Use somente depois de baixar os resultados que devem ser preservados. A exclusão é intencional e exige que a tarefa tenha terminado.

```text
O ensaio foi encerrado e os resultados que precisavam ser preservados já foram exportados. Esta mensagem autoriza a exclusão integral dos arquivos internos produzidos por esta atividade.

1. Elimine todo o diretório interno `atividade-aula-01/`, incluindo bases nacionais, originais, derivados, recortes municipais, consultas, scripts, resultados, gráficos, registros, checksums, arquivos temporários e caches criados especificamente para a atividade.
2. Elimine também qualquer arquivo produzido pela investigação experimental do Airbnb ou por outras extensões realizadas neste mesmo ensaio, caso esteja fora de `atividade-aula-01/`.
3. Não apague arquivos exportados para a pasta de entregáveis do usuário nem arquivos que não tenham sido criados por esta atividade.
4. Não crie cópia de segurança, pacote compactado ou duplicata antes da exclusão.
5. Depois da limpeza, verifique se ainda existe algum arquivo interno relacionado à atividade e informe exatamente o que foi removido, o que permaneceu e por quê.

Encerre com uma despedida curta. Não inicie novas aquisições, análises ou tarefas.
```
