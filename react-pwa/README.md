# Esse projeto foi construido com [Create React App](https://github.com/facebook/create-react-app).

## Como foi criado

Primeiro instale o create-react-app globalmente:
`npm i create-react-app -g`

Crie o projeto com:
`create-react-app react-pwa`

Instale o http-server:
`npm i http-server -D`

Crie um novo script em seu package.json:

```json
"scripts": {
        "start": "react-scripts start",
        "build": "react-scripts build",
        "test": "react-scripts test",
        "eject": "react-scripts eject",
        "start-sw": "http-server ./build"
  },
```

Crie a pasta build:
`npm run build`

Suba a aplicação na porta 8080 
`npm run start-sw`

Agora é só verificar o funcionamento do service work nas ferramentas de desenvolvedor de seu browser 😃
