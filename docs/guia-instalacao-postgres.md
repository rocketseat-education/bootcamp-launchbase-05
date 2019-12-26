# PostgresSQL

O banco de dados que iremos usar é o PostgresSQL.

É um banco de dados relacional, com código aberto e um dos mais avançados.


## NodeJS

Para usar postgres no seu projeto NodeJS adicione a dependencia ao seu projeto

```shell
npm install pg
```

## Mac

```shell
brew install postgres
```

### Iniciar o postgres

```shell
pg_ctl -D /usr/local/var/postgres start
```

### Desligar o postgres

```shell
pg_ctl -D /usr/local/var/postgres stop
```

## Windows

Para instalar o postgres no windows, você pode baixar o instalador no site abaixo, ou seguir o passo-a-passo para instalar com o `chocolatey`

**Baixar do site oficial**
- https://www.enterprisedb.com/downloads/postgres-postgresql-downloads

**Chocolatey**

```bash
cinst postgresql12 --params '/Password:postgres' -y
```

*Esse processo vai demorar um bocado. Nos meus testes, cerca de 20 minutos, mas depende da sua máquina e da sua conexão com a internet.*

Quando chegar numa tela parecida com essa, provavelmente estará na **metade do caminho.**

![Metade Da Instalação](https://i.imgur.com/PqLBWYy.png)

Caso fique tudo travado por mais de 20 minutos ou dê erros, procure entrar na pasta `C:\Program Files\PostgreSQL\12`, caso seu Windows seja 32 bits ou `C:\Program Files (x86)\PostgreSQL\12`, caso seu Windows seja 64 bits.

*Perceba que a versão que estou usando para criar esse tutorial, é a versão 12. Caso a sua versão instalada seja outra, atente-se ao número da versão na pasta acima. Troque o 12 pela versão do seu postgres.*

![Image](https://media.discordapp.net/attachments/616282793625911332/646795822859550721/unknown.png)

Caso haja os arquivos, então sua instação deu certo. Se não deu certo, você pode tentar novamente o processo, ou, baixar direto do site do fabricante e instalar o pacote.

### Ligar o Postgres

1. Abra o Powershell como administrador, e navegue até a pasta da instação

```bash
cd "C:\Program Files\PostgreSQL\12\bin\"
```

2. Inicie o postgres com o comando abaixo:

```bash
.\pg_ctl.exe -D "C:\Program Files\PostgreSQL\12\data" start
```

*Note que o -D tem que ser maiúsculo para que o comando seja executado perfeitamente.*

**Desligar o Postgres**

Use o passo número 1 acima e digite o comando para desligar

```bash
.\pg_ctl.exe -D "C:\Program Files\PostgreSQL\12\data" stop
```

## Linux

[Documentação Oficial de Instalação do Postgres](https://www.postgresql.org/download/linux/)

# Postbird

É um aplicativo multi plataforma que vai te permitir usar o PostgresSQL com uma interface gráfica, para fazer as operações no banco de dados.

Para instalar, vá até o site: https://electronjs.org/apps/postbird e baixe o app.
