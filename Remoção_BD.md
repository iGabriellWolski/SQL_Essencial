# Comandos de Remoção de Dados em Tabelas MySQL

O comando `DELETE` é usado para remover registros de uma tabela com base em uma condição específica.

- **Sintaxe**

    ```sql
    DELETE FROM nome_da_tabela WHERE condição;

    --  O comando DELETE remove os registros da tabela que satisfazem a condição especificada.

    DELETE FROM clientes WHERE idade > 30;

    -- Este exemplo remove todos os registros da tabela 'clientes' onde a idade é superior a 30.
    ```

## TRUNCATE TABLE
O comando `TRUNCATE TABLE` é usado para remover todos os registros de uma tabela, mas mantém a estrutura da tabela intacta.

- **Sintaxe**

    ```sql
    TRUNCATE TABLE nome_da_tabela;

    -- O comando TRUNCATE TABLE remove todos os registros de uma tabela, mas não pode ser revertido. Ele é mais rápido que o DELETE para remover todos os registros de uma tabela.

    TRUNCATE TABLE pedidos;

    -- Este exemplo remove todos os registros da tabela 'pedidos', mas mantém a estrutura da tabela.
    ```

## DROP TABLE
O comando `DROP TABLE` é usado para remover uma tabela inteira do banco de dados.

- **Sintaxe**

    ```sql
    DROP TABLE nome_da_tabela;

    -- O comando DROP TABLE exclui permanentemente a tabela e todos os seus dados, índices e privilégios associados.

    DROP TABLE produtos;

    -- Este exemplo remove permanentemente a tabela 'produtos' do banco de dados.
    ```
