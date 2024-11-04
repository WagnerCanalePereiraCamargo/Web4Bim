# Backlog de Tarefas para o Projeto de Gerenciamento de Tarefas

## Menu
1. [Tarefa 1: Página de "Em Construção"](##tarefa-1-página-de-em-construção)
2. [Tarefa 2: Configuração do Ambiente e API Base](##tarefa-2-configuração-do-ambiente-e-api-base)
3. [Tarefa 3: Implementação de Autenticação e Sistema de Usuários](##tarefa-3-implementação-de-autenticação-e-sistema-de-usuários)
4. [Tarefa 4: CRUD de Tarefas](##tarefa-4-crud-de-tarefas)
5. [Tarefa 5: Funcionalidades de Filtro, Ordenação e Melhorias Finais](##tarefa-5-funcionalidades-de-filtro-ordenação-e-melhorias-finais)

---

## Tarefa 1: Página de "Em Construção"
- **Criar uma estrutura básica do projeto**:
  - Definir diretórios para front-end e back-end.
  - Inicializar o projeto com arquivos padrão (index.html, app.js, styles.css).
  
- **Adicionar Vue.js por CDN para suportar a interface**:
  - Incluir a biblioteca Vue.js no arquivo HTML.

- **Desenvolver uma página inicial com a mensagem "Em construção"**:
  - Criar a estrutura HTML da página.
  - Adicionar a mensagem "Em construção".

- **Implementar estilo básico (ex.: CSS minimalista) para a página**:
  - Criar regras CSS simples para a página.

- **Documentar a configuração inicial e estrutura básica do projeto**:
  - Criar um arquivo README.md com instruções de configuração.

---

## Tarefa 2: Configuração do Ambiente e API Base
- **Configurar a API com um servidor básico (Node.js ou outra alternativa)**:
  - Instalar dependências (Express, CORS, etc.).
  - Criar um servidor básico que escute em uma porta específica.

- **Configurar um banco de dados simples (SQLite ou outro) para o armazenamento inicial**:
  - Instalar dependências para o banco de dados.
  - Criar a estrutura básica do banco de dados (ex.: conexão, tabelas).

- **Testar a comunicação entre o front-end e a API**:
  - Criar uma rota simples na API.
  - Fazer uma chamada de teste do front-end para verificar a comunicação.

- **Documentar o processo de configuração do ambiente e da API**:
  - Atualizar o README.md com detalhes sobre a configuração do ambiente e a estrutura da API.

---

## Tarefa 3: Implementação de Autenticação e Sistema de Usuários
- **Implementar sistema de registro e login de usuários usando JWT**:
  - Criar rotas para registro e login na API.
  - Implementar a lógica para geração e validação de tokens JWT.

- **Configurar proteção nas rotas da API para que apenas usuários autenticados acessem suas tarefas**:
  - Criar middleware de autenticação.
  - Aplicar middleware nas rotas de tarefas.

- **Desenvolver componentes Vue.js para as telas de login e registro**:
  - Criar formulários de login e registro com validação.

- **Testar e documentar o fluxo de autenticação**:
  - Testar todos os cenários (sucesso, falha, token expirado).
  - Documentar o fluxo no README.md.

---

## Tarefa 4: CRUD de Tarefas
- **Desenvolver endpoints da API para as operações CRUD de tarefas**:
  - Criar rotas para criar, ler, atualizar e excluir tarefas.

- **Criar componentes Vue.js para adicionar, editar, exibir e excluir tarefas**:
  - Implementar a lógica nos componentes para gerenciar tarefas.

- **Integrar o front-end com a API para garantir persistência de dados**:
  - Fazer chamadas API nos componentes Vue.js para operações CRUD.

- **Testar e documentar as funcionalidades de CRUD**:
  - Testar todas as operações CRUD.
  - Documentar no README.md.

---

## Tarefa 5: Funcionalidades de Filtro, Ordenação e Melhorias Finais
- **Adicionar filtros e opções de ordenação de tarefas**:
  - Implementar lógica para filtrar e ordenar tarefas no front-end.

- **Implementar notificações visuais para confirmações de ações (ex.: sucesso ou falha na criação de tarefas)**:
  - Adicionar mensagens de feedback após operações de CRUD.

- **Revisar a interface para usabilidade e responsividade**:
  - Realizar testes de usabilidade e aplicar melhorias.

- **Corrigir bugs, realizar ajustes e documentar o software para a entrega final**:
  - Fazer uma lista de bugs encontrados e resolvê-los.
  - Atualizar a documentação para refletir a versão final do projeto.

---
