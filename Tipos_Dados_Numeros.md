# Tipos de Dados Numéricos e Booleanos em MySQL
<br>

## INT
O tipo de dado `INT` é usado para armazenar números inteiros.

- **Sintaxe**

    ```sql
    column_name INT;

    idade INT; -- Pode armazenar valores entre -2147483648 e 2147483647.
    ```

## DECIMAL
O tipo de dado `DECIMAL` é usado para armazenar números decimais exatos.

- **Sintaxe**

    ```sql
    column_name DECIMAL(precision, scale);

    preco DECIMAL(8, 2); -- 8 dígitos, sendo 2 após o ponto decimal.
    ```

## FLOAT
O tipo de dado `FLOAT` é usado para armazenar números de ponto flutuante.

- **Sintaxe**

    ```sql
    column_name FLOAT;

    altura FLOAT;
    ```

## DOUBLE
O tipo de dado `DOUBLE` é usado para armazenar números de ponto flutuante de precisão dupla.

- **Sintaxe**

    ```sql
    column_name DOUBLE;

    peso DOUBLE;
    ```

## BOOLEAN
O tipo de dado `BOOLEAN` é usado para armazenar valores booleanos, que podem ser TRUE ou FALSE.

- **Sintaxe**

    ```sql
    column_name BOOLEAN;

    ativo BOOLEAN;
    ```

## TINYINT
O tipo de dado `TINYINT` é usado para armazenar números inteiros pequenos. Pode armazenar valores entre -128 e 127.

- **Sintaxe**

    ```sql
    column_name TINYINT;

    status TINYINT; -- Pode armazenar valores entre -128 e 127.
    ```

## SMALLINT
O tipo de dado `SMALLINT` é usado para armazenar números inteiros pequenos. Pode armazenar valores entre -32768 e 32767.

- **Sintaxe**

    ```sql
    column_name SMALLINT;

    quantidade SMALLINT; -- Pode armazenar valores entre -32768 e 32767.
    ```
