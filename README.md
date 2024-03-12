## Comandos para Criação de Tabelas no MySQL

No MySQL, você pode usar os seguintes comandos para criar tabelas em um banco de dados:

* __CREATE TABLE__: Este é o comando principal usado para criar uma nova tabela no banco de dados. Você define o nome da tabela e lista as colunas e seus tipos de dados.

Exemplo:
```sql
CREATE TABLE usuarios (
id INT AUTO_INCREMENT PRIMARY KEY,
nome VARCHAR(50),
idade INT
);
   ```

 * __PRIMARY KEY__: Este comando é usado para definir uma coluna como chave primária, que deve ser única para cada linha na tabela e pode ser usada para identificar exclusivamente cada linha.

Exemplo:
```sql
CREATE TABLE produtos (
    id INT PRIMARY KEY,
    nome VARCHAR(100),
    preco DECIMAL(10,2)
);
```

* __AUTO_INCREMENT__: Este comando é usado em conjunto com uma coluna INT para criar uma sequência automática de valores numéricos para essa coluna. É comumente usado com chaves primárias para criar identificadores únicos para cada linha.

Exemplo:
```sql
CREATE TABLE alunos (
    id INT AUTO_INCREMENT PRIMARY KEY,
    nome VARCHAR(50),
    idade INT
);
```
* __NOT NULL__: Este comando é usado para especificar que uma coluna não pode aceitar valores nulos, ou seja, cada linha deve ter um valor para essa coluna.

Exemplo:
```sql
CREATE TABLE pedidos (
    id INT PRIMARY KEY,
    nome_cliente VARCHAR(100) NOT NULL,
    total_pedido DECIMAL(10,2)
);
```
* __DEFAULT__: Este comando é usado para definir um valor padrão para uma coluna, que será usado quando nenhum valor é especificado durante a inserção de uma nova linha.

Exemplo:
```sql
CREATE TABLE funcionarios (
    id INT PRIMARY KEY,
    nome VARCHAR(50),
    cargo VARCHAR(50) DEFAULT 'Funcionário'
);
```
* __UNIQUE__: Este comando é usado para garantir que os valores em uma coluna sejam exclusivos, ou seja, nenhum valor duplicado é permitido.

Exemplo:
```sql
CREATE TABLE emails (
    id INT PRIMARY KEY,
    email VARCHAR(100) UNIQUE,
    data_registro DATE
);
```
* __FOREIGN KEY__: Este comando é usado para criar uma chave estrangeira que estabelece uma relação entre duas tabelas. Ele garante a integridade referencial entre as tabelas.

Exemplo:
```sql
CREATE TABLE pedidos (
    id INT PRIMARY KEY,
    id_cliente INT,
    total_pedido DECIMAL(10,2),
    FOREIGN KEY (id_cliente) REFERENCES clientes(id)
);
```
## Comandos para Deletar Tabelas em MySQL

### DROP TABLE
* O comando __DROP TABLE__ é usado para remover uma tabela do banco de dados.

#### Sintaxe:
```sql
DROP TABLE nome_da_tabela;
```

* DROP TABLE IF EXISTS
O comando DROP TABLE IF EXISTS é usado para remover uma tabela do banco de dados somente se ela existir.

Exemplo:
```sql
DROP TABLE IF EXISTS nome_da_tabela;

```
* DROP TABLE CASCADE
O comando DROP TABLE CASCADE é usado para remover uma tabela e todas as suas dependências, como chaves estrangeiras.

Exemplo:
```sql
DROP TABLE nome_da_tabela CASCADE;

```
 * DROP TABLE RESTRICT
O comando DROP TABLE RESTRICT é usado para remover uma tabela apenas se não houver dependências.

Exemplo:
```sql
DROP TABLE nome_da_tabela RESTRICT;

```

## Tipos de Dados de Texto em MySQL

### CHAR
O tipo de dado `CHAR` é usado para armazenar uma string de tamanho fixo. Ele pode armazenar até `length` caracteres.

#### Exemplo:
```sql
column_name CHAR(length);

nome CHAR(50); -- Pode armazenar até 50 caracteres.
```

VARCHAR
O tipo de dado VARCHAR é usado para armazenar uma string de tamanho variável. Ele pode armazenar até length caracteres.

```sql
column_name VARCHAR(length);

endereco VARCHAR(100); -- Pode armazenar até 100 caracteres.
```

TEXT
O tipo de dado TEXT é usado para armazenar grandes blocos de texto.

Sintaxe: 
```sql
column_name TEXT;

descricao TEXT; -- Pode armazenar até 65,535 caracteres.

```

TINYTEXT
O tipo de dado TINYTEXT é usado para armazenar uma pequena quantidade de texto. Ele pode armazenar até 255 caracteres.

Sintaxe:
```sql
column_name TINYTEXT;

comentario TINYTEXT; -- Pode armazenar até 255 caracteres.
```
MEDIUMTEXT
O tipo de dado MEDIUMTEXT é usado para armazenar uma quantidade moderada de texto. Ele pode armazenar até 16,777,215 caracteres.

