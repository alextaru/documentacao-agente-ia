# Diagramas (PlantUML)

Este diretorio contem diagramas de referencia a features, é usado o PlantUML para criar os diagramas.

## Estrutura de pastas

- `classes`: diagramas de classes, mostrando a estrutura do banco de dados.
- `fluxogramas`: diagramas de fluxos ou fluxogramas.
- `exemplos`: diagramas de exemplo para referencia quando for criar novos diagramas, não devem ser usados diretamente.

## Como Identificar a qual feature um diagrama se refere

- O nome do arquivo deve seguir o formato `XXXX-descricao.puml`, onde `XXXX` e o numero sequencial da feature a qual o diagrama se refere.
- Toda feature pode ter um ou mais diagramas associados, e cada diagrama deve ser identificado pelo seu número sequencial.

## Como usar

1. os fluxogramas mostram o fluxo de forma simplificada para analise e entendimento do sistema.
2. não deve fazer um fluxo diferente que esteja no fluxograma, deve seguir o fluxo do fluxograma para garantir que o desenvolvimento esteja alinhado com o diagrama.
3. na pasta classes, mostra como as classes devem ser estruturadas e implementadas, deve ser usado no desenvolvimento para garantir que a estrutura do codigo esteja alinhada com o diagrama.
4. Não deve alter as nome das classes, metodos e propriedades do diagrama de classes, deve seguir o diagrama para garantir que a estrutura do codigo esteja alinhada com o diagrama.
5. as classes referenciao as tabelas do banco de dados, no codigo devem usar o padrao de nomenclatura padrao usado caso haja.