# Cypress Web Test Automation Project 🚀

Este projeto utiliza **Cypress** para automação de testes web, garantindo confiabilidade e escalabilidade para aplicações modernas.

---

## 📂 Estrutura do Projeto  

phpt-travel-automation/
├── cypress/
│   ├── e2e/                     # Pasta para os testes de ponta a ponta
│   │   ├── tests/               # Testes automatizados
│   │   │   ├── login.cy.js      # Exemplo de teste de login
│   │   │   ├── search.cy.js     # Exemplo de teste de busca
│   │   └── features/            # Features para BDD (se necessário)
│   ├── fixtures/                # Dados estáticos para os testes (JSONs)
│   │   └── userCredentials.json # Exemplo de credenciais para login
│   ├── support/                 # Suporte e customizações
│   │   ├── commands.js          # Comandos customizados do Cypress
│   │   ├── e2e.js               # Configurações gerais do Cypress
│   │   └── page_objects/        # Objetos de página (POM)
│   │       ├── loginPage.js     # Página de Login
│   │       ├── searchPage.js    # Página de Busca
│   │       └── homePage.js      # Página Principal
│   └── videos/                  # Gravações de testes (ignoradas no Git)
│   └── screenshots/             # Capturas de tela de falhas (ignoradas no Git)
├── .github/
│   └── workflows/
│       └── cypress.yml          # Configuração do GitHub Actions para CI
├── node_modules/                # Dependências (ignorado no Git)
├── .gitignore                   # Arquivos e pastas a serem ignorados
├── cypress.config.js            # Configuração principal do Cypress
├── package.json                 # Dependências do Node.js
├── README.md                    # Documentação do projeto



---

## 🛠️ Pré-requisitos

Certifique-se de ter as seguintes ferramentas instaladas:
- [Node.js](https://nodejs.org/) (>= 16)
- [NPM](https://www.npmjs.com/) ou [Yarn](https://yarnpkg.com/)

---

## 🚀 Como executar

1️⃣ Instalar dependências:
```bash
npm install  
# ou  
yarn install  

npx cypress open  
# ou  
yarn cypress open  

npx cypress run  
# ou  
yarn cypress run  

const { defineConfig } = require('cypress');

module.exports = defineConfig({
  e2e: {
    baseUrl: 'https://sua-aplicacao.com',
    viewportWidth: 1280,
    viewportHeight: 720,
    retries: 2, // Tenta novamente em caso de falha
  },
});
