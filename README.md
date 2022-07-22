# Configuração para automatizar a geração de código js a partir do Typescript

- Instalação dos pacotes necessários

```
npm install ts-node-dev --save-dev
```

- Inserindo script dev para automatizar o processo de compilação

```
ts-node-dev --inspect --transpile-only --ignore-watch node_modules --respawn src/server.ts
```

## Imagem do diagrama do projeto de API

![Imagem do diagrama](diagrama.png)
