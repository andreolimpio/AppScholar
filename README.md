# AppScholar

## Sobre o projeto

O AppScholar é um sistema acadêmico desenvolvido para auxiliar no gerenciamento de informações relacionadas ao ambiente escolar.

A aplicação possui uma interface mobile desenvolvida com React Native utilizando o ambiente Expo Snack, responsável pela interação do usuário com o sistema. A comunicação com os dados é realizada por meio de uma API desenvolvida em PHP, que utiliza PDO para acessar um banco de dados MySQL.

A arquitetura da aplicação utiliza uma separação entre interface, API e banco de dados. Dessa forma, o aplicativo não acessa diretamente o MySQL. As solicitações são realizadas pelo aplicativo utilizando requisições HTTP por meio da função `fetch()`. A API PHP recebe essas requisições, executa as operações necessárias no banco de dados e retorna os resultados em formato JSON.

O sistema foi projetado para trabalhar com diferentes informações acadêmicas, incluindo alunos, professores, cursos, disciplinas, turmas, matrículas, responsáveis, avaliações, coordenadores e boletins.

A estrutura geral de comunicação do sistema pode ser representada da seguinte maneira:

AppScholar  
React Native / Expo  
↓  
fetch()  
↓  
API PHP  
↓  
PDO  
↓  
MySQL  

O objetivo do projeto é construir uma aplicação acadêmica organizada em diferentes módulos, permitindo cadastrar, consultar, atualizar e gerenciar as informações utilizadas no ambiente escolar.

---

## Funcionalidades

As funcionalidades implementadas no projeto deverão ser atualizadas conforme a evolução do sistema.

Entre as funcionalidades do App_Scholar estão:

- Navegação entre as diferentes telas da aplicação;
- Tela inicial com acesso aos módulos do sistema;
- Tela com informações sobre a aplicação;
- Cadastro de alunos;
- Consulta de alunos;
- Edição dos dados de alunos;
- Pesquisa e listagem de alunos;
- Exclusão lógica de alunos por meio da alteração de seu status;
- Comunicação entre o aplicativo e a API utilizando requisições HTTP;
- Consulta de dados armazenados no MySQL;
- Envio de dados em formato JSON entre o aplicativo e a API;
- Integração entre React Native, PHP e MySQL.

Conforme o desenvolvimento do projeto avançar, novos módulos poderão ser implementados para o gerenciamento de:

- Professores;
- Turmas;
- Cursos;
- Disciplinas;
- Matrículas;
- Responsáveis;
- Avaliações;
- Coordenadores;
- Boletins.

> O README deverá ser atualizado sempre que uma nova funcionalidade for efetivamente implementada no sistema.

---

## Tecnologias utilizadas

O projeto utiliza as seguintes tecnologias:

- React Native;
- Expo;
- Expo Snack;
- JavaScript;
- HTML5;
- CSS3;
- PHP;
- PDO;
- MySQL;
- JSON;
- API;
- HTTP;
- Git;
- GitHub.

Também são utilizados conceitos e recursos como:

- `fetch()`;
- `async`;
- `await`;
- `useState`;
- React Navigation;
- métodos HTTP `GET`, `POST` e `PUT`;
- prepared statements;
- `prepare()`;
- `bindValue()`;
- `execute()`;
- CORS;
- operações SQL `SELECT`, `INSERT` e `UPDATE`.

---

## Estrutura do projeto

O projeto está organizado em diferentes áreas, separando a aplicação mobile, a interface web, a API, o banco de dados e a documentação.

Estrutura geral do repositório:

```text
App-Scholar/
│
├── mobile/
│   ├── assets/
│   └── src/
│       ├── components/
│       ├── navigation/
│       ├── screens/
│       ├── services/
│       ├── styles/
│       └── utils/
│
├── web/
│   ├── assets/
│   ├── css/
│   ├── js/
│   └── pages/
│
├── api/
│   ├── config/
│   ├── alunos/
│   ├── professores/
│   ├── cursos/
│   ├── disciplinas/
│   ├── turmas/
│   ├── matriculas/
│   ├── responsaveis/
│   ├── avaliacoes/
│   ├── coordenadores/
│   └── boletins/
│
├── database/
│   ├── schema/
│   ├── seeds/
│   └── scripts/
│
├── docs/
│
├── README.md
│
└── .gitignore
