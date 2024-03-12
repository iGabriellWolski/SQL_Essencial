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






