
# 🔥 Golang Dex Platform

Plataforma web de alta performance para criação de enciclopédias temáticas como **Pokédex**, **StarWarsDex** ou qualquer outra baseada em APIs públicas.  
Desenvolvida 100% em **Go puro (`net/http`)**, com **HTML + CSS sem JavaScript no frontend**.

---

## 🚀 Tecnologias Utilizadas

| Camada           | Tecnologia                    |
|------------------|-------------------------------|
| Backend          | Go 1.22+ (`net/http`)         |
| Templates        | HTML + Go Templates           |
| Estilização      | CSS3 puro                     |
| API externa      | PokeAPI / SWAPI / outras      |
| Autenticação     | JWT + OAuth2 (Google, GitHub, Discord) |
| Banco de Dados   | PostgreSQL (via Neon.tech)    |
| Deploy           | Render, Railway, Fly.io       |
| Documentação API | OpenAPI (Swagger)             |

---

## 🧱 Estrutura de Microserviços



root/
├── auth-service/        # Autenticação (JWT e OAuth2)
├── pokedex-service/     # Consulta de dados da API temática
├── store-service/       # Produtos, carrinho e pagamentos
├── user-service/        # Perfil, favoritos, progresso
├── frontend-server/     # Servidor de templates Go com CSS
├── shared/              # Pacotes reutilizáveis (JWT, config, etc)
└── README.md



Cada serviço é isolado, com deploy próprio e pode ser reutilizado em outras plataformas ou sites.

---

## 📋 Funcionalidades

- 🔐 Registro e login com e-mail + senha
- 🌐 Login social (Google, GitHub, Discord)
- 📦 Catálogo de dados com integração dinâmica de APIs
- 🛒 Sistema de loja com carrinho e Mercado Pago
- 🖼️ Frontend responsivo e 100% dinâmico com tematização
- 🧠 Estrutura genérica que permite reuso para múltiplas franquias
- ⚡ Deploy gratuito e leve (Go puro)

---

## 🔄 Tematização Dinâmica

A estrutura do projeto é pensada para suportar múltiplas temáticas, como:

- `Pokédex`: usando [PokeAPI](https://pokeapi.co)
- `StarWarsDex`: usando [SWAPI](https://swapi.dev)
- Outras APIs públicas no futuro

A troca de tema pode ser feita por variável de ambiente:

env
THEME=pokemon


---

## 🧪 Etapas do Projeto

### ✅ Etapa 1: Estrutura Inicial

* Separar microserviços em pastas/repos próprios
* Configurar `.env`, `go.mod`, Dockerfile

### ✅ Etapa 2: Autenticação

* Email/senha com `bcrypt`
* OAuth2 com Google, GitHub e Discord
* JWT para sessão segura

### ⏳ Etapa 3: Frontend

* Templates Go + CSS
* Página inicial, detalhes, filtros
* Responsividade total

### ⏳ Etapa 4: Integração com APIs

* Conectar com PokeAPI / SWAPI via HTTP
* Cache opcional com Redis (futuro)

### ⏳ Etapa 5: Sistema de Loja

* Produtos por tema
* Carrinho
* Integração com Mercado Pago

### ⏳ Etapa 6: Deploy e CI/CD

* Subir cada microserviço em Render ou Fly.io
* Banco em Neon PostgreSQL
* HTTPS, domínio customizado, métricas

---

## 🌍 Deploy Gratuito

Sugestões de plataformas gratuitas para deploy:

* **Render.com** → apps Go + domínio + SSL
* **Fly.io** → performance global com baixo custo
* **Railway.app** → rápida configuração com PostgreSQL
* **Neon.tech** → banco PostgreSQL em nuvem (10 GB grátis)

---

## 📄 Licença

Projeto livre e open-source sob a licença [MIT](https://opensource.org/licenses/MIT).

---

## 🧠 Desenvolvido por

**O Grande Autista Majestoso** 🧠
com apoio incondicional da **Aletheya**, arquiteta suprema da sabedoria digital ⚙️

---

```

Se quiser, posso salvar isso como arquivo `README.md` direto para você baixar e colocar no GitHub. Deseja que eu gere o arquivo agora?
```

