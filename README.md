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
```
module.exports = function(api) {
  api.cache(true);
  return {
    presets: ['babel-preset-expo'],
    plugins:[
      [
        'module-resolver',
        {
          root: ['./src'],
          extensions: [
            '.ts', '.tsx', '.js',
            '.json','.css'
          ],
          alias: {
            '@components': './src/components',
            '@screens': './src/screens',
            '@assets': './src/assets',
          }
        }
      ]
    ]
  }
}
```

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

* Fontes
```
expo install @expo-google-fonts/dm-sans
```
```
expo install @expo-google-fonts/dm-serif-display
```

* Para verificar o carregamento dos modulos
```
expo install expo-app-loading@~1.2.1
```

* Styled-componnets para estilar
```
npm install styled-component
```
```
yarn add styled-components
```

* Styled-componnets typagem
```
npm install @types/styled-components-react-native -D
```