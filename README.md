<h1 align="center">
  ReadFileCSV
</h1>

<p align="center">
  <img src="https://img.shields.io/static/v1?label=ReadFileCSV&message=1.0&color=#43853d&labelColor=000000" alt="Upfi" />

  <img src="https://img.shields.io/github/stars/alexandresantosm/read-file-csv?label=stars&message=MIT&color=#43853d&labelColor=000000" alt="Stars" />

  <img  src="https://img.shields.io/static/v1?label=license&message=MIT&color=#43853d&labelColor=000000" alt="License">
</p>

<br>

## 🧪 Tecnologias

A aplicação desenvolvida utiliza as seguintes tecnologias:

- [Node.js](https://nodejs.org/en/)
- [TypeScript](https://www.typescriptlang.org)
- [Express](http://expressjs.com/pt-br/)
- [Prisma](https://www.prisma.io/)
- [Multer](https://www.npmjs.com/package/multer)

## 🚀 Como executar

Antes de começar, você vai precisar ter instalado em sua máquina as seguintes ferramentas:
[Git](https://git-scm.com), [Node.js](https://nodejs.org/en/).
Além disto é bom ter um editor de sua preferência para trabalhar com o código como por exemplo o [VSCode](https://code.visualstudio.com/).

- Inicialização do projeto

```bash
$ git clone https://github.com/alexandresantosm/read-file-csv
$ cd read-file-csv
```

Para iniciar o projeto, siga os passos abaixo:

```bash
# Instalar as dependências necessárias do projeto
$ yarn

# Execute a aplicação em modo de desenvolvimento
$ yarn dev
```

O app estará disponível no seguinte endereço http://localhost:3000/products.

- Configuração do Prisma ORM

  - Inicializar o prisma na aplicação com o comando:

    ```bash
    yarn prisma init
    ```

- Será necessário editar o arquivo `.env` da aplicação.

  - Substitua `johndoe` pelo seu usuário do banco de bados.
  - Substitua `randompassword` pela sua senha do banco de bados.

    ```bash
    DATABASE_URL="postgresql://johndoe:randompassword@localhost:5432/codedrops?schema=public"
    ```

  - Delete a pasta `migartions` do seu projeto e execute o comando:

    ```bash
    yarn prisma migrate dev
    ```

    - O console irá solicitar um nome para sua migration. Uma sujestão é colocar `create_products`.

## 🔖 Requisitos prévios

- Ter instalado uma ferramenta para testar rotas de uma API, como por exemplo:

  - O [Insomnia](https://insomnia.rest/); ou
  - O [Postman](https://www.postman.com/).

-Ter instalado e configurado um banco de dados, por exemplo PostgreSQL, MySQL, SQLite, SQL Server ou MongoDB.

## 💻 Projeto

ReadFileCSV é uma API onde o principal objetivo é realizar a leitura e manipulação de dados de um arquivo em formato .csv.

Uma requisição feita para API enviando um arquivo com extensão .csv. Esse arquivo é interceptado pelo multer. A API, então, processa o arquivo retirando os dados necessários e salvando no banco de dados através do Prisma ORM.

## ✅ Demonstração da aplicação

<br>

<p align="center">
  <img src=".github/read_csv_console.png" alt="Demonstração do arquivo lido e impresso no terminal" />
</p>

<p align="center">
  <img src=".github/request_with_insomnia.png" alt="Demonstração de uma requisição para endpoint da API" />
</p>

<p align="center">
  <img src=".github/data_save_postgres.png" alt="Demonstração dos dados do arquivo .csv saldo no banco de dados PostgreSQL" />
</p>

## 📝 License

Esse projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE.md) para mais detalhes.

---

Feito com 💜 by Alexandre 👋🏻
