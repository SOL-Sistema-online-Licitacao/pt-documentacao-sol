# Instalação da API

### Preparando o ambiente

É necessário fazer a instalação de algumas ferramentas. Clique nos links abaixo para fazer a incitação de cada uma delas.

[![YARN](https://img.shields.io/badge/Yarn-2C8EBB.svg?style=for-the-badge\&logo=Yarn\&logoColor=white)](https://yarnpkg.com/cli/install)[![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge\&logo=docker\&logoColor=white)](https://docs.docker.com/compose/install/#install-compose)[![NodeJS](https://img.shields.io/badge/node.js-%2343853D.svg?style=for-the-badge\&logo=node.js\&logoColor=white)](https://nodejs.org/en/)[![PM2](https://img.shields.io/badge/PM2-2B037A.svg?style=for-the-badge\&logo=PM2\&logoColor=white)](https://www.npmjs.com/package/pm2)

### Configurando o arquivo do ambiente (.env)

Acesse o diretório raiz da API e execute o comando abaixo:

```
λ docker-compose up -d
```

Crie um arquivo `prod.env` na pasta `/env` da API com o seguinte formato:

```
PORT=4002
NOSQL_CONNECTION_STRING=mongodb://localhost:20000/lacchain
JWT_KEY=secret_KEY
JWT_REFRESH_TOKEN_KEY=****************==
JWT_ACCESS_TOKEN_EXPIRATION=8h
JWT_REFRESH_TOKEN_EXPIRATION=7d
ENCRYPT_KEY=********-****-****-****-************
SENDGRID_EMAIL_SENDER=email@email.com
SENDGRID_API_KEY=******************

AWS_REGION=us-east-1
AWS_ACCESS_KEY_ID=******************
AWS_SECRET_ACCESS_KEY=**********/********/****

S3_BUCKET=dev-sol-app-api
S3_BUCKET_DOCUMENTS=dev-sol-app-api
S3_BUCKET_ANNOUNCEMENT_PHOTO=dev-sol-app-api                                    
```

Descrição dos parâmetros do arquivo env:&#x20;

<table><thead><tr><th width="378">Descrição</th><th>Parâmetro</th></tr></thead><tbody><tr><td>PORT</td><td>Porta em que a API será iniciada</td></tr><tr><td>NOSQL_CONNECTION_STRING</td><td>String de conexão com a base de dados, aqui deve ser adicionado o caminho publicado pelo docker compose.</td></tr><tr><td>JWT_KEY</td><td>Chave utilizada para a criptografia JWT</td></tr><tr><td>JWT_REFRESH_TOKEN_KEY</td><td>Chave utilizada para verificar a autenticidade dos Tokens de atualização JWT</td></tr><tr><td>JWT_ACCESS_TOKEN_EXPIRATION</td><td>Tempo de expiração do Token JWT</td></tr><tr><td>JWT_REFRESH_TOKEN_EXPIRATION</td><td>Tempo de expiração do Token de atualização JWT</td></tr><tr><td>ENCRYPT_KEY</td><td>Chave utilizada para a criptografia do Payload. Deve ser gerada pelo usuário e o mesmo deve estar de acordo com o frontend.</td></tr><tr><td>SENDGRID_EMAIL_SENDER</td><td>Email de origem para os serviços SendGrid</td></tr><tr><td>SENDGRID_API_KEY</td><td>Chave utilizada para autenticar e autorizar o acesso aos recursos do serviço SendGrid</td></tr><tr><td>AWS_REGION</td><td>Região do servidor AWS (Nulo caso não utilize AWS)</td></tr><tr><td>AWS_ACCESS_KEY_ID</td><td>Chave de acesso da AWS</td></tr><tr><td>AWS_SECRET_ACCESS_KEY</td><td>Autenticador de acesso para serviços AWS</td></tr><tr><td>S3_BUCKET</td><td>Bucket de armazenamento da AWS (Opcional, podendo utilizar outro bucket)</td></tr><tr><td>S3_BUCKET_DOCUMENTS</td><td>Bucket de armazenamento da AWS (Opcional, podendo utilizar outro bucket)</td></tr><tr><td>S3_BUCKET_ANNOUNCEMENT_PHOTO</td><td>Bucket de armazenamento da AWS (Opcional, podendo utilizar outro bucket)</td></tr></tbody></table>

### Publicando a API

Acesse o diretório raiz da API e execute o comando abaixo:

```
λ yarn publish:prod
```

O Yarn criará um pacote contendo todo o código-fonte do pacote, juntamente com o arquivo "package.json" atualizado com a versão.

### Instalar o PM2 no servidor

&#x20;Documentação PM2:&#x20;

[https://pm2.keymetrics.io/docs/usage/pm2-doc-single-page/](https://pm2.keymetrics.io/docs/usage/pm2-doc-single-page/)

Execute o comando:

```
λ npm install pm2@latest -g
```

#### Executando o PM2

Execute o comando:

```
λ pm2 start npm --name "sol-api-dev" -- run "start:dev"
```

### Executar o seed

O seed cria o usuário administrativo e uma associação.

```
λ yarn run seed
```
