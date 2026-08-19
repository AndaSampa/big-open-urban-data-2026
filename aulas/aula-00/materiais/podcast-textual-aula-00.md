# Podcast textual — Aula 0

## Big Open Urban Data — Representação, complexidade e investigação

**Apresentação:** 75 lâminas  
**Duração estimada:** 80–100 minutos de fala contínua  
**Uso:** roteiro para estudo do professor, gravação futura e material complementar dos alunos

## Convenções

- O texto principal foi escrito para ser falado, não como resumo de tópicos.
- Indicações entre colchetes, como `[pausa]`, não precisam ser lidas.
- “Na lâmina” indica algo que deve ser observado na imagem projetada.
- As transições fazem parte do roteiro: elas explicitam por que um assunto conduz ao seguinte.
- Citações literais curtas são identificadas. As demais formulações atribuídas a autores são paráfrases.

---

# Capítulo 1 — Chegada: uma ausência que produz cidade

## Lâmina 01 — O mapa que não mostra tudo

Bem-vindas e bem-vindos ao curso Big Open Urban Data. Quero começar não por uma definição de dados, por um software ou por uma lista de conteúdos, mas por uma pequena perturbação. A notícia que aparece nesta lâmina fala de lombadas instaladas por moradores ou agentes locais em Paraisópolis e posteriormente retiradas pela polícia. O episódio interessa porque existe primeiro como situação urbana: pessoas atravessam uma rua, percebem um risco, produzem uma intervenção física e reorganizam, ainda que provisoriamente, a circulação.

Mas essa realidade pode não aparecer em um mapa oficial, em um cadastro viário ou em uma base sobre dispositivos de trânsito. Ausência no mapa não significa ausência na cidade. Ao mesmo tempo, quando algo não aparece nas representações oficiais, sua capacidade de existir publicamente, disputar recursos ou orientar políticas pode ficar reduzida. Esse será um dos problemas centrais do curso: como certos fenômenos urbanos tornam-se dados, mapas e argumentos, enquanto outros permanecem invisíveis, informais ou classificados como erro.

Não partiremos da ideia de que os dados mentem ou de que os mapas são inúteis. Partiremos de uma pergunta mais cuidadosa: quais operações fizeram com que uma situação urbana se tornasse — ou não se tornasse — uma evidência reconhecível?

## Lâmina 02 — Quem está falando

Antes de seguir, quero me apresentar a partir dos problemas que me trouxeram até aqui. Meu percurso combina arquitetura, urbanismo, representação, dados urbanos, cartografia e inteligência artificial. Isso não significa que eu tenha chegado a uma síntese final entre esses campos. Significa que fui encontrando situações nas quais nenhuma disciplina, isoladamente, parecia suficiente.

Ao trabalhar com cidades, imagens, sensores, modelos tridimensionais ou bases públicas, comecei a perceber uma questão recorrente: toda ferramenta torna algumas coisas muito visíveis e outras difíceis de perceber. Um levantamento pode produzir precisão geométrica e, ainda assim, não registrar a forma como um espaço é usado. Uma visualização pode revelar um padrão e simultaneamente esconder como os dados foram produzidos. Uma inteligência artificial pode responder com fluência e não possuir experiência, responsabilidade ou compromisso com a fonte.

É desse lugar que este curso será conduzido. Não como uma oficina neutra de ferramentas, mas como uma investigação sobre o que fazemos quando transformamos cidades em inscrições manipuláveis. Minha expectativa não é que vocês adotem minhas respostas, mas que aprendamos a formular perguntas melhores e a documentar as decisões que tornam nossas respostas possíveis.

## Lâmina 03 — Quem está ouvindo e de onde olha

Agora é importante que a turma também apareça. Toda leitura urbana parte de uma posição: uma formação profissional, uma cidade conhecida, um repertório visual, uma experiência de mobilidade, moradia, trabalho ou cuidado. Isso não invalida a investigação; ao contrário, oferece um ponto de partida que precisa tornar-se consciente e discutível.

[Se este roteiro for usado como podcast para alunos, faça aqui uma pausa de alguns segundos.] Pense na cidade que você conhece melhor. Qual elemento dela aparece mal nos mapas? Pode ser uma viela, um curso d’água enterrado, uma prática de cuidado, um comércio temporário, uma rota informal ou mesmo uma atmosfera difícil de quantificar. Agora pense no contrário: existe alguma representação que tenha moldado excessivamente a forma como você imagina uma cidade que quase não conhece?

Essas duas perguntas — o que não aparece e o que aparece com força demais — ajudam a situar o curso. Não existe observador sem posição, mas existe diferença entre uma posição ocultada e uma posição declarada, examinada e confrontada com outras evidências.

---

# Capítulo 2 — O curso e a matriz da investigação

## Lâmina 04 — Agora vamos apresentar o curso

Esta é uma lâmina de localização. Ao longo da aula, usaremos metapainéis como este para que ninguém precise adivinhar onde estamos ou por que mudamos de assunto. Neste primeiro bloco, apresentarei a disciplina, sua pergunta central, o percurso dos encontros e o trabalho que será desenvolvido.

O curso não foi organizado como uma progressão de aplicativos. As ferramentas mudarão, e muitas das que hoje parecem indispensáveis poderão ser substituídas. O que desejamos construir é uma forma de investigar que permaneça útil diante de novos instrumentos: saber formular uma dúvida, examinar como uma evidência foi produzida, escolher uma representação coerente e compreender que toda representação participa de uma ação.

Quando chegarmos às demonstrações técnicas, portanto, elas não aparecerão como respostas automáticas. Cada ferramenta será colocada dentro de uma situação de conhecimento: quem a utiliza, sobre quais registros, segundo quais categorias, com que finalidade e com quais possibilidades de contestação.

## Lâmina 05 — Perguntas antes de ferramentas

A tese pedagógica do curso pode ser dita de maneira simples: começamos por perguntas, não por ferramentas. Isso não significa desprezar a técnica. Uma boa pergunta sem capacidade técnica pode permanecer impotente; uma técnica sem pergunta, porém, tende a produzir respostas para problemas que nunca foram formulados.

Em estudos urbanos, é comum começar pelo que está disponível: uma base encontrada, uma API, um mapa pronto, uma biblioteca de visualização. A disponibilidade já orienta o olhar. Passamos a enxergar a cidade segundo as colunas existentes e a confundir o que é mensurável com o que é importante. O movimento que propomos é ligeiramente diferente: reconhecer uma inquietação, perguntar que evidências poderiam colocá-la à prova e só então avaliar ferramentas e fontes.

Às vezes o caminho começa por uma base, uma imagem ou uma representação estranha. Não há problema. O essencial é permitir que o encontro com esse artefato reformule a pergunta, em vez de apenas confirmar uma narrativa escolhida de antemão.

## Lâmina 06 — Dúvida, dado, representação e ação

Esta figura é importante e retornará durante o semestre. Ela não é um ciclo e não descreve uma ordem obrigatória. Dúvida, dado, representação e ação formam uma matriz de relações. Cada elemento pode transformar todos os outros e também transformar a si próprio.

Uma dúvida orienta a busca por dados, mas um dado inesperado pode alterar completamente a dúvida. Um dado nunca chega sem representação: antes de entrar numa tabela, alguém definiu um campo, uma unidade, uma categoria ou um procedimento de medição. Uma representação pode orientar uma ação, mas a ação modifica o fenômeno e passa a produzir novos dados. Investigar também é agir: escolher observar uma ausência já reorganiza o campo de atenção.

Pense novamente na viela ausente. A dúvida pode ser: por que ela não aparece? O dado pode ser um cadastro viário, uma caminhada ou o relato dos moradores. A representação pode ser um mapa que confronte fontes. A ação pode ser corrigir uma base, reivindicar um endereço ou simplesmente reformular a pergunta. Nenhuma dessas operações acontece uma única vez. A investigação pode começar em qualquer ponto e retornar a qualquer ponto.

## Lâmina 07 — Seis encontros, seis perguntas

O percurso do curso é organizado por perguntas que se aprofundam. Começamos examinando representação e investigação. Depois perguntamos quem produz a cidade que aparece nos dados; o que muda quando fenômenos urbanos viram tabelas e mapas; como comparar, relacionar e interpretar evidências; o que a inteligência artificial acrescenta ou oculta; e, finalmente, como transformar esse processo em uma pequena investigação comunicável.

Não é necessário memorizar agora toda a programação. O importante é perceber sua direção. Sairemos da capacidade humana de representar, passaremos pelas instituições e infraestruturas que produzem dados, chegaremos às formas de visualização e aos modelos de IA, e retornaremos à responsabilidade de formular e sustentar um argumento.

As aulas combinarão exposição, leitura, discussão e pequenas operações práticas. A técnica não ficará separada da reflexão conceitual, porque cada comando técnico contém escolhas: projeção cartográfica, unidade espacial, tratamento de ausência, agrupamento, escala, cor, fonte e método de verificação.

---

# Capítulo 3 — O trabalho do semestre

## Lâmina 08 — Agora vamos falar do trabalho

