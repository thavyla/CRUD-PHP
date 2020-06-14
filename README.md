# Projeto CRUD em PHP

## Sobre o projeto

O projeto é um CRUD de clientes criado utilizando o framework laravel e banco de dados mysql.

## Requesitos

-   php = "^7.2.5".
-   laravel = "5.8.\*".
-   mysql.
-   Composer.

## Funcionalidades

-   Cadastro;
-   Listagem;
-   Edição;
-   Exclusão;

## Instalação

Realize o clone do projeto (https://github.com/thavyla/CRUD-PHP.git).

Crie um banco de dados no mysql e utilize o Arquivo .env.example para configura-lo no projeto;

### Instalando dependencias;

-   composer install

#### Criando as tabelas no banco

-   php artisan migrate

## Rotas

### Cadastro do Cliente

```http
POST http://localhost:8000/cliente
```

Parâmetros

```js
{
    "_token":"",
    "nome":"",
    "sobre_nome":"",
    "endereco":"",
    "bairro":"",
    "cidade":"",
    "uf":"",
    "cep":"",
}
```

### Listando todos os clientes

```http
GET http://localhost:8000/cliente
```

### Editando os dados do cliente

```http
Passe o ID do cliente no qual deseja editar.

PUT http://localhost:8000/cliente/{id}

```

Parâmetros

```js
{
    "_token":"",
    "nome":"",
    "sobre_nome":"",
    "endereco":"",
    "bairro":"",
    "cidade":"",
    "uf":"",
    "cep":"",
}
```

### Excluindo um cliente

```http
Passe o ID do cliente no qual deseja excluir.

DELETE http://localhost:8000/cliente/{id}

```

Parâmetros

```js
{
    "_token":""
}
```

### Pesquisar

```http

POST http://localhost:8000/pesquisar

```

Parâmetros

```js
{
    "_token":"",
    "texto_busca":""
}
```

## CRUD cliente finalizado.
