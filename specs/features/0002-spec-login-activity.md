---
id: 0002
title: login-activity
status: done
depends_on: []
---

# Contexto

Implementar a Login Activity, que é a tela de login do aplicativo.

# Escopo

Passar todo o codigo da Login Activity, incluindo layout e suas dependencias, do projeto antigo para o novo projeto, mantendo a mesma estrutura de pastas e arquivos.

## Requisitos nao funcionais

- Deve manter o mesmo codigo e lógica do projeto antigo, não deve fazer alterações no código, apenas migrar para o novo projeto.

## Requisitos funcionais

## Regras de negocio

-fazer apenas arquivos relacionados e sub arquivos relacionados.

## Referencias

`siaf-pedidos-android/app/src/main/java/br/com/adsoft/siafpedido/activity/LoginActivity.java`: login activity do projeto antigo.
`siaf-pedidos-android-novo/app/src/main/java/br/com/adsof/siafpedido/activity/LoginActivity.java`: login activity do projeto novo.

## Detalhes da implementacao

- nao deve fazer alterações no código, apenas migrar para o novo projeto.
- deve passar tambem todos os arquivos relacionados a Login Activity, como layout, imagens e etc e todos os recursos necessários para o funcionamento da tela.
- a PrincipalActivity que é chamada pela LoginActivity não deve ser migrada agora, deve deixar ela como está no projeto novo, sem alterações.

## Ajustes

- ✅ Corrigido o fluxo entre LoginActivity e ConfiguracaoActivity, com migracao da activity de configuracao, seus recursos e ajuste do retorno em onActivityResult com chamada a super.
- ✅ Migradas as classes e interfaces ja criadas no projeto novo que sao dependencias diretas e indiretas da LoginActivity, incluindo helpers, services, controllers, models, responses, views, manifest e dependencias Gradle correlatas.
- ✅ Corrigidos os erros de compilacao do Android resource linking com migracao dos drawables `circulo_*` faltantes e adicao dos aliases de cores (`purple_*`, `teal_*`, `black`, `white`) usados pelos temas.

## Plano de execucao

1. Levantar dependencias diretas da LoginActivity no projeto antigo e validar existencia no projeto novo.
2. Migrar o arquivo da activity e ajustar somente o pacote para o namespace atual do projeto novo.
3. Migrar os recursos visuais diretamente utilizados pela tela de login (layout, include de toolbar, menu e drawables).
4. Migrar recursos de valores usados pela tela de login (cores, dimensoes, strings e paleta material referenciada).
5. Ajustar build.gradle do app novo com bibliotecas usadas diretamente pela LoginActivity.
6. Atualizar o status da feature no registro consolidado.