Antes de entrar na questão intelectual da aula, vamos tornar o trabalho do semestre previsível. A intenção não é criar uma tarefa paralela que consuma toda a disciplina. O trabalho deve funcionar como um pequeno campo de experimentação no qual as ideias do curso ganham consequência.

Vocês não produzirão uma tese. Produzirão uma pequena investigação bem feita. “Pequena” diz respeito ao recorte; “bem feita” diz respeito à clareza da pergunta, ao cuidado com a origem dos dados, à coerência da representação e à honestidade sobre limites e decisões.

É melhor investigar uma única ausência concreta e documentar rigorosamente o percurso do que apresentar um painel grandioso cujas categorias, transformações e fontes ninguém consegue reconstruir. A qualidade não será medida pela quantidade de mapas, pelo número de linhas de código ou pela aparência tecnológica do resultado.

## Lâmina 09 — Uma pequena investigação bem feita

O trabalho será um atlas mínimo ou ensaio investigativo sobre uma questão urbana. A palavra atlas não exige uma coleção extensa de mapas. Aqui ela designa uma montagem intencional de evidências: uma pergunta, alguns registros, representações escolhidas e uma interpretação que permita ao leitor acompanhar o raciocínio.

O recorte pode ser espacialmente pequeno e intelectualmente significativo. Uma quadra, uma rua, um conjunto de nomes, uma categoria administrativa, uma mudança temporal ou um conflito entre duas fontes já podem sustentar uma boa investigação. O desafio é evitar tanto a generalidade excessiva — “explicar a desigualdade de São Paulo” — quanto o levantamento sem pergunta — “mapear todos os equipamentos porque os dados existem”.

Uma investigação pequena também precisa declarar o que não conseguiu fazer. Limites não são confissões de fracasso; são informações sobre o alcance do argumento. Ao final, queremos saber não apenas o que vocês concluíram, mas como a dúvida inicial foi transformada pelo encontro com dados, representações e possíveis ações.

## Lâmina 10 — Exemplos como portas de entrada

Os exemplos desta lâmina não formam um cardápio obrigatório. Servem para mostrar escalas e tipos de entrada possíveis. Alguém pode começar por nomes de ruas e perguntar quem é homenageado no espaço público. Outra pessoa pode investigar cursos d’água que desapareceram da paisagem visível, mas continuam orientando relevo, drenagem e enchentes. Outra pode comparar acessibilidade registrada e acessibilidade experimentada.

O importante é que o caso permita observar mediações. Se o tema for arborização, não basta mapear árvores: é preciso perguntar quem contou, o que foi considerado árvore, quando ocorreu o levantamento e que territórios receberam mais atenção. Se o tema for mobilidade, não basta baixar trajetos: é necessário entender que população produziu os registros e quais deslocamentos não deixam rastros equivalentes.

Escolha um caso porque ele produz uma dúvida relevante e manejável, não apenas porque promete uma imagem bonita. A representação final deverá ser consequência da investigação, e não o objetivo que determina antecipadamente tudo o que poderá ser visto.

## Lâmina 11 — A matriz retorna no trabalho

A matriz da investigação reaparece aqui para afastar a ansiedade de encontrar um começo perfeito. O trabalho pode começar por uma dúvida, mas também por um dado encontrado, por uma imagem que incomoda ou por uma ação já em andamento. Uma associação de moradores pode estar corrigindo endereços; essa ação produz uma pergunta. Um mapa pode mostrar um vazio; essa representação provoca a busca por outras evidências.

O que será avaliado é a capacidade de registrar as transformações. Qual era a pergunta inicial? Que dado a desestabilizou? Que escolha gráfica revelou ou ocultou uma relação? Que ação possível surgiu e que nova dúvida ela produziu? Esse diário de decisões é parte da autoria.

Evitem descrever o processo como uma sequência limpa que nunca existiu. Investigações reais possuem retornos, atalhos e impasses. O objetivo de documentá-los não é glorificar confusão, mas permitir que outra pessoa compreenda por que o trabalho chegou à forma apresentada.

## Lâmina 12 — Anatomia da entrega

A entrega terá componentes simples e reconhecíveis. Primeiro, uma pergunta formulada de modo que possa ser investigada. Depois, a identificação das fontes e de suas condições de produção. Em seguida, uma ou mais representações que façam trabalho argumentativo. Por fim, uma interpretação, os limites encontrados e uma breve documentação do processo, incluindo o uso de inteligência artificial quando houver.

Uma fonte não é apenas um endereço eletrônico. Precisamos saber instituição, data, cobertura, unidade, categorias e transformações aplicadas. Uma visualização não é apenas ilustração. Ela deve responder a uma pergunta específica e tornar sua lógica minimamente auditável. Uma interpretação não é repetição do que os números parecem dizer; é uma proposição sustentada por evidências e aberta a objeções.

Também haverá links externos e referências que permitam ao leitor continuar a investigação. O trabalho deve funcionar como objeto público de conhecimento, não como resposta cifrada destinada apenas à avaliação do professor.

## Lâmina 13 — Duas trilhas, mesma exigência intelectual

O curso acolhe pessoas com diferentes repertórios técnicos. Por isso, o trabalho poderá seguir trilhas distintas. Uma investigação pode usar ferramentas visuais, planilhas, plataformas cartográficas e operações de baixa programação. Outra pode envolver código, automação, APIs ou modelos mais complexos. A diferença está nos meios, não na exigência intelectual.

Código não compensa pergunta fraca. Uma solução tecnicamente simples não é inferior se suas escolhas forem pertinentes e bem justificadas. Da mesma forma, quem usar automação precisará explicar transformações, dependências e formas de verificação, em vez de apresentar o resultado como caixa-preta.

Os apoios serão adaptados ao ponto de partida de cada pessoa ou grupo. O objetivo comum é produzir uma investigação que outra pessoa consiga seguir: reconhecer a dúvida, localizar a evidência, compreender a representação, avaliar a interpretação e identificar as decisões humanas envolvidas.

## Lâmina 14 — Avaliação, autoria e uso de IA

A inteligência artificial pode participar do trabalho, mas seu uso precisa permanecer visível. Não trataremos autoria como ausência de ferramentas; autoria é a responsabilidade pelas escolhas, verificações e consequências do que foi produzido. Uma pessoa pode escrever cada frase sozinha e ainda assim repetir fontes sem compreendê-las. Outra pode usar um modelo para explorar hipóteses e manter rigorosamente a responsabilidade sobre o resultado.

Documentem os usos relevantes: para que o modelo foi acionado, que material recebeu, que resposta produziu, como foi verificada e que decisão coube ao grupo. Não é necessário anexar conversas intermináveis. É preciso tornar reconstruíveis as operações que afetaram o argumento.

A avaliação observará coerência entre pergunta, evidência, representação e interpretação; qualidade da documentação; capacidade de reconhecer limites; e responsabilidade no uso de ferramentas. Fluência verbal ou acabamento visual não substituirão a verificação.

## Lâmina 15 — Agora começa a pergunta fundadora

O curso e o trabalho estão apresentados. Podemos entrar na pergunta intelectual que sustenta todo o percurso: o que significa representar e por que essa capacidade é tão decisiva para pensar cidades, dados e inteligência artificial?

Até aqui usamos palavras como mapa, tabela, imagem, modelo e evidência. Todas elas envolvem algum tipo de substituição. Algo que não está presente — uma rua distante, uma população, um acontecimento passado, uma situação futura — torna-se manipulável por meio de outra coisa. Essa operação parece tão cotidiana que frequentemente esquecemos sua estranheza.

O próximo bloco desacelera esse gesto. Antes de perguntar se uma representação é boa, verdadeira ou bonita, perguntaremos o que ela torna possível, o que precisa retirar do mundo e que tipo de ação passa a autorizar.

---

# Capítulo 4 — Representar: tornar presente, reduzir e agir

## Lâmina 16 — O que a representação torna possível?

Representar é uma capacidade humana fundadora. Por meio de marcas, gestos, imagens, palavras, números e modelos, podemos nos relacionar com aquilo que não está diante de nós. Evocamos ausências, coordenamos ações entre pessoas, conservamos experiências, imaginamos futuros e construímos objetos que ainda não existem.

Uma planta permite discutir um edifício antes de construí-lo. Um mapa permite organizar uma viagem por um território que não vemos integralmente. Uma tabela permite comparar acontecimentos separados no espaço e no tempo. Uma narrativa permite partilhar uma experiência sem reproduzi-la materialmente.

Mas cada ganho depende de uma diferença. A planta não é o edifício; o mapa não é o território; a tabela não é a população; a narrativa não é a experiência. Se esquecemos essa diferença, a representação ganha uma autoridade que não pode sustentar. Se recusamos toda representação por ser incompleta, perdemos a capacidade de conhecer e agir coletivamente. A questão será habitar essa tensão.

## Lâmina 17 — Evocar o ausente e imaginar o inexistente

A representação não se limita a copiar coisas existentes. Ela também produz relações com o passado, o futuro e o possível. Podemos desenhar uma cidade que ainda não existe, simular uma inundação futura, reconstruir uma paisagem desaparecida ou elaborar um cenário alternativo.

