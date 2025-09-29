# API CRUD - CODE QUEENS

<p align="center">
   <img src="https://img.shields.io/static/v1?label=STATUS&message=CONCLUIDO&color=RED&style=for-the-badge" alt="status"/>
</p>

Uma API RESTful simples para gerenciar informações de pessoas, desenvolvida com Node.js e Express para fins educacionais.

## Sobre o Projeto

Este projeto demonstra os conceitos fundamentais de desenvolvimento de APIs, incluindo operações CRUD (Create, Read, Update, Delete) e os principais métodos HTTP. É ideal para quem está começando a aprender sobre desenvolvimento backend. O objeto desse repositório é para promover um ambiente de estudo documentado para as alunas CodeQueens, projeto da UNIVALI.

## Conceitos Abordados

### 🔗 API (Application Programming Interface)

Uma API é como um "garçom" em um restaurante que faz a comunicação entre você (cliente) e a cozinha (servidor). Ela recebe seus pedidos, processa e retorna as respostas.

### 📍 Endpoint

É o endereço específico onde você faz suas requisições. Como o endereço de uma casa, cada endpoint tem uma função específica.

- Exemplo: `http://localhost:3000/pessoas`

### 🛤️ Rota

É o caminho que define qual função será executada quando alguém acessa um endpoint específico.

- Exemplo: `/pessoas` → função que retorna todas as pessoas

### 📝 CRUD

As 4 operações básicas para manipular dados:

- **C**reate (Criar) → POST
- **R**ead (Ler) → GET
- **U**pdate (Atualizar) → PUT
- **D**elete (Deletar) → DELETE

## Funcionalidades

- Listar todas as pessoas
- Buscar pessoa por ID
- Criar nova pessoa
- Atualizar dados de uma pessoa
- Contar total de pessoas

## Tecnologias Utilizadas

- **Node.js** - Runtime JavaScript
- **Express.js** - Framework web para Node.js
- **JavaScript** - Linguagem de programação

## Instalação e Execução

### Pré-requisitos

- Node.js instalado em sua máquina
- npm (geralmente vem com Node.js)

### Passos para executar:

1. **Clone o repositório**

```bash
   git clone https://github.com/GabriellyOlinsc/itens-codequeens.git
   cd itens-codequeens
```

2. **Instale as dependências**

```bash
    npm install express
    npm install path
```

3. **Execute o servidor**

```bash
    node index.js
```

4. **Acesse a API**

```bash
   Servidor rodando em: http://localhost:3000
```

##  Endpoints Disponíveis

| Método | Endpoint        | Descrição               | Exemplo de Uso      |
| ------ | --------------- | ----------------------- | ------------------- |
| `GET`  | `/`             | Exibe página login.html | `GET /`             |
| `GET`  | `/itens.html`   | Exibe página itens.html | `GET /itens.html`   |
| `GET`  | `/pessoas`      | Listar todas as pessoas | `GET /pessoas`      |
| `POST` | `/pessoas`      | Criar nova pessoa       | `POST /pessoas`     |
| `PUT`  | `/pessoa/:id`   | Atualizar pessoa        | `PUT /pessoa/1`     |

##  Exemplos de Uso

### 1. Listar todas as pessoas

```bash
    GET http://localhost:3000/pessoas
```

### 2. Criar nova pessoa
```bash
    POST http://localhost:3000/pessoa

    no body:

    {
        "nome": "Maria",
        "idade": 15
    }
```

## Estrutura do projeto

```
itens-codequeens/
│
├── public/
|   ├── login.html    # tela de login.html
|   ├── itens.html    # tela de itens.html 
├── index.js          # Arquivo principal da aplicação
├── package.json      # Dependências e scripts do projeto
└── README.md         # Documentação do projeto
```
