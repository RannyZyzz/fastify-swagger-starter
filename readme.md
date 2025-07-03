

# 🧪 Fastify + Zod + Swagger API Boilerplate

Este é um experimento para refatorar projetos originalmente desenvolvidos com **Express** para utilizar o **Fastify**, ganhando mais performance e uma integração elegante com **Swagger** para geração automática de documentação da API.

## 🚀 Tecnologias Utilizadas

- [Fastify](https://www.fastify.io/) — Framework web focado em performance
- [Zod](https://zod.dev/) — Validador de esquemas para entrada e saída de dados
- [fastify-type-provider-zod](https://github.com/fastify/fastify-type-provider-zod) — Integração entre Fastify e Zod
- [Swagger](https://swagger.io/) via `@fastify/swagger` e `@fastify/swagger-ui`

## 📚 Funcionalidades

- 🚀 Endpoints com tipagem forte usando Zod
- 📄 Documentação automática com Swagger/OpenAPI
- 🔒 Validação e serialização de dados automáticas
- 🧪 Estrutura simples e pronta para expandir

## 🛠️ Como rodar localmente

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/nome-do-repositorio.git
   cd nome-do-repositorio
    ```

2. Instale as dependências:

   ```bash
   npm install
   ```

3. Inicie o servidor de desenvolvimento:

   ```bash
    npm run dev
   ```

4. Acesse a aplicação:

   * API: [http://localhost:3333](http://localhost:3333)
   * Documentação Swagger: [http://localhost:3333/docs](http://localhost:3333/docs)

## 🧪 Endpoints disponíveis

### `GET /users`

Retorna todos os usuários cadastrados.

**Resposta:**

```json
[
  {
    "id": "uuid",
    "name": "Nome do usuário",
    "email": "email@exemplo.com"
  }
]
```

### `POST /users`

Cria um novo usuário.

**Requisição:**

```json
{
  "name": "Nome do usuário",
  "email": "email@exemplo.com"
}
```

**Resposta:** `201 Created`

## 📁 Estrutura do projeto

```
├── src/
│   ├── server.ts         # Inicialização do Fastify e Swagger
│   ├── routes.ts         # Definição de rotas da API
│   └── types.ts          # Tipagem para instância do Fastify com Zod
```

## 🧭 Objetivo

Esse projeto serve como base para futuras refatorações, substituindo o Express por Fastify com uma estrutura moderna e escalável, mantendo a clareza na documentação da API e a segurança na validação de dados.

---

Sinta-se livre para contribuir ou usar este projeto como base para suas próprias aplicações Fastify!


