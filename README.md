# Documentação do MySQL

## Introdução ao SQL

SQL (Structured Query Language) é uma linguagem de programação utilizada para gerenciar e manipular bancos de dados relacionais. Ela fornece uma maneira padronizada de acessar dados armazenados em um sistema de gerenciamento de banco de dados (SGBD) como MySQL, PostgreSQL, SQLite, entre outros.

Com SQL, você pode realizar diversas operações, incluindo a criação de bancos de dados e tabelas, inserção, atualização e exclusão de dados, consulta de informações específicas, entre outras.

## Comandos Básicos

### DDL (Data Definition Language - Linguagem de Definição de Dados)
- `CREATE DATABASE`: Cria um novo banco de dados.
- `CREATE TABLE`: Cria uma nova tabela no banco de dados.
- `ALTER TABLE`: Modifica a estrutura de uma tabela existente (adicionar, modificar ou excluir colunas).
- `DROP TABLE`: Exclui uma tabela do banco de dados.
- `TRUNCATE TABLE`: Remove todos os registros de uma tabela sem log.

### DML (Data Manipulation Language - Linguagem de Manipulação de Dados)
- `SELECT`: Recupera dados de uma ou mais tabelas.
- `INSERT INTO`: Insere novas linhas em uma tabela.
- `UPDATE`: Modifica dados existentes em uma tabela.
- `DELETE FROM`: Exclui registros de uma tabela.

### DCL (Data Control Language - Linguagem de Controle de Dados)
- `GRANT`: Concede privilégios específicos para usuários em um banco de dados.
- `REVOKE`: Revoga privilégios previamente concedidos a usuários.

## Comandos Intermediários

### TCL (Transaction Control Language - Linguagem de Controle de Transações)
- `COMMIT`: Confirma as transações pendentes.
- `ROLLBACK`: Desfaz as transações pendentes.
- `SAVEPOINT`: Define um ponto no qual você pode rolar de volta a transação.
- `SET TRANSACTION`: Configura propriedades de transação como isolamento e acesso somente leitura.

### DQL (Data Query Language - Linguagem de Consulta de Dados)
- `SELECT`: Consulta dados de uma ou mais tabelas.

### DDL e DML
- `COMMENT`: Adiciona comentários a objetos de banco de dados.

## Conclusão
Esta documentação fornece uma visão geral dos comandos SQL comuns no MySQL, organizados por níveis de complexidade. Para informações mais detalhadas e avançadas, consulte a documentação oficial do MySQL.