Sintaxe:
```sql
column_name MEDIUMTEXT;

artigo MEDIUMTEXT; -- Pode armazenar até 16,777,215 caracteres.
```

LONGTEXT
O tipo de dado LONGTEXT é usado para armazenar uma grande quantidade de texto. Ele pode armazenar até 4,294,967,295 caracteres.

Sintaxe:
```sql
column_name LONGTEXT;

conteudo LONGTEXT; -- Pode armazenar até 4,294,967,295 caracteres.
```
## Tipos de Dados Numéricos e Booleanos em MySQL

### INT
O tipo de dado `INT` é usado para armazenar números inteiros.

#### Sintaxe:
```sql
column_name INT;

idade INT; -- Pode armazenar valores entre -2147483648 e 2147483647.
```

DECIMAL
O tipo de dado DECIMAL é usado para armazenar números decimais exatos.

Sintaxe:
```sql
column_name DECIMAL(precision, scale);

preco DECIMAL(8, 2); -- 8 dígitos, sendo 2 após o ponto decimal.
```

FLOAT
O tipo de dado FLOAT é usado para armazenar números de ponto flutuante.

Sintaxe:
```sql
column_name FLOAT;

altura FLOAT;
```
DOUBLE
O tipo de dado DOUBLE é usado para armazenar números de ponto flutuante de precisão dupla.

Sintaxe:
```sql
column_name DOUBLE;

peso DOUBLE;
```
BOOLEAN
O tipo de dado BOOLEAN é usado para armazenar valores booleanos, que podem ser TRUE ou FALSE.

Sintaxe:
```sql
column_name BOOLEAN;

ativo BOOLEAN;
```
TINYINT
O tipo de dado TINYINT é usado para armazenar números inteiros pequenos. Pode armazenar valores entre -128 e 127.

Sintaxe:
```sql
column_name TINYINT;

status TINYINT; -- Pode armazenar valores entre -128 e 127.
```
SMALLINT
O tipo de dado SMALLINT é usado para armazenar números inteiros pequenos. Pode armazenar valores entre -32768 e 32767.

Sintaxe:
```sql
column_name SMALLINT;

quantidade SMALLINT; -- Pode armazenar valores entre -32768 e 32767.
```
## Tipos de Dados de Data em MySQL

### DATE
O tipo de dado `DATE` é usado para armazenar datas no formato 'YYYY-MM-DD'.

#### Sintaxe:
```sql
column_name DATE;

data_nascimento DATE;
```

TIME
O tipo de dado TIME é usado para armazenar horários no formato 'HH:MM:SS'.

Sintaxe:
```sql
column_name TIME;

hora_cadastro TIME;
```

DATETIME
O tipo de dado DATETIME é usado para armazenar datas e horários no formato 'YYYY-MM-DD HH:MM:SS'.

Sintaxe:
```sql
column_name DATETIME;

data_hora_registro DATETIME;
```

TIMESTAMP
O tipo de dado TIMESTAMP é usado para armazenar marcas de tempo, geralmente usadas para registrar a última atualização de uma linha.

Sintaxe:
```sql
column_name TIMESTAMP;

ultima_atualizacao TIMESTAMP;
```

YEAR
O tipo de dado YEAR é usado para armazenar anos no formato 'YYYY'.

Sintaxe:
```sql
column_name YEAR;

ano_fabricacao YEAR;
```
## Comandos de Inserção de Dados em Tabelas MySQL

### INSERT INTO
O comando `INSERT INTO` é usado para inserir novas linhas em uma tabela existente.

#### Sintaxe:
```sql
INSERT INTO nome_da_tabela (coluna1, coluna2, ...) VALUES (valor1, valor2, ...);

INSERT INTO clientes (nome, idade, email) VALUES ('João', 30, 'joao@example.com');
```

INSERT IGNORE INTO
O comando INSERT IGNORE INTO é semelhante ao INSERT INTO, mas ignora as linhas que causariam erros de chave duplicada.

Sintaxe:
```sql
INSERT IGNORE INTO nome_da_tabela (coluna1, coluna2, ...) VALUES (valor1, valor2, ...);

INSERT IGNORE INTO produtos (nome, preco) VALUES ('Camiseta', 20.99);
```
INSERT INTO ... SELECT
O comando INSERT INTO ... SELECT é usado para inserir dados de uma consulta em uma tabela.

Sintaxe:
```sql
INSERT INTO nome_da_tabela (coluna1, coluna2, ...)
SELECT valor1, valor2, ...
FROM outra_tabela
WHERE condição;

INSERT INTO pedidos (produto_id, quantidade)
SELECT id, 2
FROM produtos
WHERE categoria = 'Eletrônicos';
```
REPLACE INTO
O comando REPLACE INTO insere uma nova linha na tabela ou substitui uma linha existente se houver uma chave única ou primária duplicada.

Sintaxe:
```sql
REPLACE INTO nome_da_tabela (coluna1, coluna2, ...) VALUES (valor1, valor2, ...);

REPLACE INTO usuarios (id, nome, email) VALUES (1, 'Maria', 'maria@example.com');
```


