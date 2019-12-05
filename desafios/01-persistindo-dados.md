# Banco de Dados do Foodfy

Nesse desafio você irá criar um banco de dados para o Foodfy.

A partir desse desafio, os dados que antes você vinha salvando em um arquivo JSON agora serão armazenados em um banco de dados PostgreSQL.

Você irá criar novas páginas de cadastro, listagem e edição de chefs, pois uma receita será atribuida a um chef.

Você irá criar um busca de receitas, onde você poderá filtrar receitas pelo seu nome.

Por fim, você irá adicionar a funcionalidade de paginação na listagem de receitas.

## 🗄 Banco de dados

Usando os conhecimentos adquiridos até aqui, você irá criar um banco de dados pelo Postgres, utilize o nome `foodfy`. 

Você irá criar uma tabela de receitas, chame-a de `receipts` e uma tabela de cozinheiros, nomei-a como `chefs`.

A tabela `receipts` deverá conter os seguintes campos:

* `id integer primary unique` (o postbird cria esse campo por padrão)
* `chef_id integer` (esse campo armazenará o ID do chef que criou essa receita)
* `image text`
* `title text`
* `ingredients text[]`
* `preparation text[]`
* `information text`
* `created_at datetime` (armazena a data de criação da receita no banco de dados)

*Obs.: Você consegue armazenar vetores (`arrays`) no Postgres utilizando o `[]` no fim do campo.*

A tabela `chefs` deverá conter os seguinte campos:

* `id integer primary unique` (o postbird cria esse campo por padrão)
* `name text`
* `avatar_url text`
* `created_at datetime` (armazena a data de criação do chef no banco de dados)

## 🍴 [Admin] Cadastro de chefs

<div align="center">
   <img src="https://rocketseat-cdn.s3-sa-east-1.amazonaws.com/launchbase/mockup-cadastro-chefs.png" />
</div>

Você irá colocar novas páginas administrativas que serão capazes de fazer as operação de cadastro, listagem, atualização e remoção de chefs.

**Download dos arquivos:** https://github.com/Rocketseat/bootcamp-launchbase-desafios-05/archive/master.zip

Acesse o arquivo `layouts/admin/index.html` para ver todas especificações do layout do site.

>Importante: Quando um chef for removido, se o mesmo possuir pelo menos uma receita, retorne um erro informando que chefs que possuem receitas não podem ser deletados.

## 🕵🏻‍♂️ [Site] Busca de receitas

<div align="center">
   <img src="https://rocketseat-cdn.s3-sa-east-1.amazonaws.com/launchbase/mockup-busca.png" />
</div>

Para facilitar a busca de uma receita cadastrada, a pessoa que acessar o site poderá filtrar por nome da receita.

Você criará também uma página de resultado da busca que listará as receitas de acordo com a busca do usuário.

**Download dos arquivos:** https://github.com/Rocketseat/bootcamp-launchbase-desafios-05/archive/master.zip

Acesse o arquivo `layouts/site/index.html` para ver todas especificações do layout do site.

## 👩🏽‍🍳 [Site] Listagem de chefs

<div align="center">
   <img src="https://rocketseat-cdn.s3-sa-east-1.amazonaws.com/launchbase/mockup-chefs.png" />
</div>

Fazer uma página com nome "Chefs" no site onde irá mostrar os chefs do Foodfy.

Fazer uma contagem de todas a receitas daquele chef, e apresentar nessa página.

**Download dos arquivos:** https://github.com/Rocketseat/bootcamp-launchbase-desafios-05/archive/master.zip

Acesse o arquivo `layouts/site/index.html` para ver todas especificações do layout do site.

