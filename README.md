# NLW 13ª Edição - IA
Projeto da 13ª edição do NLW da [Rocketseat](https://www.rocketseat.com.br/), onde o foco é a criação de uma aplicação que utiliza de IA para extrair informações de vídeos.

## :rocket: Começando
Abaixo é possível encontrar instruções de como obter uma cópia do projeto para fins de teste e desenvolvimento.

## :exclamation: Pré-requisitos 
Para implementar e testar o projeto localmente é necessário:  
* [NodeJS](https://nodejs.org/en) v18.17.0 ou superior.

Entre na raiz de cada uma das pastas a seguir e rode os comandos correspondentes para instalação das dependências:

| Parte       | Caminho          | Comando       |
| :---------- | :--------------- | :------------ |
| API         | `/upload-ai-api` | `npm install` |
| Web         | `/upload-ai-web` | `npm install` |

Assim, a pasta `node_modules` será criada em cada um dos diretórios.
### :gear: API
Parte do projeto responsável por implementar a camada de comunicação com o banco de dados, que nesse projeto é o [SQLite](https://www.sqlite.org/index.html), usando o [Prisma ORM](https://www.prisma.io/).

### Execução
```bash
  npm run dev
```

### Endpoints

***_Upload do vídeo:_***
```http
  POST /videos
```
| Parâmetro   | Tipo       | Descrição                           |
| :---------- | :--------- | :---------------------------------- |
| `video`     | `file`     | **obrig.** Vídeo para upload        |

--------------

### :desktop_computer: Aplicação Web

Parte do projeto por implementar uma das camadas de interação do usuário com os requisitos do projeto. Foi criado usando [React](https://react.dev/) com [Vite](https://vitejs.dev/) e [TailwindCSS](https://tailwindcss.com/).

### Execução
```bash
  npm run dev
```

Permite o usuário:
* Realizar o upload de um vídeo e obter a transcrição do mesmo para texto;
* Utilizar templates anteriormente cadastrados para instruir a IA a fazer aquilo que ele desejar com a transcrição.