# Sobre o projeto
Aplicativo para fazer vendas e enviar para API do sistema SIAF. 
O aplicativo antigo está desatualizado e não é possível fazer alterações e builds, mas deve ser migrado para um novo projeto como android mais atualizado.

# Tecnologias
- Java para o desenvolvimento do aplicativo android
- android studio como IDE de desenvolvimento

## Arquitetura
- API REST para comunicação com o sistema SIAF rodando para quando a aplicacao estiver online.
- banco local no dispositivo usando quando o aplicativo estiver offline;

### banco de dados
banco de dados local usando o realm para armazenar.

### estrutura de pastas
- `siaf-pedidos-android`: projeto antigo.
- `siaf-pedidos-android-novo`: projeto novo.

# orientações e regras do projeto
- Deve migrar todo o código do projeto antigo para o novo projeto, mantendo a mesma estrutura de pastas e arquivos.
- Deve manter o mesmo codigo e lógica do projeto antigo, não deve fazer alterações no código, apenas migrar para o novo projeto.
- Fazer ajustes necessários para o código funcionar no novo projeto, como ajustes de dependências, configurações e etc.
- fazer alterações no código apenas se der erro de compilação, não deve fazer alterações no código se não for necessário para o funcionamento do aplicativo.
- atualizar as dependências do projeto para as versões mais recentes, mas mantendo a compatibilidade com o código existente.