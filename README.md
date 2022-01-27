# react_immersive



### Códigos usados

````
# Rodar projeto em dev
yarn dev

# Criação do package.json
yarn init -y

# Inicializando o next no projeto
yarn add next react react-dom

# Executar o projeto (obs: antes é necessário inserir os scripts de execução no package.json)
yarn dev

# Instalar Storybook skynexui com components desenvolvidos
yarn add @skynexui/components

# Ignorar node quando subir alterações para branch pela 1° vez
npx gitignore node

# Integrando o supabase ao projeto
yarn add @supabase/supabase-js
````



### SEO - semântica

Nesse exemplo dizemos para o componente qual é a **Tag** que será utilizada, dessa forma conseguimos manipular e trabalhar a semântica e ter um SEO com uma classificação maior.

```javascript
function Titulo(props) {
    const Tag = props.tag;
    return (
        <>
            <Tag>{props.children}</Tag>
            <style jsx>{`
            ${Tag} {
                color: red;
                font-size: 24px;
                font-weight: 600;
            }
            `}</style>
        </>
    )
}

function HomePage() {
    return (
        <div>
            <Titulo tag="h2">Boas vindas de volta!</Titulo>
            <h2>Discord - Alura Matrix</h2>
        </div>
    )
}

export default HomePage
```



### Links usados

- [projeto original](https://github.com/alura-challenges/aluracord-matrix/tree/aula03/pages)
- [projeto com Next](https://nextjs.org/docs/getting-started) Instruções de como criar uma página inicial.
  - [custom app](https://nextjs.org/docs/advanced-features/custom-app)
- [figma do projeto](https://www.figma.com/file/X5kVg1hNCajiV73ah7iyPz/Imers%C3%A3o-React---Aluracord---Matrix?node-id=0%3A1)
- [styled jsx (css)](https://github.com/vercel/styled-jsx)
- [código pronto index](https://gist.github.com/omariosouto/983909257ff37d47c6bc31dd286f6caa)
- [código pronto chat](https://gist.github.com/omariosouto/8517c711f36770b73371185e4aed92d6)
  - [código aula 4](https://github.com/alura-challenges/aluracord-matrix/blob/aula04/pages/chat.js)

- [collors](https://coolors.co/)
- [skynexui](https://github.com/skynexui/components) components storybook
- [vercel](https://vercel.com/) para publicação da aplicação na internet
- [subabase - ambiente para criação de backend](https://supabase.com/) (acesso com github)
  - [github supabase](https://github.com/supabase/supabase-js)






