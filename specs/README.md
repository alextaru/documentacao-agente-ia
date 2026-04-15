# Especificacoes de Features

Regra geral para horientações de como criar e executar features.

## Estrutura

- `features/`: pasta de arquivos das features, um arquivo por feature.
- `templates/`: modelos base para criação e entendimento de modelos.
- `feature-registry.yaml`: quadro consolidado de status das features.

## Como identificar feature

- O nome do arquivo deve seguir o formato `XXXX-spec-nome-da-feature.md`, onde `XXXX` e um numero sequencial unico.

## Explicacao cabecalho da feature

- id: identificador unico da feature.
- title: titulo curto da feature.
- status: status atual da feature.
- depends_on: lista de features das quais esta feature depende para ser executada, usando o formato de id das features.

### Politica de atualizacao de status

- `backlog`: definida, sem preparo para execucao.
- `ready`: detalhada, pronta para execucao.
- `in_progress`: em execucao.
- `done`: concluida e validada.

### Ciclo de status

`backlog -> ready -> in_progress -> done`

## Regras

### Fazer ou ajustar uma feature

#### Leitura obrigatoria

- Ler `feature-registry.yaml`.
- Ler o arquivo da feature alvo.
- Ler features dependentes.
- Ler instrucoes na pasta `diagramas`.

#### Regras de execucao

- executar sempre por ordem crescente de ID.
- Executar apenas features com dependencias resolvidas.
- Executar apenas uma feature com status `ready` ou `in_progress`.
- Executar apenas dependencias com status `ready` ou `in_progress`.
- Caso haja dependencias com status `in_progress`, executar essas primeiro.
- Status `in_progress` deve ler o Plano de execucao e fazer apenas os Ajustes que nao estejam ✅, apos terminar os ajustes deve marcar como ✅.
- Features com status `backlog` nao devem ser executadas, caso tenha dependencias deve ser executadas primeiro, caso contrario deve seguir para a proxima.
- Na feature adiconar o plano de execucao em Plano de execucao, para futuras consultas.
- Atualizar para `done` ao finalizar.
- Em Ajustes não deve adicionar novas tarefas, apenas marcar como ✅ as tarefas que foram realizadas, caso seja feito algum ajuste de ser requistrado no Plano de execucao.
- Em plano de execucao deve ser detalhodo, registrar o mesmo plano de execucao usando pelo agente antes de executar a tarefa, para ficar como memoria futura.

### Criar uma feature

#### Leitura obrigatoria

- Ler instrucoes na pasta `templates`.

#### Regras de execucao

- Toda feature deve possuir ID unico no formato `XXXX-spec-nome-da-feature.md` sendo `XXXX` um numero sequencial e nome-da-feature o nome sugerido na criação.
- O status no arquivo da feature e no registry deve ser consistente.
- deve seguir o template em na pasta `templates`.
- Deve ser registrada no `feature-registry.yaml` com status `backlog`.
- Não deve especificar nada apenas criar no formato do template, pois as especificações serão adicionadas posteriormente.
- ao registrar no `feature-registry.yaml` não deve adicionar dependências, pois elas serão adicionadas posteriormente.
