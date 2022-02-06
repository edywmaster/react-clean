# React Clean 2022

Este é um modelo de projeto limpo, para iniciar novos projetos React utilizando Next e Typescript em 2022.

## Como esse projeto foi criado

Primeiro passo, iniciando um novo projeto com npm:

```bash
npx create-next-app react-clean --use-npm
```
Excluir arquivos e pastas:

- Excluir todos os arquivos da pasta `public`;
- Excluir pasta API dentro da pasta pages. Ex.: `pages/API`;

Adicionar Typescript:

```bash
npm install --save @types/react @types/node
```
Renomear arquivos para .tsx:

- _app.js para _app.tsx;
- index.js para index.tsx;

Limpar todos os conteudos e remover importações desnecessarias em _app.tsx e index.tsx

Rodar projeto para reconhecer typescript e criar arquivos nescessarios:

```bash
npm run dev
```
Arquivos criados após comando:

- next-env.d.ts
- tsconfig.json

Instalar eslint como dependencia de desenvolvimento:

```bash
npm install eslint --save-dev
```
Configurar eslint:

```bash
npx eslint --init
```
Selecionar as seguintes opções de configuração:

- To check syntax, find problems, and enforce code style
- JavaScript modules (import/export)
- React
- Does your project use TypeScript? » Yes
- Where does your code run » Browser e Node
- Use a popular style guide » Standard
- What format do you want your config file to be in? » JSON
- Do you want to downgrade? » Yes
-  Would you like to install them now with npm? » Yes

Configurar vscode para corrigir o código em autosave usando eslint:

"editor.codeActionsOnSave": {
    "source.fixAll.eslint": true,
},

Adicionar a extenção editconfig:

- Instalar extenção editconfig;
- Criar arquivo de configuração;

Instalar o Prettier e plugns para eslint:

```bash
npm install --save-dev prettier eslint-plugin-prettier eslint-config-prettier
```

Configurar o eslint no arquivo `.eslintrc.json`
Criar arquivo ignore do eslint `.eslintignore`
Criar de configuração do prettier `prettier.config.js`

