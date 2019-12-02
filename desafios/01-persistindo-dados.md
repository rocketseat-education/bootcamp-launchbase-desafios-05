# Banco de Dados do Foodfy

Nesse desafio você irá criar um banco de dados para o Foodfy.

Você irá manter o padrão que vinha utilizando no Foodfy, e adicionar essa funcionalidade de cadastro de dados em um banco de dados Postgres.

Você irá criar novas páginas de cadastro de chefs, pois uma receita será atribuida a um chef.

Você irá criar filtro de receitas, onde você poderá buscar por determinada receita.

Por fim, você irá adicionar as funcionalidade de paginação na listagem de receitas.

## Banco de Dados e SQL

Usando os conhecimentos adquiridos até aqui, você irá criar um banco de dados pelo Postgres. Coloque o nome `foodfy`. 

Você irá criar uma tabela de receitas. Chame-a de `receipts`. E uma tabela de cozinheiros. Nomei-a como `chefs`. 

Os campos (`colunas`) da tabela `receipts` serão os mesmos que você está usando até o momento. Adicione também, uma coluna de data de criação `created_at`, pois você irá posteriormente ordernar a apresentação das receitas por data de cadastro.

A tabela `chefs` deverá conter os seguinte campos:

* `id integer primary unique` (o postbird cria esse campo por padrão)
* `name text`
* `avatar_url text`
* `created_at datetime`
* `receipt_id integer`

## Cadastro de Chefs

Você irá colocar novas páginas administrativas que serão capazes de fazer as operação de cadastro, listagem, atualização e remoção de chefs.

[Veja o layout das páginas](layouts/)

>Importante: Quando for remover um `chef` você precisa verificar se existem receitas cadastradas para aquele Chef. Você só poderá remover o `chef` se houver uma confirmação de remoção das receitas que foram atribuidas a esse chefe.

## Relacionamento

Fazer uma página especial no site, onde irá mostrar os chefs do Foodfy.

[Veja o layout das páginas](layouts/)

Fazer uma contagem de todas a receitas daquele chef, e apresentar nessa página.

## Filtro e Pesquisa

Para facilitar a busca de uma receita cadastrada, a pessoa que acessar o site poderá filtrar por nome da receita ou por ingredientes.

[Veja o layout da página](layouts/)

## Paginação

Crie uma paginação para a parte de listagem receitas apresentadas no site.

Use uma paginação estilo ` < ANTERIOR | PRÓXIMA >`

Dica: Incremente `page++` ou Decremente `page--` a página atual.
