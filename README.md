# warren-starter-test

### Dependencias:

#### Tenha instalado o [Git](https://git-scm.com/downloads), [Docker](https://docs.docker.com/engine/install/) e o [Docker Compose](https://docs.docker.com/compose/install/) na sua máquina

#
###  Repositórios:
#### O detalhamento de cada projeto estão disponiveis em seus READMEs:

* [Readme do Front-end](https://github.com/LeafarDev/warren-client-test/blob/main/README.md)
* [Readme do Back-end](https://github.com/LeafarDev/warren-api-test/blob/main/README.md)

#

### Instalação:

#### Clone esse projeto junto com seus modulos utilizando o comando abaixo:

```git clone --recurse-submodules -j8 https://github.com/LeafarDev/warren-starter-test```

#### Dentro da pasta do repositório utilize os comando abaixo para criar os arquivos .env

* Back-end:
  ``` cp applications/warren-api-test/.env.example applications/warren-api-test/.env ```
* Front-end:
  ``` cp applications/warren-client-test/.env.example applications/warren-client-test/.env```

#### Execute o docker-compose:

```docker-compose up --build -d```

#### Após o "build" do comando anterior estiver finalizado e tudo estiver executando corretamente, execute as instruções abaixo:

##### *Se estiver executando o Docker no Windows, utilize o PowerShell

* Execute as migrations: ```docker-compose run warren-bank-api npm run typeorm migration:run```
* Execute os seeders: ```docker-compose run warren-bank-api npm run seed:run```

#

### Funcionalidades:

* Deposito: Permite a inserção de dinheiro na conta do usuário logado
* Saque: Permite a retirada de dinheiro da conta do usuário logado
* Pagamento: Permite que uma conta pague uma quantia desejada para outras contas
* Rendimento Diário: Todo dia o sistema executa uma rotina que gera um rendimento de acordo com o balanço
  de cada conta

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