Isso tem importância política e projetual. Quem consegue representar um futuro torna esse futuro discutível, financiável e, às vezes, realizável. Um render imobiliário não é apenas uma imagem bonita: organiza expectativas, valores e decisões. Um mapa de risco não apenas descreve; influencia prioridades, seguros, obras e deslocamentos. Uma categoria estatística pode fazer uma população aparecer como sujeito de política pública.

Ao mesmo tempo, imaginar não é produzir livremente. Toda representação possível utiliza convenções, técnicas e repertórios existentes. Perguntar quem domina essas linguagens e quais futuros conseguem ganhar forma será parte da análise.

## Lâmina 18 — Uma definição operacional

Para esta aula, usaremos uma definição de trabalho: representar é tornar algo presente por meio de outra coisa. Essa é uma síntese didática do curso, não uma citação literal de um único autor. Ela será desdobrada em quatro operações.

Primeiro, substituir: algo ausente pode ser evocado. Segundo, selecionar: nem tudo cabe ou importa igualmente. Terceiro, relacionar: elementos ganham sentido por sua posição e associação. Quarto, agir: a representação orienta decisões.

Uma planta de emergência mostra bem o conjunto. Ela não copia o edifício; substitui a experiência espacial. Elimina textura, decoração e muitos objetos; seleciona saídas, rotas e riscos. Relaciona a posição do observador com um percurso possível. Finalmente, orienta uma ação urgente. Sua redução é parte de sua eficácia.

Mas podemos perguntar: ela considera pessoas com mobilidade reduzida? As portas representadas permanecem abertas? A fumaça altera a legibilidade? A definição operacional não encerra a crítica; ela oferece um vocabulário para localizar decisões.

## Lâmina 19 — Stuart Hall: representar produz sentido

Stuart Hall foi um intelectual jamaicano-britânico e uma figura central dos estudos culturais. Seus trabalhos atravessam mídia, raça, identidade, diáspora e poder. Aqui ele nos ajuda a abandonar uma compreensão excessivamente simples da representação como espelho.

Para Hall, representar não é apenas colocar em circulação o significado já pronto de uma coisa. Linguagens, imagens, categorias e práticas participam da produção social do sentido. Uma praça materialmente idêntica pode ser representada como patrimônio, espaço degradado, oportunidade imobiliária, lugar de memória ou área perigosa. Essas descrições não criam arbitrariamente a praça, mas selecionam relações e legitimam ações diferentes.

Isso não significa que tudo seja apenas narrativa. Significados são disputados em condições materiais e institucionais desiguais. Algumas representações recebem a autoridade do Estado, da ciência ou da mídia; outras lutam para serem reconhecidas. A pergunta passa a ser: como um sentido se torna disponível, convincente e acionável?

## Lâmina 20 — Magritte e Borges: a representação precisa diferir

À esquerda encontramos uma referência a René Magritte, pintor surrealista belga, e à obra *A traição das imagens*, de 1929. Nela, a imagem de um cachimbo é acompanhada pela frase “Isto não é um cachimbo”. A provocação é precisa: podemos reconhecer o cachimbo, mas não podemos enchê-lo de tabaco ou fumá-lo. A imagem representa um objeto e simultaneamente declara a distância que os separa.

À direita aparece Jorge Luis Borges e o texto breve “Do rigor na ciência”. Borges imagina um império cujos cartógrafos produzem um mapa na escala de um para um. O mapa coincide com o território e perde justamente aquilo que o tornaria útil: a redução.

Juntos, os dois artefatos formulam uma tensão. Magritte lembra que a imagem não é a coisa. Borges mostra que uma representação precisa deixar de ser a coisa para funcionar. A questão não é eliminar a perda, mas compreender o que foi perdido e por quê.

## Lâmina 21 — Brunelleschi e a perspectiva como operação

A história da perspectiva linear costuma ser narrada de forma heroica, como se Filippo Brunelleschi a tivesse inventado sozinho em Florença. É mais seguro dizer que suas demonstrações, no início do século XV, foram um marco em sua operacionalização; Leon Battista Alberti posteriormente sistematizou o método.

No famoso experimento associado ao Batistério de Florença, um painel pintado, um pequeno orifício e um espelho permitiam comparar imagem e edifício a partir de uma posição controlada. O ponto de vista deixa de ser mera circunstância e torna-se regra geométrica. O observador precisa ocupar um lugar específico para que o sistema funcione.

Essa representação transforma a arquitetura. Permite antecipar, comparar, verificar e coordenar algo ainda inexistente. Mas também naturaliza um observador imóvel e monocular. Toda técnica de visão produz capacidades e estabelece condições: quem olha, de onde olha e o que precisa permanecer fora do quadro.

## Lâmina 22 — Zaha Hadid e Frank Gehry: representar para construir

Com Zaha Hadid e Frank Gehry, a representação não apenas descreve o edifício: ela participa de sua invenção e fabricação. Hadid utilizou pintura, distorção e perspectivas múltiplas como instrumentos de investigação espacial. Seus desenhos não eram ilustrações tardias de uma solução definida; exploravam relações que a planta e a perspectiva convencionais dificilmente acomodavam.

Gehry combinou croquis, modelos físicos e sistemas digitais como o CATIA para descrever e fabricar geometrias complexas. O Guggenheim de Bilbao não é simplesmente uma forma imaginada pelo computador. Ele resulta da circulação entre gesto, maquete, cálculo, detalhamento, indústria e canteiro.

A questão que importa para o curso é esta: quando uma representação começa a produzir aquilo que representa? E quando passamos a acreditar mais na fluência do render do que na experiência futura do edifício? A potência projetual e o risco de sedução nascem da mesma capacidade de antecipar.

## Lâmina 23 — Perder mundo, ganhar capacidade

Podemos condensar o bloco em uma tensão: toda representação perde mundo e ganha capacidade de ação. Essa frase é uma síntese do curso, não uma lei atribuída a um autor. Ela serve para impedir dois extremos.

No primeiro, exigimos uma representação completa e esquecemos que sua utilidade depende de selecionar. No segundo, aceitamos qualquer redução como inevitável e deixamos de perguntar quem escolheu, com qual finalidade e com quais consequências.

Uma boa representação não é necessariamente aquela que contém mais informação. É aquela cuja redução é adequada à pergunta, cujos critérios podem ser examinados e cujos limites não são confundidos com limites do próprio mundo. A partir daqui mudaremos de escala. Um cachimbo ou um edifício ainda podem ser relativamente isolados. Uma cidade reage ao modo como separamos suas partes.

---

# Capítulo 5 — A cidade como problema de complexidade

## Lâmina 24 — Mas uma cidade não é um cachimbo

Um cachimbo pode ser isolado para ser representado. Na cidade, moradia, trabalho, cuidado, mobilidade e memória se sobrepõem. Quando isolamos uma parte, podemos alterar o fenômeno que desejamos compreender.

Uma rua é simultaneamente endereço, rota, espaço de encontro, infraestrutura de drenagem, frente comercial, memória e objeto de disputa. Desenhá-la apenas como eixo viário produz uma representação válida para algumas operações, mas não uma definição completa do que ela é.

Os círculos sobrepostos da lâmina não são um modelo final da cidade. Eles preparam uma pergunta: como representar algo cujos elementos pertencem simultaneamente a muitos sistemas? Acrescentar camadas pode não bastar se continuarmos tratando cada camada como realidade independente. Precisamos observar as relações que fazem com que uma mudança na mobilidade transforme comércio, cuidado, valor da terra e vida cotidiana.

## Lâmina 25 — Christopher Alexander: árvore e semirretículo

Christopher Alexander foi arquiteto e teórico do design, professor em Berkeley. No artigo “A City Is Not a Tree”, publicado em 1965, ele usa árvore e semirretículo como estruturas lógicas.

Na árvore, conjuntos estão separados ou inteiramente contidos em outros conjuntos. É uma estrutura fácil de desenhar, administrar e compreender. No semirretículo, os conjuntos se sobrepõem: o mesmo elemento participa de diversos sistemas. É mais próximo da vida urbana, mas muito mais difícil de apreender de uma só vez.

Alexander observa que, em um único ato mental, tendemos a visualizar uma árvore. Isso explica por que planos e diagramas reduzem sobreposições a hierarquias funcionais. Sua crítica não significa que toda cidade planejada fracassa ou que toda formação espontânea funciona. O valor do texto está em mostrar que nossa capacidade de representar pode empobrecer precisamente as relações que sustentam a urbanidade.

## Lâmina 26 — O problema cognitivo

Na lâmina, a mesma rua participa de cadastro, mobilidade, cotidiano, economia, ambiente e política. Não são apenas seis descrições colocadas lado a lado. Cada relação modifica as demais. Uma alteração no transporte muda fluxos de pedestres; os fluxos alteram comércio; o comércio modifica encontros e preços; pavimentação e drenagem reorganizam usos e riscos.

