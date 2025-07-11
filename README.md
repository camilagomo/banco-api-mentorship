# Validações em APIs - Mentoria 2.0 - Julio de Lima
Objetivo



    Linguagem: JavaScript (Node.js)
    Framework de testes: Mocha
    Biblioteca de requisições HTTP: Supertest
    Biblioteca de asserções: Chai
    Relatórios de testes: Mochawesome
    Gerenciamento de variáveis de ambiente: dotenv

Estrutura de diretórios

banco-api-tests/
├── test/               # Testes organizados por funcionalidades
│   ├── login.test.js
│   └── transferencias.test.js
├── mochawesome-report/ # Diretório gerado automaticamente com o relatório HTML dos testes
├── .env                # Arquivo para configuração da variável BASE_URL
├── .gitignore
├── package.json
└── README.md

Formato do arquivo .env

Antes de rodar os testes, crie um arquivo chamado .env na raiz do projeto com o seguinte conteúdo:

BASE_URL=http://localhost:3000

Substitua http://localhost:3000 pela URL onde a API banco-api está rodando.
Comandos para execução

Instale as dependências:

npm install

Execute todos os testes:

npm test

Geração automática do relatório HTML:

    Após executar npm test, o relatório será gerado dentro da pasta mochawesome-report/.

Sugestão: para executar os testes e abrir o relatório HTML automaticamente, adicione um script no package.json:

"scripts": {
  "test:report": "npm test && open mochawesome-report/mochawesome.html"
}

(Em Windows, substitua open por start.)
Dependências utilizadas e suas documentações

    Mocha - Framework de execução de testes
    Supertest - Biblioteca para chamadas HTTP
    Chai - Biblioteca de asserções
    Mochawesome - Geração de relatórios em HTML
    dotenv - Gerenciamento de variáveis de ambiente

