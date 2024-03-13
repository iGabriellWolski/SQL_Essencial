# Comandos para Deletar Tabelas em MySQL

## DROP TABLE

- O comando `DROP TABLE` é usado para remover uma tabela do banco de dados.

- **Sintaxe**

  ```sql
  DROP TABLE nome_da_tabela;
  ```

## DROP TABLE IF EXISTS

O comando `DROP TABLE IF EXISTS` é usado para remover uma tabela do banco de dados somente se ela existir.

- **Sintaxe**

  ```sql
  DROP TABLE IF EXISTS nome_da_tabela;
  ```

## DROP TABLE CASCADE

O comando `DROP TABLE CASCADE` é usado para remover uma tabela e todas as suas dependências, como chaves estrangeiras.

- **Sintaxe**

  ```sql
  DROP TABLE nome_da_tabela CASCADE;
  ```

## DROP TABLE RESTRICT

O comando `DROP TABLE RESTRICT` é usado para remover uma tabela apenas se não houver dependências.

- **Sintaxe**

  ```sql
  DROP TABLE nome_da_tabela RESTRICT;
  ```
