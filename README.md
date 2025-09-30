# 💼 DevBills API

API backend para o projeto DevBills, responsável por gerenciar contas, despesas e recebimentos.  
Serve como suporte para o front-end (app ou dashboard) lidar com dados financeiros de forma segura e organizada.

---

## 🚧 Status do Projeto

> Em desenvolvimento — algumas rotas ainda podem estar faltando ou serem alteradas.

---

## Tecnologias Utilizadas 🛠

- Node.js  
- Express  
- (Banco de dados como PostgreSQL / MySQL / MongoDB — ajustar conforme uso)  
- ORM / query builder (ex: Prisma, Sequelize, Mongoose)  
- Validação de dados (ex: Joi, Zod)  
- Middleware para tratamento de erros, CORS, autenticação (se aplicável)  

---

## Endpoints Principais (exemplo) ⚙

| Método | Rota                        | Função                       |
|--------|-----------------------------|------------------------------|
| GET    | `/bills`                    | Listar todas as contas/despesas/receitas |
| GET    | `/bills/:id`                | Mostrar uma conta específica |
| POST   | `/bills`                    | Criar nova conta / despesa / receita |
| PUT    | `/bills/:id`                | Atualizar dados de uma conta |
| DELETE | `/bills/:id`                | Remover uma conta / despesa / receita |

---

## 🚀 Como Rodar Localmente

1. Clone o repositório  
   ```bash
   git clone https://github.com/nandosabino/devbills-api.git
   ```
2. Acesse a pasta do projeto
   ```bash
   cd devbills-api
   ```
3. Instale dependências
   ```bash
   npm install
   ```
4. Configure variáveis de ambiente
   Crie um arquivo .env com as configurações necessárias, por exemplo:
   ```ini
   PORT=3000
   DATABASE_URL=...
   JWT_SECRET=...
   ```
5. Inicie o servidor
   ```bash
   npm run dev
   ```
6. A API estará rodando em:
   ```arduino
   http://localhost:<PORT>
   ```

---

## 🔜 Funcionalidades Planejadas / a Implementar

- Autenticação de usuários (login / registro)

- Controle de permissões (usuário admin, usuário comum)

- Relatórios financeiros (gastos mensais, médias etc.)

- Paginação nas rotas de listagem

- Testes automatizados (unitários / integração)

- Documentação de API (Swagger / OpenAPI)