O problema cognitivo não se resolve simplesmente adicionando mais categorias. Podemos criar dezenas de camadas e continuar incapazes de representar suas interdependências. A simplificação é inevitável para pensar e agir, mas ela precisa ser tratada como operação provisória.

A passagem para Jane Jacobs acontece aqui. Alexander mostra por que tendemos a organizar a cidade como árvore. Jacobs mostrará que as interações difíceis de isolar não são ruído a ser eliminado. Elas constituem o tipo específico de problema que uma cidade apresenta.

## Lâmina 27 — Milton Santos: o espaço como instância social ativa

Milton Santos foi geógrafo brasileiro, professor emérito da Universidade de São Paulo e vencedor do Prêmio Vautrin Lud, uma das principais distinções internacionais da geografia. Sua presença aqui não funciona apenas como contraponto nacional aos autores europeus e anglo-saxões. Ele modifica a própria maneira como estamos definindo o espaço.

Em *A natureza do espaço*, publicado em 1996, Santos pensa o espaço como conjunto indissociável de sistemas de objetos e sistemas de ações. Ruas, edifícios, redes e máquinas não constituem um cenário neutro no qual a sociedade acontece. Eles condicionam ações e são continuamente apropriados, valorizados e transformados por elas.

Isso permite avançar em relação a Alexander. Não basta representar corretamente sobreposições entre objetos urbanos. Precisamos perguntar que ações produzem essas relações e como técnica, tempo e poder participam da organização espacial. Pensar o espaço a partir do Brasil também significa produzir categorias capazes de reconhecer desigualdades, dependências e experiências periféricas que teorias universalizantes frequentemente tratam como exceção.

## Lâmina 28 — Sistemas de objetos e sistemas de ações

Na parte azul estão rua, calçada, ônibus, edifício, fibra e sensor. Na parte vermelha aparecem circular, cuidar, trabalhar, regular, mapear e resistir. As linhas indicam que não existe correspondência simples de um para um.

Uma rua suporta circulação, comércio, cuidado, conflito e memória. As ações também transformam sua função e seu valor. Um edifício pode ser moradia, investimento, ocupação, patrimônio ou obstáculo. O sensor não apenas registra o território: sua instalação modifica práticas, expectativas e formas de vigilância.

A contribuição de Milton Santos para o curso pode ser condensada numa pergunta: os dados urbanos registram objetos com facilidade, mas como representar as ações que produzem, usam e transformam esses objetos? Quando uma base conta equipamentos, lotes e vias, precisamos procurar usos, normas, temporalidades e disputas. O espaço não é apenas forma representada; é forma sendo continuamente praticada.

## Lâmina 29 — Jane Jacobs e a complexidade organizada

Jane Jacobs foi jornalista, escritora e ativista urbana, nascida nos Estados Unidos e depois radicada no Canadá. Sua crítica ao urbanismo modernizador foi construída pela observação da vida cotidiana e pela resistência a grandes operações de renovação.

No capítulo “The Kind of Problem a City Is”, de *Morte e vida de grandes cidades*, Jacobs afirma: “Cities happen to be problems in organized complexity.” Cidades são problemas de complexidade organizada. Muitas variáveis heterogêneas interagem de maneiras reconhecíveis, mas não podem ser isoladas sem perda importante.

Diversidade de usos, horários, edifícios, pessoas e escalas pode produzir ordem sem desenho central único. O mapa sinóptico tende a ver separação onde a rua produz relação. Jacobs não nos pede que abandonemos dados ou planejamento; pede que métodos se tornem capazes de aprender com processos urbanos reais, em vez de obrigar a realidade a obedecer ao esquema.

## Lâmina 30 — Warren Weaver: três tipos de problema

Warren Weaver foi matemático e administrador científico norte-americano. Em “Science and Complexity”, de 1948, distinguiu problemas de simplicidade, de complexidade desorganizada e de complexidade organizada.

Problemas de simplicidade envolvem poucas variáveis e relações relativamente isoláveis. Na complexidade desorganizada, um grande número de elementos pode ser tratado estatisticamente, como comportamento médio de partículas. A complexidade organizada combina muitas variáveis interdependentes sem que o conjunto se torne puramente aleatório.

Jacobs toma esse vocabulário para dizer que a cidade exige métodos atentos a relações organizadas, não apenas médias ou cadeias monocausais. A classificação de Weaver é histórica e heurística; não precisamos transformá-la em taxonomia eterna. Sua importância aqui é oferecer uma genealogia para a pergunta: como estudar sistemas nos quais muitas coisas importam simultaneamente e as interações produzem efeitos que nenhuma variável isolada explica?

## Lâmina 31 — Edgar Morin: distinguir sem separar

Edgar Morin é filósofo e sociólogo francês, conhecido por desenvolver o pensamento complexo. Sua contribuição impede que a palavra complexidade se torne sinônimo de confusão, totalidade impossível ou desculpa para não decidir.

Pensar de maneira complexa não significa colocar tudo em um modelo gigantesco. Significa distinguir sem separar definitivamente e relacionar sem apagar diferenças. Também significa reconhecer incerteza, retroações e o fato de que o observador participa da produção do conhecimento.

Se analisamos enchentes, podemos distinguir chuva, impermeabilização, relevo, drenagem, ocupação, manutenção e desigualdade. O erro seria tratá-los como causas independentes ou imaginar que uma explicação precisa incorporar literalmente cada detalhe da cidade. A complexidade exige recortes conscientes, relações justificadas e disposição para revisar o modelo quando seus efeitos retornam ao sistema.

## Lâmina 32 — Quatro pistas para representar complexidade

Esta síntese reúne quatro pistas: relações, escalas, temporalidades e emergência. Relações lembram que elementos ganham propriedades pelo modo como se conectam. Escalas mostram que um padrão visível na quadra pode desaparecer no município, ou o contrário. Temporalidades impedem que um retrato momentâneo pareça estrutura permanente. Emergência nomeia efeitos do conjunto que não estavam contidos em um elemento isolado.

Essas pistas não formam um método automático. Funcionam como perguntas para qualquer representação urbana. Que relações foram preservadas? Em qual escala o padrão aparece? Que duração foi condensada? O resultado é soma de partes ou efeito de interação?

Agora faremos uma mudança importante. Até aqui falamos da cidade como fenômeno complexo. Para transformá-la em dado, precisamos classificar. Classificar torna possível comparar e agir, mas traça fronteiras conceituais dentro de uma realidade sobreposta.

---

# Capítulo 6 — Classificação e *capta*: como algo vira dado

## Lâmina 33 — Classificar é traçar uma fronteira

Imagine um caminho estreito entre casas. Ele deve entrar na rede viária? Para responder, diferentes instituições podem usar largura, acesso, uso, domínio, circulação ou existência legal. O mesmo espaço pode tornar-se rua, viela, passagem ou acesso.

A categoria produz efeitos. Pode permitir rota, endereço, serviço e reconhecimento; também pode gerar invisibilidade. O objetivo não é descobrir a palavra essencial que o espaço sempre carregou. É tornar explícito que uma classificação foi definida para uma finalidade.

Moradores, Correios, bombeiros, cadastro municipal, aplicativo de rotas e Censo podem classificar a mesma passagem de maneiras diferentes. Cada classificação preserva certas propriedades e perde outras. Uma categoria responsável precisa declarar critérios, casos limítrofes, possibilidade de revisão e consequências para quem será organizado por ela.

## Lâmina 34 — Bowker e Star: classificações são infraestrutura

Geoffrey Bowker é historiador da ciência, tecnologia e informação. Susan Leigh Star foi socióloga da ciência e da tecnologia, conhecida por seus estudos sobre classificação, padrões, infraestrutura e trabalho invisível. Em *Sorting Things Out*, eles mostram que sistemas classificatórios coordenam o mundo e desaparecem da atenção quando funcionam.

Uma categoria parece apenas uma coluna numa base, mas pode organizar formulários, profissionais, recursos e trajetórias de vida. O que não cabe pode virar “outros”, erro, nulo ou inexistência administrativa. A padronização facilita comparação e cooperação; ao mesmo tempo, distribui custos e benefícios.

A conclusão não é que toda classificação seja violência e deva ser abandonada. Sem categorias, muitas ações coletivas se tornam impossíveis. A tarefa é reconhecer que padrões valorizam pontos de vista, requerem manutenção e precisam oferecer formas de contestação.

## Lâmina 35 — Categorias construídas podem revelar padrões reais

Dizer que uma categoria foi construída não significa dizer que o fenômeno seja imaginário. Feminicídio é um exemplo forte. A categoria geral “homicídio” agrega mortes com relações e motivações diferentes. Nomear a violência de gênero torna recorrências, responsabilidades e condições sociais mais legíveis.

No campo urbano, o IBGE precisa construir uma definição operacional para contar população em situação de rua, justamente porque a unidade convencional do Censo é o domicílio. Período, locais e situações de permanência decidem quem entra no levantamento. A mudança de “aglomerados subnormais” para “favelas e comunidades urbanas” também reorganiza reconhecimento, comparação e relação institucional.

A pergunta não é “inventado ou verdadeiro?”. Perguntamos: que fenômeno a categoria permite perceber, que limite estabelece, quem participa da definição e que ações ela torna possíveis?

