# Diagramas (PlantUML)

Este diretorio contem diagramas de referencia a features, é usado o PlantUML para criar os diagramas.

## Estrutura de arquivos

- `classes`: diagramas de classes.
- `fluxogramas`: diagramas de fluxos.

## Como Identificar a qual feature um diagrama se refere
- O nome do arquivo deve seguir o formato `XXXX-descricao.puml`, onde `XXXX` e o numero sequencial da feature a qual o diagrama se refere.
- Toda feature pode ter um ou mais diagramas associados, e cada diagrama deve ser identificado pelo seu número sequencial.

## Como usar

1. cada arquivo `.puml` representa um diagrama.
2. o codico no inicio do arquivo referencia qual feature ele representa.
3. os diagramas mostram o fluxo de forma simplificada para analise não deve ser usado para desenvolvimento, mas sim para entendimento do sistema.
4. na pasta classes, mostra como as classes devem ser estruturadas e implementadas.
