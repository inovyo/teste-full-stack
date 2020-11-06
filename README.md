# TESTE - Desenvolvedor Full Stack
Neste teste você deverá desenvolver uma aplicação para gerenciamento de pesquisas.

Desenvolva o frontend utilizando [React](https://reactjs.org/) e, para a criação do backend, utilize a linguagem que mais tem afinidade e persista os dados em um banco de sua preferência (SQL ou NoSQL).

*Aqui na Inovyo nós utilizamos Python ([FastAPI](https://fastapi.tiangolo.com/)) e Node ([Express](https://expressjs.com/)) para desenvolvimento backend, e a persistência de dados é em um banco SQL.*

## Quais telas precisam ter nesta aplicação?
O usuário deve ter no mínimo 2 telas:
1. Tela com a lista de pesquisas, com opção de criar uma nova pesquisa e editar ou deletar uma pesquisa existente;
2. Tela de edição da pesquisa, onde o usuário poderá inserir, editar ou deletar questões, que poderão ser de 3 tipos: checkbox*, radio* ou textarea.

*No caso das perguntas do tipo `checkbox` ou `radio` o usuário deverá ter um campo para inserir as opções da questão. Ex:

Qual fruta você mais gosta?
- Banana
- Laranja
- Maça
- Outras

## Quais endpoints minha API precisa ter?
GET
- Consulta de todas as pesquisas;
- Consulta individual de pesquisa com as questões da mesma;

POST
- Criação de pesquisa;
- Criação de questão dentro da pesquisa;

PUT/PATCH
- Atualização de pesquisa;
- Atualização de questão;

DELETE
- Remoção de pesquisa;
- Remoção de questão;

### Campos
**Pesquisa**
Variável | Tipo
------------ | -------------
`id` | `int`
`title` | `string`
`status` | `lista` [open, closed]
`created_at` | `data`
`modified_at` | `data`

**Questão**
Variável | Tipo
------------ | -------------
`id` | `int`
`surveyid` | `int`
`title` | `string`
`type` | `lista` [radio, checkbox, textarea]
`options` | `objeto` (obrigatório quando o `type` for `radio` ou `checkbox`)
`created_at` | `data`
`modified_at` | `data`

## Entrega
- Deixamos o visual da aplicação a critério do candidato, iremos avaliar a usabilidade e criatividade;
- Crie um `README.md` curto com os comandos necessários para rodar a aplicação, bastando copiar/colar no terminal;
- Publique sua aplicação no [GitHub](http://github.com/) e envie a URL para o e-mail [talentos@inovyo.com](mailto:talentos@inovyo.com?subject=Teste%20Full%20Stack) com o título `Teste Full Stack`.

## Boa sorte!