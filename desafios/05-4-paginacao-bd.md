<h1 align="center">
    <img alt="Launchbase" src="https://storage.googleapis.com/golden-wind/bootcamp-launchbase/logo.png" width="400px" />
</h1>

<h3 align="center">
  Desafio 5-4: Paginação de resultados no BD
</h3>

<blockquote align="center">“Não compare o seu bastidor com o palco do outro!”</blockquote>

<p align="center">

  <a href="https://rocketseat.com.br">
    <img alt="Made by Rocketseat" src="https://img.shields.io/badge/made%20by-Rocketseat-%23F8952D">
  </a>

  <a href="LICENSE" >
    <img alt="License" src="https://img.shields.io/badge/license-MIT-%23F8952D">
  </a>

</p>

<p align="center">
  <a href="#rocket-sobre-o-desafio">Sobre o desafio</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#calendar-entrega">Entrega</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#memo-licença">Licença</a>
</p>

## :rocket: Sobre o desafio

Nessa etapa, você deve implementar a lógica de paginação dos resultados do BD.

### Backend

Adicione no método `index` do controller de professores o tratamento dos campos `page` e `limit` que serão transmitidos via `query params`. Além disso, faça o cálculo do `offset` a ser passado para a query. Por fim, crie um novo método `paginate` no model que deve implementar toda a query já existente (com filter e order) e também adicionar a paginação (utilize `LIMIT` e `OFFSET`).

### Frontend

Crie um algoritmo que realize a paginação dos resultados da seguinte forma:

- As duas primeiras e últimas páginas sempre devem ser apresentadas (ex: 1, 2, 45 e 46 de um total de 46 pags.);
- Caso existam mais de 7 páginas, as intermediárias selecionadas devem ser apresentadas juntamente com seu sucessor e antecessor (ex.: 1, 2, ..., 12, 13 (selecionada), 14, ..., 23, 24);
- Só apresente as reticências se elas representarem um grupo de 2 páginas ou mais (ex.: 1, 2, 3 (sem reticências), 4, 5 (selecionada), 6, ...(pags 7 e 8), 9, 10).

Em seguida, implemente na query do método `paginate` no model de professor a lógica da páginação:

- realizar o `count` de todos os registros de professores (utilize uma `subquery`);
- aplicar os filtros tanto na `query` de busca dos professores quanto na `subquery` de `count`.

Por fim, utilize o `scripts.js` para renderizar no `html` (não faça no `nunjucks`) a paginação ao final da listagem (não esqueça que as reticências não devem ser links).

### Ajustes finais

Para finalizar, basta:

- Estilizar a paginação;
- Preservar o filter quando a página for alterada;
- Implementar no front dos estudantes a paginação (siga a mesma ideia aplicada nos professores).

### Estilização

Você tem liberdade para escolher a estilização que preferir para esse desafio.

## :calendar: Entrega

Esse desafio **não precisa ser entregue** e não receberá correção. Após concluí-lo, adicionar esse código ao seu Github é uma boa forma de demonstrar seus conhecimentos para oportunidades futuras.

## :memo: Licença

Esse projeto está sob a licença MIT. Veja o arquivo [LICENSE](../LICENSE) para mais detalhes.

---

Feito com :purple_heart: by [Rocketseat](https://rocketseat.com.br) :wave: [Entre na nossa comunidade!](https://discordapp.com/invite/gCRAFhc)
