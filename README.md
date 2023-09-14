# Banco de Dados: O que é e porque utilizar?

O banco de dados é a organização e armazenamento de informações sobre um domínio esspecifico. De forma mais simples, é o agrupamento de dados que tratam do mesmo assunto, que precisam ser armazenados para segurança ou conferência futura.

Hoje, existem diversos tipos de `SGBDs` (*Sistema Gerenciados de Banco de Dados*), e cada um é addequado para uma necessidade dos clientes. São os mais comuns: `Oracle`, `D2B`, `MySQL`, `SQL Server`, `PostgreSQL` entre outros.

## Relacional

É o mais tradicional dos bancos de dados do mercado. Ele é baseado em relações de tabelas com linhas e colunas armazenadas e controladas por um sistema gerenciador de banco de dados, ou **SGBD**.

As principais vantagens do banco de dados é que são altamente estruturados. Os dados são facilmente armazenados e recuperados por meio de `SQL`(*Structured Query Language* ou *Linguagem de Consulta Estruturada*). Além disso, eles podem ser restritivos ao acesso.

Os bancos de dados relacionais são recomendados para dados altamente estruturados, que necessitam de integidade.

Bancos de dados relacionais trabalham no princípio de que cada tabela tem um campo chave que identifica unicamente cada linha, e que estes campos-chave podem ser usados para ligar uma tabela de dados a outra.

### DER

`DER` (*Diagrama Entidade Relacionamento*), **[Diagrama DER - modulo 26, aula 1, 12:00min]**

### Vantagens

- Rapidez na manipulação e no acesso à informação.
- Redução do esforço de redundancia e de inconsistência de informações, compartilhamento de dados
- Aplicação automatica de restrições de segurança,
- Redução de problemas de integridade.

### Desvantagens

- Pode ser caro dependendo da escolha do SGBD
- Equipe especializada para gerenciar o SGBD
- redundancia de dados

## Não relacional /NoSQL

`NoSQL` (*Not Only SQL*) é o termo utilizado para banco de dados não relacionais de alto desempenho onde, geralmente, o **SQL** não é utilizado como linguagem de consulta.

O **NoSQL** foi criado para ter uma performance melhor e uma escalabilidade mais horizontal para suprir necessidades onde os bancos relacionais não são eficazes.

Geralmente, temos 4 tipos de bancos de dados **NoSQL**: *documentos, colunas, grafos e chave e valor*.

### Documentos

Os dados são armazenados como documentos. Os documentos podem ser descritos como dados no formato de chave-valor como, por exemplo, o padrão `JSON`.

Um exemplo de banco de dados neste formato é o `MongoDB`.

### Colunas

Os dados são armazenados em linhas particulares de tabelas no disco, podendo suportar várias linhas e colunas, além de permitir subcolunas.

U banco de dados dessa família, por exemplo, é o `Cassandra`.

### Grafos

Os dados são armazenados na forma de grafos (*vértices e arestas).

O `Neo4J` é um banco que utiliza grafos.

### Chave e Valor

Essa família de bancos **NoSQL** é a que aguenta a maior carga de dados, pois o conceito dea é que um determindo valor seja acessado através de uma chave identificadora única.

Um exemplo é o banco de dados `Redis`.

## Comparação SQL/NoSQL

**SQL Terms/Concepts**
- database
    - tables
        - rows
            - columns

**NoSQL Terms/Concepts**
- database
    - collections
        - documents (BSON)
            - fields

