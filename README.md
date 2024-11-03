# Documentação do Projeto: Agenda de Tarefas

## Menu
1. [Resumo do Projeto](#resumo-do-projeto)
2. [Planejamento e Escopo](#planejamento-e-escopo)
   - [Requisitos Funcionais](#requisitos-funcionais)
   - [Requisitos Não Funcionais](#requisitos-não-funcionais)
3. [Tecnologias Utilizadas](#tecnologias-utilizadas)
4. [Modelo do Banco de Dados](#modelo-do-banco-de-dados)
   - [Tabela Usuário](#tabela-usuario)
   - [Tabela Tarefa](#tabela-tarefa)
---
## Resumo do Projeto
Agenda de Tarefas é um sistema desenvolvido para facilitar o gerenciamento de atividades diárias dos usuários, permitindo a criação, edição, exclusão e finalização de tarefas. O projeto inclui uma aplicação web e outra mobile.

## Planejamento e Escopo

### Requisitos Funcionais
- **CRUD de Usuário**: Cadastro de usuários com autenticação por senha.
- **CRUD de Tarefas**: Adicionar, editar, excluir e marcar como concluída.
- **Interface Web e Mobile**: Disponível para ambos os dispositivos.

### Requisitos Não Funcionais
- **API**: O sistema deve ter uma API para comunicação entre frontend e backend.
- **Desempenho**: O banco de dados deve estar estruturado para permitir consultas rápidas e escaláveis.
- **Responsividade**: O sistema deve ser responsivo e acessível em múltiplos dispositivos.

## Tecnologias Utilizadas
- **Frontend Web**: HTML, CSS, Vue.js
- **Frontend Mobile**: XML
- **Backend**: Node.js ou Spring Boot
- **Banco de Dados**: MySQL
- **Ferramentas de Desenvolvimento**: Visual Studio Code, Git

## Modelo do Banco de Dados

### Tabela Usuário
- `ID_Usuario`: Chave primária, identifica cada usuário de forma única.
- `Nome`: Nome do usuário.
- `Senha`: Armazena a senha para autenticação.

### Tabela Tarefa
- `ID_Tarefa`: Chave primária, identifica cada tarefa de forma única.
- `Titulo`: Título ou nome da tarefa.
- `Descricao`: Detalhes adicionais sobre a tarefa.
- `Data_Criacao`: Data de criação da tarefa.
- `Data_Conclusao`: Data em que a tarefa foi marcada como concluída.
- `Status`: Indica o status da tarefa (pendente ou concluída).
- `ID_Usuario`: Chave estrangeira, vincula a tarefa a um usuário específico.
