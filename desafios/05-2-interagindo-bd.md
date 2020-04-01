<h1 align="center">
    <img alt="Launchbase" src="https://storage.googleapis.com/golden-wind/bootcamp-launchbase/logo.png" width="400px" />
</h1>

<h3 align="center">
  Desafio 5-2: Interagindo com o BD
</h3>

<blockquote align="center">“Não basta saber, é preferível saber aplicar. Não é o bastante querer, é preciso saber querer.”</blockquote>

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

Nessa etapa, você deve refatorar os CRUDs dos professores e estudantes para que eles utilizem o banco de dados.

### Inserindo dados

No método `post`, construa uma query usando `INSERT` que crie um novo registro no banco de dados.

### Buscando dados

No método `index`, construa uma query usando `SELECT` que retorne todos os registros do banco de dados. Ordene esses resultados pelo nome de forma crescente.

### Criando Model

As operações com o banco de dados não devem ficar no controller, por isso crie um model que contenha os cinco métodos:

- `all`: Buscar todos os registros;
- `create`: Criar um registro;
- `find`: Buscar apenas um registro a partir do id informado;
- `update`: Atualiza um registro a partir do id informado;
- `delete`: Remove um registro a partir do id informado;

### Atualizando dados

Crie um método `update` no model. Nesse método, construa uma query utilizando `UPDATE`, `SET` e `WHERE` que atualiza um registro do banco de dados a partir do id informado.

### Removendo dados

Crie um método `delete` no model. Nesse método, construa uma query utilizando `DELETE` e `WHERE` que remova um registro do banco de dados a partir do id informado.

### Refatorando students

Refatore o controller de estudantes utilizando as mesmas ideias aplicadas no controller de professores.

### Estilização

Você tem liberdade para escolher a estilização que preferir para esse desafio.

## :calendar: Entrega

Esse desafio **não precisa ser entregue** e não receberá correção. Após concluí-lo, adicionar esse código ao seu Github é uma boa forma de demonstrar seus conhecimentos para oportunidades futuras.

## :memo: Licença

Esse projeto está sob a licença MIT. Veja o arquivo [LICENSE](../LICENSE) para mais detalhes.

---

Feito com :purple_heart: by [Rocketseat](https://rocketseat.com.br) :wave: [Entre na nossa comunidade!](https://discordapp.com/invite/gCRAFhc)
