# Comandos úteis
```bash
nvm -v #ver a versão do Node.js instalada
nvm alias default lts/hydrogen #Set default node version on a shell
```
# Atalhos de teclado
`CTRL+L` para limpar terminal
# Versão do Node.js
Diferentes versões do Node.js podem atrapalhar o funcionamento do código. Por isso criar arquivo .nvmrc na raiz do site contendo o nome da versão do Node.js a ser usada com uma nova linha após (ex: lts/hydrogen) 
```bash
nvm install #(para instalar a versão no arquivo .nvmrc)
```
# Definir dependências com package.json
```bash
npm init #para criar o arquivo package.json
npm install next@13.1.6
npm install react@18.2.0
npm install react-dom@18.2.0
```
# Rodar servidor local
Criar atalho para ```next dev``` (servidor local) em package.json
```
"scripts": {
    "dev": "next dev"
  },
```
Criar pasta `pages` na raiz do site contendo arquivo `index.js`. Colocar os seguintes dados:
```
function Home() {
    return <h1>Hello world!</h1>
}
export default Home;
```
Executar comando `run dev` para iniciar servidor local. Clicar na antena canto inferior esquerdo para ver endereço e modifiar visibilidade para `public`. Abrir o link para ver a página (alterações são enviadas em tempo real).
