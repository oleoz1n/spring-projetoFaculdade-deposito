# Spring Deposito - Projeto Faculdade

# Sumário

[Estudo de caso ](#_Estudo_de_caso)

[Diagrama de Classes ](#_Diagrama_de_Classes)

<a id="_Estudo_de_caso"></a>

# Estudo de caso

A Holding Benezinho está interessada em investir na abertura de Depósitos no Brasil em 2024. Este investimento pode oferecer diversas vantagens para o empresário, especialmente considerando o contexto econômico e social do país.

Com o objetivo de fazer este negócio dar certo, idealizamos o desenvolvimento de um Sistema de Gestão de produtos estocados a serem comercializados pelas lojas do Conglomerado de empresas da rede.

Criaremos, nesta aula, um Produto Mínimo Viável (PMV) de uma API Rest para este sistema.

Nossa equipe de analistas desenvolveu o Diagrama de Classes abaixo, e a sua missão aqui é realizar o Mapeamento Objeto Relacional das classes de Entidade. Usaremos a JPA e o Hibernate como ferramentas de Mapeamento Objeto Relacional.

Na sprint atual, você foi incumbido de fazer:

1. O Mapeamento Objeto Relacional das primeiras classes envolvidas neste projeto de software;

2. A criação automatizada das tabelas no banco de dados Oracle;

3. A persistência de todos os dados, e;

4. A criação dos Seguintes Repositorios :

    1. DepositoRepository
    2. EnderecoRepository
    3. ItemEstocadoRepository
    4. ProdutoRepository

5. A criação dos Seguintes Resources:

    1. **DepositoResource** com as seguintes ROTAS e VERBOS:

        1. "localhost/deposito" - **GET**, **POST**
        2. "logalhost/deposito/{id}" - **GET**

    2. **EnderecoResource** com as seguintes ROTAS e VERBOS:
        1. "localhost/endereco" - **GET**, **POST**
        2. "logalhost/endereco/{id}" - **GET**
    3. **ProdutoResource** com as seguintes ROTAS e VERBOS:
        1. "localhost/produto" - **GET**, **POST**
        2. "logalhost/produto/{id}" - **GET**
    4. **EntradaResource** com as seguintes ROTAS e VERBOS:

        1. "localhost/entrada/deposito/{idDeposito}/produto/{idProduto}" - **POST**
           No corpo da requisição deverá vir a quantidade de itens da entrada.
           O retorno deverá ser a Lista de Produtos estocados nesta entrada.

    5. **SaidaResource** com as seguintes ROTAS e VERBOS:
        1. "localhost/saida/deposito/{idDeposito}/produto/{idProduto}" - **POST**
           No corpo da requisição deverá vir a quantidade de itens que sairão do deposito.
           O retorno deverá ser a Lista de Produtos que saem nesta requisição.

<a id="_Diagrama_de_Classes"></a>

# Diagrama de Classes

![diagrama-de-classes-deposito.png](documentacao%2Fdiagrama-de-classes-deposito.png)