## Lâmina 36 — Atividade: abrir a caixa da categoria

Esta atividade propõe que escolhamos uma categoria urbana e a tratemos como objeto de investigação. Pode ser imóvel vago, área de risco, pessoa em situação de rua, favela, rua, árvore ou ocorrência de violência.

Primeiro, localizamos a definição. Depois procuramos critérios e casos limítrofes. Em seguida perguntamos quem é afetado quando a categoria é aplicada. Finalmente, imaginamos como ela poderia ser revisada ou contestada.

O exercício não exige resolver o problema em poucos minutos. Seu objetivo é substituir a leitura automática da coluna por uma leitura infraestrutural. Toda vez que encontrarmos um campo numa base, tentaremos enxergar o trabalho anterior que o estabilizou: reuniões, leis, manuais, formulários, sistemas, treinamento e decisões sobre exceções. O dado começa antes da planilha.

## Lâmina 37 — Johanna Drucker e a passagem de *data* a *capta*

Johanna Drucker é artista, escritora, historiadora do livro e pesquisadora das humanidades digitais. Essa combinação importa porque ela pensa forma gráfica e conhecimento interpretativo de maneira inseparável.

No artigo “Humanities Approaches to Graphical Display”, de 2011, Drucker propõe deslocar a ideia de *data*, aquilo que seria dado, para *capta*, aquilo que foi tomado. Sua frase curta é: “Data are capta, taken not given.” Dados são *capta*: tomados, não simplesmente dados.

Isso não torna a palavra “dados” proibida. Funciona como lembrete epistemológico. Observar, selecionar, medir, classificar e registrar são operações constitutivas. Uma visualização não recebe matéria neutra e apenas lhe dá aparência; ela continua a cadeia de interpretação iniciada muito antes.

## Lâmina 38 — A categoria já interpreta

Os dois diagramas vêm do artigo de Drucker, com desenho gráfico de Xárene Eskandar. À esquerda, um gráfico de barras convencional compara categorias masculinas e femininas entre unidades nacionais. A forma sugere classes estáveis, medidas homogêneas e fronteiras nítidas.

À direita, a alternativa gráfica perturba a estabilidade das barras. Sobreposições, extensões e densidades tornam visível que gênero, população e pertencimento nacional não são recipientes perfeitamente separados.

Drucker não está oferecendo um novo padrão universal de gráfico. Ela realiza uma provocação: se nossas categorias são interpretativas, por que a forma gráfica deveria apresentá-las como entidades naturais? A ambiguidade não precisa ser escondida como defeito. Em certos problemas, ela é informação substantiva. A representação pode expressar a qualidade epistemológica do que foi capturado.

## Lâmina 39 — Uma data pode esconder um processo

À esquerda, publicações são contadas por ano. É uma visualização perfeitamente útil para certas perguntas. Mas “data de publicação” condensa uma sequência: escrita, aquisição, edição, preparação, impressão, lançamento e circulação.

À direita, Drucker redesenha a temporalidade para mostrar esses processos. O objetivo não é declarar falso o ponto anual, mas perguntar o que acontece quando um evento processual é tratado como instante. Nas cidades fazemos isso frequentemente: data de inauguração, data de ocupação, ano de construção, momento da ocorrência.

Cada ponto pode esconder durações, antecipações e atrasos. Se a pergunta é contar lançamentos, a simplificação funciona. Se desejamos compreender produção cultural ou transformação urbana, talvez precisemos representar ritmos e etapas. Todo eixo temporal contém uma teoria sobre o que conta como acontecimento.

## Lâmina 40 — Experiência não cabe numa régua neutra

Os diagramas seguintes investigam afeto e experiência. Num gráfico convencional, estados subjetivos são posicionados sobre uma métrica temporal estável. A régua permanece neutra e a experiência torna-se valor.

Na alternativa, atividades e intensidades dão forma ao próprio dia. Certos períodos se expandem, outros se comprimem. Drucker sugere que, para questões humanísticas, talvez a métrica deva carregar marcas da experiência em vez de fingir exterioridade completa.

Isso interessa à cidade. Cinco minutos esperando em situação de risco não equivalem necessariamente a cinco minutos dentro de um veículo confortável. Dois trajetos de mesma distância podem possuir dificuldades radicalmente diferentes. Não precisamos abandonar medidas convencionais, mas podemos confrontá-las com representações capazes de expressar ritmo, expectativa, memória e desigualdade vivida.

## Lâmina 41 — Do espaço para a espacialidade

Aqui o espaço deixa de aparecer como recipiente neutro. Num diagrama, o acontecimento do naufrágio deforma a grade; no outro, a experiência do percurso reorganiza o terreno. Drucker distingue implicitamente coordenadas abstratas de espacialidade vivida.

Um mapa métrico pode representar com precisão a distância entre dois pontos e continuar insuficiente para descrever barreiras, familiaridade, medo, esforço ou pertencimento. Isso não invalida coordenadas. Mostra que a pergunta determina o tipo de espaço relevante.

Em urbanismo, frequentemente tratamos proximidade geométrica como acesso. Um equipamento a quinhentos metros pode estar separado por uma via hostil, declive, horário, tarifa ou fronteira social. A contribuição de Drucker é gráfica e epistemológica: deixar que relações experimentadas pressionem a forma da representação.

## Lâmina 42 — Todo mapa responde a uma pergunta

À esquerda aparece o célebre mapa de John Snow sobre a epidemia de cólera em Londres. Marcas de mortes e localização de bombas d’água ajudaram a relacionar casos à Broad Street. O mapa tornou um padrão espacial legível e apoiou uma intervenção.

À direita, Drucker reinscreve pessoas sobre o espaço. Não pretende corrigir Snow para a mesma pergunta. Mostra que uma representação poderosa para localizar mortes e uma bomba não responde automaticamente a questões sobre vidas, experiências, famílias e desigualdades.

Uma visualização deve ser julgada em relação à pergunta que sustenta. O perigo surge quando uma resposta eficaz passa a funcionar como imagem total do fenômeno. O mapa de Snow é exemplar não porque contém tudo, mas porque seleciona relações pertinentes. Outras perguntas exigem outras inscrições.

## Lâmina 43 — Limite cartográfico e fronteira do fenômeno

Uma linha administrativa pode ser juridicamente exata. Isso não significa que desigualdade, paisagem, pertencimento, circulação ou risco terminem exatamente nela. A precisão da linha pertence à decisão legal; não necessariamente ao fenômeno que desejamos investigar.

Na lâmina, círculos atravessam a divisão entre dois municípios. Podemos imaginar uma bacia hidrográfica, uma mancha de poluição, uma rede de trabalho ou uma continuidade urbana. O mapa precisa cortar o papel, mas o pesquisador deve perguntar se o corte também existe no objeto.

Esta distinção evita dizer vagamente que “linhas escondem fontes”. A linha representa um limite definido segundo regras. O problema ocorre quando sua exatidão visual transfere aparência de exatidão para fenômenos porosos. Pergunte sempre: qual linha é exata e qual realidade ela faz parecer exata?

## Lâmina 44 — Exercício guiado com uma base pública

Na primeira aula, não faz sentido abandonar cada aluno diante de milhares de tabelas. O professor traz uma base pequena e preparada, como uma camada de favelas e comunidades urbanas ou uma tabela territorial do IBGE.

Primeiro localizamos instituição, data e finalidade. Depois lemos unidade, campos e categorias. Em seguida perguntamos o que precisou ser definido para que os registros existissem. Finalmente, renomeamos honestamente a base: não “as favelas de São Paulo”, mas “registros produzidos por determinada instituição, segundo determinados critérios, numa data e para uma finalidade”.

Essa frase mais longa não serve para paralisar a análise. Serve para lembrar que a tabela é uma inscrição situada. Depois desse reconhecimento, podemos utilizá-la com mais precisão e procurar fontes complementares para aquilo que ela não foi criada para responder.

---

# Capítulo 7 — Mapas, dados e poder

## Lâmina 45 — Agora falaremos de mapas, dados e poder

Até aqui examinamos representação, complexidade, classificação e *capta*. Agora concentraremos essas questões na cartografia e na produção de legibilidade pública.

Esta não será ainda a aula completa sobre política dos mapas. O objetivo é estabelecer um vocabulário que retornará nos encontros seguintes: seleção, nomeação, hierarquia, autoridade, silêncio e possibilidade de contestação.

Mapas não são politizados apenas quando contêm propaganda evidente. Toda cartografia depende de instituições, convenções e finalidades. Isso não torna cada mapa uma mentira. Reduzir e selecionar são condições de sua existência; mentir implica uma intenção adicional de enganar. Queremos desenvolver uma crítica capaz de reconhecer simultaneamente utilidade técnica e posição política.

## Lâmina 46 — Teresa Caldeira: Cidade de muros

Teresa Pires do Rio Caldeira é antropóloga brasileira e professora de planejamento urbano em Berkeley. Seus trabalhos examinam segregação, cidadania, violência, espaço público e formas de urbanização nas periferias do Sul Global. Em *Cidade de muros*, ela analisa como crime, medo, violência policial, privatização da segurança e enclaves fortificados reorganizaram São Paulo.

