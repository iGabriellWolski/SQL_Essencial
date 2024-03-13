# Tipos de Dados de Texto em MySQL
<br>

# CHAR
O tipo de dado `CHAR` é usado para armazenar uma string de tamanho fixo. Ele pode armazenar até `length` caracteres.

- **Sintaxe**

    ```sql
    column_name CHAR(length);

    nome CHAR(50); -- Pode armazenar até 50 caracteres.
    ```

## VARCHAR
O tipo de dado `VARCHAR` é usado para armazenar uma string de tamanho variável. Ele pode armazenar até length caracteres.

    ```sql
    column_name VARCHAR(length);

    endereco VARCHAR(100); -- Pode armazenar até 100 caracteres.
    ```

# TEXT
O tipo de dado `TEXT` é usado para armazenar grandes blocos de texto.

- **Sintaxe**

    ```sql
    column_name TEXT;

    descricao TEXT; -- Pode armazenar até 65,535 caracteres.

    ```

# TINYTEXT
O tipo de dado `TINYTEXT` é usado para armazenar uma pequena quantidade de texto. Ele pode armazenar até 255 caracteres.

- **Sintaxe**

    ```sql
    column_name TINYTEXT;

    comentario TINYTEXT; -- Pode armazenar até 255 caracteres.
    ```

# MEDIUMTEXT
O tipo de dado `MEDIUMTEXT` é usado para armazenar uma quantidade moderada de texto. Ele pode armazenar até 16,777,215 caracteres.

- **Sintaxe**

    ```sql
    column_name MEDIUMTEXT;

    artigo MEDIUMTEXT; -- Pode armazenar até 16,777,215 caracteres.
    ```

# LONGTEXT
O tipo de dado `LONGTEXT` é usado para armazenar uma grande quantidade de texto. Ele pode armazenar até 4,294,967,295 caracteres.

- **Sintaxe**

    ```sql
    column_name LONGTEXT;

    conteudo LONGTEXT; -- Pode armazenar até 4,294,967,295 caracteres.
    ```
