[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)



<b>Istruções para consumo da api</b>

Rotas da aplicação

<b>POST /repositories:</b> A rota deve receber title, url e techs dentro do corpo da requisição:
{ id: "uuid", title: 'Desafio Node.js', url: 'http://github.com/...', techs: ["Node.js", "..."], likes: 0 };

<b>GET /repositories:</b> Rota que lista todos os repositórios;

<b>PUT /repositories/:id:</b> A rota deve alterar apenas o title, a url e as techs do repositório que possua o id igual ao id presente nos parâmetros da rota;

<b>DELETE /repositories/:id:</b> A rota deve deletar o repositório com o id presente nos parâmetros da rota;

<b>POST /repositories/:id/like:</b> A rota deve aumentar o número de likes do repositório específico escolhido através do id presente nos parâmetros da rota, a cada chamada dessa rota, o número de likes deve ser aumentado em 1;
