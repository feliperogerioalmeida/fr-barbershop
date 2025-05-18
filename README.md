# FR Barbershop

> Site institucional e landing page para a barbearia **FR Barbershop**, construído com Next.js, TypeScript e Tailwind CSS.

🔗 **Demo:** https://fsw-barber-navy.vercel.app

---

## Índice

- [Sobre](#sobre)
- [Tecnologias](#tecnologias)
- [Pré-requisitos](#pré-requisitos)
- [Instalação e execução](#instalação-e-execução)
- [Variáveis de ambiente](#variáveis-de-ambiente)
- [Contribuição](#contribuição)
- [Fotos](#fotos)
- [Licença](#licença)

---

## Sobre

Este repositório contém o código-fonte do site da **FR Barbershop**, com design responsivo e identidade visual forte. Por enquanto, apenas a versão mobile está disponível; a versão desktop está em desenvolvimento.

O projeto utiliza a App Router do Next.js 13, integrações com Prisma para modelagem de dados e está pronto para deploy via Vercel ou Docker

---

## Tecnologias

- **Framework**: [Next.js 13](https://nextjs.org/) (App Router)
- **Linguagem**: TypeScript
- **Estilização**: Tailwind CSS
- **Banco de dados**: Prisma ORM (SQLite / PostgreSQL — via `DATABASE_URL`)
- **Qualidade de código**: ESLint, Prettier, Husky (Git hooks)
- **Containerização**: Docker & Docker Compose

---

## Pré-requisitos

- **Node.js** v16 ou superior
- **npm** ou **yarn**
- (Opcional) **Docker** e **Docker Compose** para execução containerizada

---

## Instalação e execução

1. **Clone o repositório**
   ```bash
   git clone https://github.com/feliperogerioalmeida/fr-barbershop.git
   cd fr-barbershop
   ```
2. Instale as dependências

   ```
   npm install
   # ou
   yarn install
   ```

3. Configure as variáveis de ambiente

   - Duplique o arquivo .env.example para .env

   - Preencha a variável DATABASE_URL com a sua string de conexão

4. Configure o banco de dados

   ```
   npx prisma migrate dev --name init
   ```

5. Inicie em modo de desenvolvimento

   ```
    npm run dev
    # ou
    yarn dev
   ```

6. Build e start (produção)

   ```
   npm run build
   npm start
   ```

7. (Opcional) Com Docker Compose
   ```
   docker-compose up --build
   ```

## Variáveis de ambiente

    DATABASE_URL="postgresql://usuario:senha@localhost:5432/fr-barbershop
    GOOGLE_CLIENT_ID= "id-google"
    GOOGLE_CLIENT_SECRET= "segredo-do-cliente-google"
    NEXT_AUTH_SECRET= "segredo-qualquer"

## Contribuição

1. Faça um fork deste repositório
2. Crie uma branch com a sua feature: git checkout -b feature/nome-da-feature
3. Faça commit das suas alterações: git commit -m 'feat: descrição da feature'
4. Push para a sua branch: git push origin feature/nome-da-feature
5. Abra um Pull Request

## Fotos

<p align="center">
 
  <img src="./public/examples/home.png" alt="home" width="600"/>
</p>

<p align="center">
 
  <img src="./public/examples/sidebar.png" alt="sidebar" width="600"/>
</p>

<p align="center">
 
  <img src="./public/examples/agendametos.png" alt="agendamentos" width="600"/>
</p>
<p align="center">
 
  <img src="./public/examples/barbearias.png" alt="barbearias" width="600"/>
</p>
<p align="center">
 
  <img src="./public/examples/servico.png" alt="servico" width="600"/>
</p>
<p align="center">
 
  <img src="./public/examples/agendamento.png" alt="agendamento" width="600"/>
</p>
<p align="center">
 
  <img src="./public/examples/agendamentos2.png" alt="agendamentos" width="600"/>
</p>

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.
