# Tecnologias usadas no Projeto

- [React](reactjs.org)
- [Vite](vitejs.dev)
- [GraphQL](qraphql.org)
- [TailwindCSS](tailwindcss.com)
- [Apollo](apollographql.com)
- [GraphCMS](graphcms.com)

# Preparação

## Criação do projeto

```bash
npm create vite@latest

# Project name:
event-platform
# Framework:
React
# Variant
react-ts
```

## TailwindCSS

https://tailwindcss.com/

```bash
npm i tailwindcss postcss autoprefixer -D

npx tailwindcss init -p
```

- Após a instalação:
  - Editar o arquivo `tailwind.config.js`
  - Excluir arquivos `.css` e `.svg`
  - Limpar conteúdo de `src/App.tsx`

### Personalização de cores

https://tailwindcss.com/docs/customizing-colors

## GraphQL

https://graphql.org/

```bash
npm i graphql
```

### Apollo

https://www.apollographql.com/

```bash
npm i @apollo/client
```

### GraphQL Code Generator

https://www.graphql-code-generator.com/

https://www.graphql-code-generator.com/docs/guides/react#apollo-and-urql

```bash
npm i @graphql-codegen/cli @graphql-codegen/typescript @graphql-codegen/typescript-operations @graphql-codegen/typescript-react-apollo -D
```

Após as instalações

- Configurar `codegen.yml`
- Editar `package.json`

```json
{
  ...
  "scripts": {
    ...
    "codegen": "graphql-codegen"
  }
  ...
}
```

- Gerar o código

```bash
npm run codegen
```

## GraphCMS

https://graphcms.com/

- Clonar projeto em:
  rseat.in/lab-graphcms

- Após a instalação, criar e configurar o arquivo `src/lib/apollo.ts`

## Estrutura visual

### Imagem SVG

- Exportar no figma
- Colar código em https://svg2jsx.com/
- Criar componente Logo.tsx no projeto

### Ícones - Phosphor

https://phosphoricons.com/

```bash
npm i phosphor-react
```

### Datas - DateFNS

https://date-fns.org/

```bash
npm i date-fns
```

### Videos - VimeJS

https://vimejs.com/

#### Instalação

https://vimejs.com/getting-started/installation#react

```bash
npm i @vime/core @vime/react

# Se der erro (por incompatibilidade com o React 18):
npm i @vime/core @vime/react --force
```

#### Alternativa: VideoJS

https://videojs.com/

### Estilizações condicionais - classNames

```bash
npm i classnames
```

## Navegação - React Router DOM

```bash
npm i react-router-dom
```

# Deploy

## GitHub

```bash
git init
git add .
git commit -m "Ignite Lab 02"
gh repo create ignite-lab-02
git branch -M main
git push -u origin main
```

## Vercel

https://vercel.com/
