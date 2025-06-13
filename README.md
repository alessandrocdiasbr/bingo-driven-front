# Bingo Driven - Front-end

Este é o projeto front-end para o sistema de Bingo Driven, desenvolvido com React e Vite.

## 🚀 Deploy

A aplicação está no ar e pode ser acessada através do link:

- **Aplicação:** `https://bingo-driven-front.vercel.app`

A API do back-end consumida por este projeto está disponível em:

- **API:** `https://bingo-driven-backend-sk9a.onrender.com`

---

## ⚙️ Tecnologias

- [cite_start]**Core:** React e Vite. 
- **Estilização:** CSS puro.
- [cite_start]**Roteamento:** React Router DOM. 
- [cite_start]**Requisições HTTP:** Axios. 
- **DevOps:** Docker, Docker Compose, GitHub Actions, Vercel.

---

## 💻 Executando Localmente com Docker

As instruções para executar a aplicação completa (front-end + back-end) com Docker Compose estão no repositório do back-end.

Se desejar subir apenas o contêiner do front-end:

1.  Crie um arquivo `.env` na raiz do projeto com a URL do back-end:
    ```
    VITE_BACKEND=http://localhost:5000
    ```

2.  Construa a imagem Docker:
    ```bash
    docker build -t bingo-frontend .
    ```

3.  Execute o contêiner:
    ```bash
    docker run -p 8080:80 --name bingo-ui bingo-frontend
    ```

4.  Acesse `http://localhost:8080` no seu navegador.

---

## 🛠️ Desenvolvimento (Sem Docker)

- [cite_start]Instalar as dependências com o `npm i`; 
- [cite_start]Criar o arquivo `.env` com base no exemplo do `.env.example`, apontando para a API do back-end;
- Executar o comando `npm run dev`.