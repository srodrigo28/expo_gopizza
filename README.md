# Projeto Expo GoPizza

### by Rockeatset
```
https://app.rocketseat.com.br/node/app-de-pedido-de-pizzas-2022/group/estrutura-do-projeto-1640096678756/lesson/1640096678754-adicionando-typescript
```

* Criando o projeto 
```
expo init gopizza
```

* Entrar na pasta do projeto
```
cd go pizza
```

* Criar o arquivo tsconfig.json em branco
```
expo start
```

* Auxiliar de diretório
```
babel-plugin-module-resolver -D
```

* babel.config.json


* Configurar tsconfig.json
```
{
  "extends": "expo/tsconfig.base",
  "compilerOptions": {
    "strict": true,
    "baseUrl": "/",
    "paths": {
      "@src/*": [ "./src/*"],
      "@assets/*": ["./src/assets/*"],
      "@components/*": ["./src/components/*"],
      "@screens/*": ["./src/screens/*"],
    }
  },
}
```
