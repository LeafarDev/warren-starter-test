# warren-starter-test

### Dependências:

#### Tenha instalado o [Git](https://git-scm.com/downloads), [Docker](https://docs.docker.com/engine/install/) e o [Docker Compose](https://docs.docker.com/compose/install/) na sua máquina

#

### Repositórios:

* [Front-end](https://github.com/LeafarDev/warren-client-test/blob/main/README.md)
* [Back-end](https://github.com/LeafarDev/warren-api-test/blob/main/README.md)

#
### Principais tecnologias utilizadas:

* Front-end:
    * [React.js](https://reactjs.org/)
    * [TypeScript](https://www.typescriptlang.org/)
    * [Yup](https://github.com/jquense/yup)
    * [Formik](https://formik.org/)
    * [Axios](https://github.com/axios/axios)
    * [Jest](https://jestjs.io/)
    
* Back-end:
    * [Node.js](https://nodejs.org/en/)
    * [Express.js](https://expressjs.com/)
    * [TypeOrm](https://typeorm.io/#/)
    * [TypeScript](https://www.typescriptlang.org/)
    * [Node-cron](https://github.com/kelektiv/node-cron)
    * [TypeDi](https://github.com/typestack/typedi)
    * [Jest](https://jestjs.io/)
    * [Routing-controllers](https://github.com/typestack/routing-controllers)
#
### Instalação:

#### Clone esse projeto junto com seus módulos utilizando o comando abaixo:

```git clone --recurse-submodules -j8 https://github.com/LeafarDev/warren-starter-test```

#### Dentro da pasta do repositório utilize os comandos abaixo para criar os arquivos .env

* Back-end:
    * Produção:``` cp applications/warren-api-test/.env.example applications/warren-api-test/.env ```
    * Teste:``` cp applications/warren-api-test/.env.test.example applications/warren-api-test/.env.test ```
* Front-end:
  ``` cp applications/warren-client-test/.env.example applications/warren-client-test/.env```

#### Execute o docker-compose:

```docker-compose up --build -d```

#### Após o "build" do comando anterior estiver finalizado e tudo estiver executando corretamente, execute as instruções abaixo:

##### *Se estiver executando o Docker no Windows, utilize o PowerShell

* Execute as migrations: ```docker-compose run warren-bank-api npm run typeorm migration:run```
* Execute os seeders: ```docker-compose run warren-bank-api npm run seed:run```

#

### Executando os testes:

* Back-end: ```docker-compose run warren-bank-api npm run test```
* Front-end ```docker-compose up warren-client-test```

#

### Funcionalidades:

* Depósito: Permite a inserção de dinheiro na conta do usuário logado
* Saque: Permite a retirada de dinheiro da conta do usuário logado
* Pagamento: Permite que uma conta pague uma quantia desejada para outras contas
* Rendimento Diário: Todo dia o sistema executa uma rotina que gera um rendimento de acordo com o balanço de cada conta

#

### Acesso:

* Basta acesse o client em: *http://localhost:3380/*
    * Essas sãos as contas disponíveis:
      ```
        Login: dumingaz.silva@gmail.com
        Senha: 12345678
        Conta: 65932871
      ```

      ```
        Login: charles.marciano45@gmail.com
        Senha: 12345678
        Conta: 12345678
      ```

      ```
        Login: hermes.trismegisto@gmail.com
        Senha: 12345678
        Conta: 68472358
      ```
