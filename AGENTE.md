# Guia

Orientações para a atuação no projeto, deve ser seguido como prioridade de tudo.

## Estrutura

- `diagramas/`: exemplos e diagramas oficiais em PlantUML.
- `specs/`: especificacoes funcionais por feature.
- `PROJETO.md`: especificacao geral do projeto, com estrutura e padroes.

## Fluxo recomendado

- Quando pedir para fazer ou executar uma feature, ler o arquivo README.md em specs para orientações.
- Quando pedir para fazer ajuste na feature, ler o arquivo README.md em specs para orientações.
- Quando pedir para criar uma feature, ler o arquivo README.md em specs para orientações.

## Leitura obrigatoria inicial

Antes de fazer qualquer atuação:

1. Todas as pastas tem um arquivo `README.md` com orientacoes especificas, ler antes de atuar.
2. Ler o arquivo `PROJETO.md` para entender a estrutura geral e os padroes do projeto.

## Regras de qualidade

### O que deve fazer

- Usar nomeclaturas de classes, métodos e variáveis em português e descritivas.
- Seguir os padrões de qualidade Clean Code.
- Usar padrões SOLID se aplicável.
- Seguir sempre os padrões de codificação do projeto.
- Sempre reusar código existente, evitando duplicação.

### O que nao deve fazer

- Funções ou métodos com muitos parâmetros deve ser passados como objeto.
- fazer funções ou métodos muito longos, deve dividir em funções menores.
- Evitar funções dentro de funções, deve criar funções separadas.
- deixar funções que são ultilizadas apenas na classe como públicas, deve criar funções privadas.
- nao deve criar colunas ou campos que nao estejam listados no diagramas de classes ou nas especificacoes.
- deve sempre evitar cadastro no banco dentro de loops, deve fazer um array e cadastrar em lote, fazer dentro de loop so em ultimo caso nao tenha como evitar.