Sua contribuição permite retornar à imagem de Paraisópolis sem reduzi-la a contraste visual entre pobreza e riqueza. Muros não apenas separam propriedades. Eles organizam acesso, circulação, vigilância e pertencimento. Condomínios, centros empresariais e espaços de consumo podem aproximar fisicamente grupos sociais enquanto aprofundam distâncias políticas e cotidianas.

Caldeira mostra que segregação urbana não é apenas distribuição de renda no território. É produção desigual de cidadania: algumas pessoas circulam protegidas por dispositivos privados, enquanto outras encontram suspeição e violência. O espaço construído participa ativamente dessa distribuição.

## Lâmina 47 — Perto no mapa, separado na experiência

No mapa, dois lugares podem ser vizinhos. Na experiência, muros, portarias, câmeras, medo e regimes privados de segurança produzem distâncias profundas. A lâmina organiza quatro operações: muro, medo, enclave e cidadania.

O muro separa e controla acessos. O medo ajuda a legitimar vigilância, retraimento e respostas violentas. O enclave privatiza segurança, circulação, lazer e serviços. A cidadania passa a distribuir proteção e suspeição de maneira desigual.

Essa é a ponte para mapas e poder. A cartografia consegue medir distância e mostrar vizinhança, mas pode não expressar os dispositivos sociais que transformam proximidade em segregação. Quando voltamos a Paraisópolis, perguntamos não apenas o que aparece no mapa, mas quem circula como cidadão, quem circula como trabalhador tolerado e quem circula como suspeito.

## Lâmina 48 — O mapa produz legibilidade

Um mapa seleciona o que aparecerá, nomeia elementos, estabelece hierarquias visuais e recebe autoridade de convenções e instituições. Uma linha mais espessa, uma cor dominante, um topônimo ou uma ausência orientam a leitura antes que qualquer argumento seja verbalizado.

Produzir legibilidade é uma capacidade pública importante. Mapas permitem coordenar redes, distribuir serviços, reconhecer territórios e discutir decisões. Mas aquilo que se torna legível para uma finalidade pode permanecer ilegível para outra.

Uma rede oficial de ruas facilita endereçamento e emergência; pode ignorar percursos praticados. Um zoneamento organiza direitos de uso; pode representar como homogêneo um território socialmente diverso. O mapa não apenas transporta fatos. Ele organiza relações entre evidência, instituição e ação. Por isso precisamos saber quem o fez, para quem e segundo quais regras.

## Lâmina 49 — J. B. Harley: cartografia como discurso social

J. B. Harley foi historiador britânico da cartografia. Seu trabalho ajudou a deslocar a história dos mapas de uma narrativa exclusivamente técnica, na qual representações progridem rumo a maior precisão, para uma análise de discurso, instituição e poder.

No artigo “Deconstructing the Map”, Harley aproxima cartografia de autores como Foucault e Derrida. A autoridade do mapa não depende apenas de sua geometria. Ela é construída por convenções, patrocínio, instituições e silêncios. Certas presenças são enfatizadas; outras se tornam marginais ou desaparecem.

Isso não significa que Harley prove que mapas são falsos. Ele mostra que a verdade cartográfica é produzida dentro de regras sociais e técnicas. Ler criticamente um mapa inclui examinar tanto o que ele mostra quanto as condições que o autorizam a falar.

## Lâmina 50 — Quatro movimentos para desconstruir um mapa

Podemos transformar Harley em quatro movimentos de leitura. Primeiro, ler o mapa como texto: símbolos, convenções e retórica constroem uma versão do mundo. Segundo, localizar a autoridade: Estado, ciência, empresa ou comunidade conferem legitimidade à imagem.

Terceiro, procurar silêncios. Seleção, centro, escala, nome e ausência distribuem visibilidade. Quarto, relacionar mapa e poder. A cartografia descreve territórios e também ajuda a administrá-los, ocupá-los, protegê-los ou contestá-los.

Desconstruir não é destruir nem abandonar o mapa. É expor as condições que permitem que ele funcione. A pergunta-cola pode acompanhar qualquer cartografia: quem fez, para quem, com quais convenções e o que ficou fora? Depois acrescentamos: essa ausência é limitação reconhecida, decisão pertinente ou mecanismo de poder?

## Lâmina 51 — Um protocolo de leitura cartográfica

Ao encontrar um mapa, comece pela ficha básica: autoria, instituição, data, fonte, escala, projeção e finalidade. Depois observe unidades, categorias, símbolos e hierarquia visual. Pergunte que transformações ocorreram: agregação, generalização, interpolação, recorte ou normalização.

Em seguida procure ausências relevantes. Nem toda ausência é erro; um mapa precisa selecionar. O ponto é avaliar se aquilo que ficou fora altera o argumento que o mapa parece sustentar. Por fim, identifique as ações que a representação convida: comparação, vigilância, investimento, proteção, deslocamento, curiosidade ou medo.

Este protocolo evita duas leituras pobres: acreditar automaticamente porque “está no mapa” ou rejeitar automaticamente porque “todo mapa é político”. A crítica rigorosa precisa dizer como uma escolha específica modifica uma interpretação específica.

## Lâmina 52 — Oficial e praticado

A cidade oficial e a cidade praticada não são duas realidades totalmente separadas. São modos distintos de produzir evidência. Um cadastro municipal registra entidades segundo responsabilidades legais e administrativas. Um mapa colaborativo ou levantamento de campo pode registrar percursos, nomes e usos reconhecidos localmente.

Nenhuma fonte é automaticamente superior. O cadastro pode oferecer continuidade, padronização e responsabilidade institucional; pode também demorar a reconhecer mudanças. O conhecimento praticado pode revelar situações invisíveis; pode possuir cobertura irregular ou depender de relações locais difíceis de generalizar.

Uma investigação interessante surge justamente da comparação. Onde as fontes coincidem? Onde divergem? A divergência indica erro, diferença temporal, finalidade distinta ou conflito sobre o que existe? Em vez de fundir tudo imediatamente, podemos representar a tensão e transformá-la em objeto de análise.

## Lâmina 53 — Um dado é uma inscrição produzida

Esta lâmina acompanha uma cadeia: fenômeno, formulário, tabela e mapa. Uma rua é vivida; alguém escolhe campos para descrevê-la; o registro vira linha; uma consulta espacializa os resultados. Em cada passagem, algumas propriedades tornam-se manipuláveis e outras desaparecem.

A ausência também recebe forma. Pode virar zero, nulo, “outros” ou nada. Esses estados não são equivalentes. Zero afirma quantidade inexistente; nulo pode indicar valor desconhecido; “outros” reúne diferenças; campo vazio pode resultar de falha, inaplicabilidade ou não coleta.

Antes de interpretar um padrão, precisamos conhecer essa cadeia de produção: origem, unidade, data, transformação e incerteza. A tabela não é um estágio transparente entre cidade e mapa. Ela é uma tecnologia de inscrição que prepara certas perguntas e dificulta outras.

## Lâmina 54 — James C. Scott: capacidade e cegueira

James C. Scott foi cientista político e antropólogo norte-americano. Em *Seeing Like a State*, estudou como Estados tornam sociedades e territórios legíveis por meio de nomes padronizados, cadastros, mapas, medidas e classificações.

Sua formulação central para esta aula é: tornar um território legível produz capacidade e cegueira. O Estado precisa simplificar para tributar, planejar, instalar redes e reconhecer direitos. O problema começa quando o esquema administrativo deixa de ser instrumento parcial e passa a substituir conhecimentos locais e relações que não cabem nele.

Scott não é simplesmente contra planejamento. Seus casos investigam fracassos de grandes projetos quando legibilidade estatal, poder concentrado e confiança modernizadora se combinam com a desvalorização do conhecimento prático. A pergunta é: que simplificação é necessária e que mecanismo permite corrigi-la?

## Lâmina 55 — Scott aplicado à cidade

Compare a vida urbana com o esquema legível. De um lado, um beco conhecido por apelido, usos mistos, acordos locais e percursos informais. Do outro, logradouro oficial, lote, zoneamento, proprietário e código de uso.

O segundo esquema cria capacidades reais: endereçar, tributar, instalar redes, reconhecer direitos e coordenar serviços. Também pode apagar acessos, deslocar práticas, tratar exceções como erro ou impor uma solução única.

O ponto mais importante para ensinar é que Scott não nos pede para escolher romanticamente a vida local contra qualquer cadastro. Ele pergunta o que acontece quando a administração confunde o esquema necessário para agir com a totalidade da cidade. Uma boa infraestrutura pública precisa de legibilidade, mas também de revisão, participação, conhecimento situado e formas de recurso.

## Lâmina 56 — Data Feminism: dados são relações de poder

Catherine D’Ignazio é artista, designer e professora. Lauren Klein pesquisa humanidades digitais e história cultural dos dados. Em *Data Feminism*, elas transformam crítica do poder em princípios de prática.

