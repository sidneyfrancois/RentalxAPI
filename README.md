# Configuração para automatizar a geração de código js a partir do Typescript

- Instalação dos pacotes necessários

```
npm install ts-node-dev --save-dev
npm install uuid
npm install @types/uuid --save-dev
npm install multer
npm install @types/multer --save-dev
npm install csv-parse
npm install swagger-ui-express
npm install @types/swagger-ui-express --save-dev
```

- Inserindo script dev para automatizar o processo de compilação

```
ts-node-dev --inspect --transpile-only --ignore-watch node_modules --respawn src/server.ts
```

- Docker (Comandos para criar imagem e rodar containers)

```
docker build -t rentx .
docker run -p 3333:3333 rentx
```

- Após o Docker compose inserir a tag --poll no script dev

```
ts-node-dev --poll --inspect --transpile-only --ignore-watch node_modules --respawn src/server.ts
```

## Imagem do diagrama do projeto de API

![Imagem do diagrama](diagrama.png)
