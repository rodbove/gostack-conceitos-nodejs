### :rocket: Sobre o desafio
Desafio consistiu em construir rotas para um CRUD simples com Node.js para repositórios do GitHub. As rotas deveriam ser construidas de forma que passassem todos os testes .

### :twisted_rightwards_arrows: Rotas da aplicação
- **`POST /repositories`**: Rota que recebe `title`, `url` e um array de `techs` no corpo da requisição. Além dos valores enviados, um id em formato UUID é criado e o repositório recebe a propriedade `likes` com o valor `0`;

- **`GET /repositories`**: Rota que lista todos os repositórios;

- **`PUT /repositories/:id`**: Rota que permite alterar apenas os campos `title`, `url` e `techs` do repositório com `id` igual ao `id` enviado nos parâmetros da rota;

- **`DELETE /repositories/:id`**: Deleta o repositório com o `id` igual ao enviado nos parâmetros da rota;

- **`POST /repositories/:id/like`**: Aumenta em `1` o número de likes do repositório com `id` igual ao enviado nos parâmetros da rota.

### :computer: Testando localmente
Para testar o código: clone o repositório na pasta de sua preferência -> instale as dependências utilizando `yarn` ou `npm`. Utilize o comando `yarn dev` para iniciar o servidor em `localhost:3333` e o comando `yarn test` para a verificação dos testes.