Esses princípios incluem examinar e desafiar o poder, valorizar corpo e emoção, repensar binários, abraçar pluralismo, considerar contexto e tornar o trabalho visível. Feminismo de dados não significa apenas trabalhar com dados sobre mulheres. Significa examinar como desigualdades e relações de poder atravessam aquilo que é contado e a maneira de contar.

Para a investigação urbana, surgem perguntas concretas: quem conta? Quem é contado? Quem realizou o trabalho invisível de coletar e limpar? Quem pode contestar uma categoria ou corrigir um registro? A crítica deixa de ser comentário externo e torna-se procedimento de projeto.

## Lâmina 57 — Simplificar sem confundir o esquema com o mundo

Representações precisam simplificar. Sem redução, teríamos o mapa de Borges na escala do território. O problema é esquecer a operação e começar a tratar a simplificação como natureza.

Podemos usar quatro cuidados. Declarar a finalidade: para que este recorte foi criado? Preservar procedência: de onde vieram os registros? Mostrar incerteza e ausência quando forem relevantes. Oferecer formas de contestação e atualização.

Esses cuidados não garantem neutralidade. Eles tornam decisões mais examináveis. Uma base pública deve conseguir agir e, ao mesmo tempo, admitir que suas categorias possuem história. Uma visualização deve orientar leitura e permitir que o leitor identifique limites. A maturidade metodológica não está em evitar toda simplificação, mas em impedir que ela se torne invisível e incontestável.

## Lâmina 58 — Contra-mapas e existência pública

Contra-mapear não significa apenas desenhar o oposto de um mapa oficial. Significa alterar autoria, categorias, fontes ou finalidades para tornar outras relações publicamente legíveis.

O projeto MedidaSP, ao comparar gênero em nomes de ruas, reorganiza um cadastro familiar para fazer aparecer uma desigualdade simbólica. Rios Des.Cobertos reinscreve cursos d’água apagados da paisagem cotidiana e permite relacionar memória, infraestrutura e território.

Esses exemplos não dispensam fonte, método ou crítica porque possuem intenção política. Ao contrário, sua força depende de mostrar como a operação foi feita. Um contra-mapa pode revelar ausências, mas também criar novas simplificações. O ganho está em ampliar quem pode representar a cidade, quais perguntas são admitidas e que realidades conseguem disputar reconhecimento.

---

# Capítulo 8 — Inteligência artificial como representação e infraestrutura

## Lâmina 59 — Observatório de Remoções: cartografia como infraestrutura de resistência

O Observatório de Remoções, coordenado pelo LabCidade da FAU-USP em parceria com o grupo Transborda da Unifesp, acompanha remoções e ameaças na Região Metropolitana de São Paulo desde 2012. O caso acrescenta uma dimensão importante aos exemplos anteriores: o contra-mapa participa diretamente de uma disputa por permanência e direitos.

Os registros combinam denúncias, imprensa, pesquisa de campo, dados oficiais e leitura de sentenças. A base procura identificar pessoas e territórios atingidos, agentes promotores, justificativas mobilizadas e localização dos conflitos. Universidade, movimentos, assessorias e comunidades participam de uma infraestrutura de produção de evidência.

Mapear, nesse caso, não significa somente representar um problema depois que ele aconteceu. Significa monitorar, denunciar, defender direitos e incidir em políticas e processos judiciais. O contra-mapa não é automaticamente justo nem completo; continua exigindo critérios e verificação. Sua diferença está em reorganizar autoria, finalidade e capacidade de ação.

## Lâmina 60 — Agora falaremos de inteligência artificial

Chegamos à inteligência artificial depois de construir um vocabulário sobre representação, classificação, infraestrutura e poder. Essa ordem é deliberada. Modelos de IA não aparecem fora dessas questões; eles as condensam.

Neste bloco não faremos uma história completa da tecnologia. A pergunta será: o que muda quando sistemas estatísticos capazes de produzir textos, imagens e classificações operam sobre representações anteriores do mundo?

Precisamos evitar dois mitos opostos. Um atribui ao modelo compreensão e autonomia quase mágicas. O outro o reduz a papagaio inútil e ignora sua capacidade efetiva de reorganizar trabalho e decisão. Analisaremos capacidade, mediação, materialidade e responsabilidade juntas.

## Lâmina 61 — IA também é representação

Dados, treinamento, modelo, prompt e saída aparecem numa sequência simplificada. Um modelo comprime regularidades de textos, imagens, tabelas, mapas e outros registros. Ele não acessa a cidade sem mediação; opera sobre inscrições anteriores e produz novas inscrições.

Isso explica tanto sua potência quanto seus limites. A escala dos registros permite reconhecer padrões e produzir combinações difíceis para uma pessoa. Mas categorias, ausências e desigualdades presentes na cadeia também podem ser incorporadas e transformadas.

O prompt adiciona contexto, não experiência. A saída exige verificação porque fluência não equivale a fonte, verdade ou responsabilidade. Usar IA no curso significa tratá-la como dispositivo representacional: perguntar de onde vem sua capacidade, que materiais recebeu, que inferências introduziu e quem responde pela decisão final.

## Lâmina 62 — Kate Crawford: IA não é artificial nem imaterial

Kate Crawford é pesquisadora de inteligência artificial, mídia e poder. Em *Atlas of AI* e no projeto *Anatomy of an AI System*, com Vladan Joler, ela desloca a atenção da interface limpa para as cadeias que sustentam o sistema.

A inteligência artificial depende de minérios, energia, água, logística, centros de dados, fabricação e descarte. Depende também de trabalho humano: coleta, rotulação, moderação, manutenção e avaliação. Finalmente, depende de instituições que definem objetivos, compram sistemas e distribuem consequências.

Quando dizemos “na nuvem”, territórios e trabalhos desaparecem linguisticamente. Crawford nos convida a mapear essa materialidade. A IA não é artificial porque se alimenta de natureza e trabalho; não é imaterial porque ocupa infraestruturas, consome recursos e produz impactos geograficamente distribuídos.

## Lâmina 63 — Uma câmera inteligente começa antes da câmera

Pense numa câmera urbana usada para reconhecer placas, pessoas ou ocorrências. Sua cadeia começa em território: minérios, água, energia, cabos e centros de dados. Passa por trabalho: montagem, coleta, rotulação, moderação e manutenção.

Na camada representacional, alguém define classes, corpus, rótulos, objetivo e margem de erro. Na camada pública, entram compra, implantação, produção de suspeição, decisão e possibilidade de recurso.

A pergunta de Crawford não é apenas “o modelo funciona?”. Perguntamos que recursos, trabalhos, classificações e instituições tornam seu funcionamento possível e quem suporta suas consequências. Uma taxa de acerto abstrata não informa como erros se distribuem entre grupos, situações e territórios. A análise técnica precisa alcançar a cadeia social e material na qual a técnica age.

## Lâmina 64 — Modelo é território e representação

A fluência da saída encobre duas cadeias que precisam ser examinadas juntas. A primeira é material: minérios, energia, centros de dados, equipamentos e trabalho. A segunda é representacional: corpus, rótulos, objetivos, parâmetros e prompts.

Há ainda uma camada pública: decisão, consequência, contestação e documentação. Não basta saber que um modelo foi treinado com determinado conjunto. Precisamos perguntar onde ele opera, quem é afetado, como seus resultados entram numa instituição e que alternativa existe quando falha.

Onde termina o modelo e começam suas infraestruturas? A pergunta não possui resposta simples. A fronteira técnica pode ser desenhada, mas a responsabilidade não deve desaparecer nela. O sistema relevante para a investigação inclui tudo aquilo sem o qual a decisão automatizada não teria sido produzida.

## Lâmina 65 — Limites da fluência

Modelos generativos podem explicar, resumir, comparar e sugerir com impressionante fluência. Mas fluência não é experiência, acesso garantido à fonte ou responsabilidade. Uma frase convincente pode combinar informação correta, inferência plausível e invenção sem sinalizar a diferença.

O modelo não conhece uma rua por habitá-la, não sofre as consequências de uma classificação e não assume obrigação pública pelo erro. Isso não impede seu uso. Define o tipo de parceria possível.

Precisamos oferecer fontes quando forem decisivas, solicitar distinção entre citação e paráfrase, verificar afirmações e documentar decisões. Quanto mais polida a resposta, maior a tentação de encerrar a investigação. No curso, a saída será tratada como material intermediário: uma representação a ser lida, confrontada e transformada.

## Lâmina 66 — Uma parceria com responsabilidades assimétricas

Podemos pedir ao modelo que proponha perguntas, identifique termos, compare argumentos, encontre inconsistências e ajude a reformular explicações. Essas capacidades economizam tempo e ampliam caminhos exploráveis.

Mas perguntar, verificar, documentar e decidir permanecem responsabilidades humanas. A assimetria é importante: o modelo participa da produção, mas não responde pelas consequências. Quem assina um mapa, relatório ou investigação precisa compreender suficientemente o que apresenta.

