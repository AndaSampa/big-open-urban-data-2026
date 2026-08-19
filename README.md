# Big Open Urban Data — 2026

## Dados, cartografia e inteligência artificial para investigar representações da cidade

Repositório público da disciplina **Big Open Urban Data**, ministrada por **Fernando Gomes** na pós-graduação da Escola da Cidade em 2026.

Cidades não são feitas apenas de edifícios, ruas e infraestruturas. São também feitas pelas formas como escolhemos registrá-las, classificá-las e representá-las. Esta disciplina propõe investigar essas representações e construir maneiras críticas de compreender a cidade por meio de dados, cartografia e inteligência artificial.

> **Dados e mapas não são a cidade: são representações produzidas por pessoas, instituições, comunidades, sensores, plataformas e escolhas técnicas.**

## Comece por aqui

- [Programa da disciplina](docs/programa.md)
- [Investigação de representação](docs/investigacao.md)
- [Avaliação e revisões](docs/avaliacao.md)
- [Aula 0 — Como aprendemos a ver uma cidade?](aulas/aula-00/README.md)
- [Aula 1 — Quem produz a cidade que aparece nos dados?](aulas/aula-01/README.md)
- [Aula 2 — O que muda quando os dados recebem lugar, forma, escala e vizinhança?](aulas/aula-02/README.md)

## Percurso do curso

O curso acompanha uma investigação que ganha novas dimensões a cada encontro:

> **registro → X/Y → Z → relação → argumento**

| Encontro | Inquietação central | Movimento da investigação |
|---|---|---|
| **Aula 0** | Como aprendemos a ver uma cidade? | representação, complexidade e formulação da investigação |
| **Aula 1** | Quem produz a cidade que aparece nos dados? | fontes, cadastros, dados abertos, plataformas e proveniência |
| **Aula 2** | O que muda quando os dados recebem lugar, forma, escala e vizinhança? | geometrias, QGIS, SRC, tematização e primeira relação espacial |
| **Aula 3** | O que cada modo de observação torna visível? | superfície, elevação, altura, sensores e LiDAR |
| **Aula 4** | Quando representações relacionadas se tornam evidência? | sobreposição, associação, explicações alternativas e modelos |
| **Aula 5** | Que cidades conseguimos tornar perceptíveis? | trabalhos da turma, síntese e apresentação da investigação do professor |

As aulas futuras serão acrescentadas conforme forem produzidas e validadas. A **Aula 2 já está disponível antecipadamente** para leitura; seu roteiro prático poderá receber pequenos ajustes depois da simulação em sala.

## Materiais disponíveis

### Aula 0 — Representação e complexidade

- apresentação completa em PDF;
- podcast textual e versão para impressão;
- caderno de apoio e versão para impressão;
- fontes e créditos das imagens.

### Aula 1 — Dados abertos e produção da cidade nos dados

- apresentação completa em PDF;
- roteiro integral dos prompts da investigação ao vivo;
- fontes, links e créditos.

### Aula 2 — Da tabela ao mapa

- apresentação completa em PDF;
- roteiro modular de prompts;
- preparação do GeoPackage e do projeto QGIS;
- cardápio de explorações com Censo, escolas, POIs e relações espaciais;
- fontes, links e créditos.

## A investigação da disciplina

Cada estudante, individualmente ou em dupla, escolherá algo que exista, aconteça ou importe em uma cidade, mas apareça pouco, mal ou de forma enganosa nas representações disponíveis.

A investigação deverá:

1. formular uma pergunta urbana clara;
2. examinar como o fenômeno já é representado;
3. selecionar e avaliar criticamente uma ou mais fontes;
4. realizar uma operação compreensível sobre dados ou evidências;
5. construir uma representação;
6. apresentar um pequeno achado ou deslocamento de olhar;
7. discutir o que pode e o que não pode ser afirmado;
8. reconhecer o que permanece invisível;
9. documentar o uso de inteligência artificial.

Não é necessário produzir uma tese nem dominar previamente programação ou geoprocessamento. Uma investigação pequena, verificável e intelectualmente honesta vale mais que um procedimento sofisticado sem uma pergunta clara.

## Uso de inteligência artificial

O uso de inteligência artificial é permitido e esperado como apoio à formulação de perguntas, compreensão de fontes, preparação de dados, programação, análise e comunicação.

Seu uso não transfere autoria ou responsabilidade. As pessoas responsáveis pela investigação devem:

- conferir as fontes;
- compreender o propósito das operações;
- inspecionar arquivos e resultados;
- registrar decisões e transformações;
- reconhecer erros, incertezas e ausências;
- explicar o que foi feito com IA e o que precisou ser corrigido.

Os prompts publicados neste repositório não são fórmulas universais. Eles registram protocolos didáticos utilizados nas aulas e podem ser adaptados a outras cidades, perguntas e condições técnicas.

## Ferramentas e formatos

Ao longo do curso utilizaremos, entre outros recursos:

- ChatGPT em modo Work para organizar, processar e documentar investigações;
- QGIS para abrir, inspecionar, relacionar e representar dados espaciais;
- GeoPackage como formato principal de trabalho cartográfico;
- fontes governamentais, colaborativas e corporativas com diferentes condições de acesso;
- tabelas, mapas, imagens, modelos de elevação, nuvens de pontos e outros modos de observação.

As ferramentas entram em função das perguntas. A disciplina não pretende formar especialistas num software específico.

## Estrutura do repositório

```text
big-open-urban-data-2026/
├── README.md
├── LICENSE
├── docs/
│   ├── programa.md
│   ├── investigacao.md
│   └── avaliacao.md
└── aulas/
    ├── aula-00/
    │   ├── README.md
    │   ├── apresentacao/aula-00.pdf
    │   ├── materiais/
    │   │   ├── podcast-textual-aula-00.md
    │   │   ├── podcast-textual-aula-00-a4.pdf
    │   │   ├── caderno-de-apoio.md
    │   │   └── caderno-de-apoio-a4.pdf
    │   └── fontes-e-creditos.md
    ├── aula-01/
    │   ├── README.md
    │   ├── apresentacao/aula-01.pdf
    │   ├── prompts-investigacao.md
    │   └── fontes-e-creditos.md
    └── aula-02/
        ├── README.md
        ├── apresentacao/aula-02.pdf
        ├── prompts-aula-02.md
        └── fontes-e-creditos.md
```

O repositório público contém os materiais de estudo e execução. Arquivos temporários, testes visuais, versões substituídas e bastidores de produção não são publicados.

## Abertura, autoria e reutilização

Este material é compartilhado para estudo, adaptação e aperfeiçoamento. Ao reutilizar conteúdos, preserve a autoria, as referências e as licenças específicas indicadas nos arquivos de fontes e créditos.

Textos, imagens, mapas, livros, artigos, dados e plataformas citados podem possuir licenças próprias. A presença de uma referência neste repositório não altera os direitos de seus autores ou produtores.

## Versão anterior do curso

A edição anterior permanece disponível como registro histórico em [AndaSampa/big-open-urban-data](https://github.com/AndaSampa/big-open-urban-data). Ela possui outra organização pedagógica, materiais em notebooks e maior concentração na cidade de São Paulo.

---

**Professor:** Fernando Gomes  
**Instituição:** Escola da Cidade  
**Edição:** 2026
