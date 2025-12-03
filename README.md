# Portal de Notícias Dinâmico — PBE 
### 👤 Identificação
Nome: Isadora Moraes
<br>
Unidade Curricular: Programação Back-End (PBE)

---- 

### 📝 Descrição do Projeto
O Portal de Notícias Dinâmico é uma aplicação desenvolvida em Node.js + Express que transforma um site estático criado na UC de LIMA em um portal totalmente dinâmico, consumindo dados reais da NewsAPI.
O sistema exibe automaticamente:
- As manchetes do Brasil
- Ou resultados de busca personalizados
<br>
A ideia principal é demonstrar integração com APIs reais, renderização dinâmica com EJS, além do uso de variáveis de ambiente para manter a segurança da API Key.


### 📂 Estrutura do Projeto
```bash
   📁 public/
    │   ├── css/
    │   │    └── style.css
    │   └── img/
    │        └── padrao.jpg
    📁 views/
    │   └── index.ejs
    📄 .env
    📄 .gitignore
    📄 app.js
    📄 package.json
   ```

O arquivo .env e a pasta node_modules são ignorados no versionamento, conforme boas práticas.

---- 

### 🚀 Como Rodar o Projeto
#### 1️⃣ Instale as dependências
```bash
npm install
```
#### 2️⃣ Crie o arquivo .env
```bash
API_KEY=sua_chave_aqui
PORT=3000
```
#### 3️⃣ Inicie o servidor
```bash
npm start
```
#### 4️⃣ Acesse no navegador
```bash
http://localhost:3000
```
---
### 🔍 Como o Projeto Funciona

O servidor tem apenas uma rota principal:

#### ✔ /
- Se não tiver busca → mostra manchetes do Brasil
- Se tiver busca (/?q=tecnologia) → usa o endpoint global everything

#### ✔ Lógica do EJS
Cada notícia é renderizada automaticamente:
- Se tiver imagem da API → mostra
- Se não tiver → usa padrao.jpg
- Se não tiver descrição → mostra "Sem descrição disponível."

#### ✔ Busca funcional
A barra de busca envia q= via GET usando:
```bash
<form action="/" method="GET">
    <input type="text" name="q" placeholder="Buscar notícias...">
    <button type="submit">Pesquisar</button>
</form>
```
### 🌐 Tecnologias Utilizadas
<p align="left">
    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/github/github-original.svg" width="40" height="40"/>
    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/html5/html5-original.svg" width="40" height="40" />
    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/axios/axios-plain-wordmark.svg" width="40" height="40"/>
    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/javascript/javascript-original.svg" width="40" height="40"/>
    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/vscode/vscode-original.svg" width="40" height="40"/>
    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/nodejs/nodejs-original.svg" width="40" height="40"/>
    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/express/express-original-wordmark.svg" width="40" height="40"/>
    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/css3/css3-original-wordmark.svg" width="40" height="40"/> 
</p>