Uma boa parceria não esconde o uso da ferramenta nem transfere a ela a autoridade. Registra o que foi solicitado, que material foi fornecido, que partes foram verificadas e que escolhas foram rejeitadas. Autoria aparece como capacidade de julgar e sustentar o percurso, não como fantasia de produção sem mediação.

---

# Capítulo 9 — Investigar: da inquietação à evidência

## Lâmina 67 — Agora falaremos de investigação

Retornamos à matriz inicial. Depois de representação, complexidade, classificação, mapas e IA, podemos formular com mais precisão o que significa investigar.

Investigar não é acumular informação até que a resposta apareça. É organizar uma relação revisável entre dúvida, evidência, representação e ação. A dúvida precisa conseguir aprender; a evidência precisa ter procedência; a representação precisa trabalhar para a pergunta; a ação precisa reconhecer consequências.

Este bloco prepara uma micro-oficina. O objetivo não será resolver um problema urbano, mas transformar uma inquietação em pergunta investigável e identificar uma primeira evidência possível.

## Lâmina 68 — Da inquietação à pergunta

Uma investigação pode começar por desconforto, curiosidade, experiência ou contradição. “Esta praça parece inacessível.” “Meu bairro não aparece neste mapa.” “Quase todas as ruas homenageiam homens.” Essas percepções são valiosas, mas ainda não constituem conclusão.

Transformar inquietação em pergunta exige abrir espaço para surpresa. Em vez de “provar que a praça é inacessível”, podemos perguntar: que barreiras físicas, temporais e informacionais afetam diferentes formas de acesso? A nova formulação indica evidências e permite que o resultado contrarie nossa impressão inicial.

Uma boa pergunta não precisa ser neutra no sentido de indiferente. Pode nascer de compromisso político ou experiência pessoal. Precisa, porém, declarar seu recorte e aceitar ser reformulada pelo encontro com o mundo.

## Lâmina 69 — Paulo Freire e a leitura do mundo

Paulo Freire foi educador pernambucano, ligado à alfabetização de adultos e à educação popular. Sua conhecida formulação de que a leitura do mundo precede a leitura da palavra ajuda a situar a investigação como problematização da experiência.

Ler o mundo não significa que experiência individual seja evidência suficiente para qualquer afirmação. Significa reconhecer que perguntas nascem de relações vividas e que conhecer envolve tornar essas relações discutíveis coletivamente.

Uma educação bancária entregaria categorias e métodos como conteúdos prontos. Uma prática problematizadora pergunta como os sujeitos nomeiam sua realidade, confronta essas nomeações com outras evidências e transforma professor e alunos em participantes responsáveis do conhecimento. No curso, Freire ajuda a ligar investigação técnica à capacidade de formular o mundo como problema, não como destino dado.

## Lâmina 70 — A primeira ação é observar uma evidência

Antes de escolher software, identifique uma evidência que possa tensionar a pergunta. Pode ser uma tabela, mapa, fotografia, documento, caminhada, entrevista, imagem aérea ou confronto entre fontes.

Evidência não é qualquer informação relacionada ao tema. É algo cuja origem e relação com a pergunta conseguimos explicar. Uma fotografia pode mostrar uma barreira em determinado momento, mas não medir automaticamente sua frequência. Uma base pode oferecer cobertura ampla e ainda ignorar experiências que não cabem em seus campos.

A primeira ação deve ser pequena: abrir uma fonte, ler metadados, observar um lugar, comparar duas representações. Depois perguntamos o que ela permite afirmar, o que não permite e que nova evidência seria necessária. Ferramentas entram quando a operação investigativa estiver minimamente reconhecida.

## Lâmina 71 — Micro-oficina: ausência, pergunta, evidência

Escolha uma ausência urbana que lhe incomode. Escreva uma frase puramente descritiva, sem explicar a causa. Depois transforme a frase em pergunta aberta à revisão. Finalmente, indique uma primeira evidência possível e suas limitações.

Exemplo: “Esta viela não aparece no mapa oficial.” Pergunta: “Como diferentes instituições e moradores registram os caminhos desta área, e que efeitos as divergências produzem?” Evidências iniciais: cadastro municipal, mapa colaborativo, observação de campo e relatos locais. Cada fonte vê alguma coisa e possui limites.

[Pausa sugerida.] O resultado da oficina não é um projeto pronto. É uma unidade mínima de investigação: uma ausência nomeada, uma pergunta capaz de aprender e uma evidência cuja procedência pode ser examinada.

---

# Capítulo 10 — Ler com ChatGPT sem abandonar a fonte

## Lâmina 72 — Agora vamos ler Drucker com ChatGPT

O último bloco realiza uma demonstração de leitura assistida. Retornaremos ao artigo de Johanna Drucker porque ele é uma espinha dorsal conceitual do curso e porque sua argumentação exige atenção a termos, exemplos e imagens.

O objetivo não é provar que o ChatGPT “entendeu” Drucker. Queremos tornar visível um protocolo no qual a fonte permanece central. O modelo ajudará a produzir uma síntese inicial, levantar termos e formular objeções. A turma verificará cada movimento.

Essa demonstração também prepara o podcast e os materiais do curso: IA pode ampliar acesso e oferecer explicações, mas precisa distinguir o que o texto diz, o que inferimos e o que acrescentamos como exemplo.

## Lâmina 73 — Fonte primeiro, síntese depois

Começamos situando autora, artigo, revista e data. Lemos um trecho original. Só então pedimos ao modelo uma tese e termos centrais. Para cada afirmação, buscamos evidência no texto.

Marcamos cinco estatutos: citação literal, paráfrase, inferência do modelo, exemplo novo e dúvida. Essa separação é crucial. Uma boa explicação pode conter algo que Drucker nunca afirmou diretamente. O acréscimo pode ser útil, desde que não seja devolvido à autora como citação ou posição comprovada.

Depois pedimos uma objeção e a julgamos coletivamente. O modelo não encerra a leitura; ajuda a produzir objetos de leitura. Ao final, registramos referência, decisões e questões em aberto. O protocolo vale para artigos, livros, bases e documentos técnicos.

## Lâmina 74 — Demonstração: três vozes sobre a tela

Durante a demonstração, mantenha três camadas visíveis. A primeira é o texto de Drucker. A segunda é a resposta do modelo. A terceira é a decisão interpretativa da turma.

Pergunte: onde está no original a evidência para esta frase? O modelo transformou uma metáfora em definição? Confundiu *capta* com uma rejeição total dos dados? Acrescentou um exemplo urbano que não pertence ao artigo? A resposta pode estar correta como inferência e incorreta como atribuição.

Essa prática ensina mais do que detectar alucinações. Mostra que toda síntese reorganiza ênfases. Nós também interpretamos quando lemos. A diferença é tornar o processo responsável: manter a fonte acessível, declarar o estatuto das frases e aceitar correção. A IA entra como interlocutora, não como origem final da autoridade.

## Lâmina 75 — Fechamento: da ausência à próxima operação

Começamos com algo que existia na cidade e não aparecia adequadamente no mapa. Percorremos a capacidade humana de representar, a necessidade de reduzir, a complexidade das relações urbanas, a construção de categorias, a produção de mapas, a materialidade da IA e a responsabilidade da investigação.

Podemos fechar com uma sequência aberta: ausência, dúvida, evidência e próxima operação. A ausência não prova sozinha uma injustiça ou um erro; ela produz uma pergunta. A pergunta busca evidências. A evidência exige representação. A representação orienta uma ação e cria novas ausências e dúvidas.

O compromisso do curso não é produzir uma imagem final da cidade. É aprender a construir representações úteis sem esquecer que são parciais; usar dados sem tratá-los como naturais; trabalhar com IA sem terceirizar julgamento; e transformar aquilo que não aparece em uma investigação pública, verificável e capaz de agir.

[Pausa final.] A pergunta que fica é simples: qual ausência você deseja investigar — e qual será sua próxima operação?

---

# Créditos e referências essenciais para acompanhamento

- ALEXANDER, Christopher. “A City Is Not a Tree”.
- BORGES, Jorge Luis. “Do rigor na ciência”.
- BOWKER, Geoffrey C.; STAR, Susan Leigh. *Sorting Things Out*.
- CRAWFORD, Kate. *Atlas of AI*.
- D’IGNAZIO, Catherine; KLEIN, Lauren F. *Data Feminism*.
- DRUCKER, Johanna. “Humanities Approaches to Graphical Display”.
- FREIRE, Paulo. *Pedagogia do oprimido*.
- HALL, Stuart et al. *Representation: Cultural Representations and Signifying Practices*.
- HARLEY, J. B. “Deconstructing the Map”.
- JACOBS, Jane. *Morte e vida de grandes cidades*.
- MORIN, Edgar. *Introdução ao pensamento complexo*.
- SCOTT, James C. *Seeing Like a State*.
- WEAVER, Warren. “Science and Complexity”.

## Nota editorial

Este roteiro acompanha as 75 lâminas da apresentação. Foi escrito para estudo e oralização, não para substituir os textos originais. Antes de uma gravação pública, recomenda-se uma revisão oral por capítulo, sobretudo para ajustar duração, pronúncia de nomes, pausas e eventuais comentários pessoais do professor.
