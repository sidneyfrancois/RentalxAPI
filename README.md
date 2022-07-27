# Configuração para automatizar a geração de código js a partir do Typescript

- Instalação dos pacotes necessários

```
npm install ts-node-dev --save-dev
npm install uuid
npm install @types/uuid --save-dev
npm install multer
npm install @types/multer --save-dev
npm install csv-parse
```

- Inserindo script dev para automatizar o processo de compilação

```
ts-node-dev --inspect --transpile-only --ignore-watch node_modules --respawn src/server.ts
```

## Imagem do diagrama do projeto de API

![Imagem do diagrama](diagrama.png)
