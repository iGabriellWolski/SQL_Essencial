# Comandos para Criação de Tabelas no MySQL

No MySQL, você pode usar os seguintes comandos para criar tabelas em um banco de dados:

* _CREATE TABLE_: Este é o comando principal usado para criar uma nova tabela no banco de dados. Você define o nome da tabela e lista as colunas e seus tipos de dados.

Exemplo:
```sql
CREATE TABLE usuarios (
id INT AUTO_INCREMENT PRIMARY KEY,
nome VARCHAR(50),
idade INT
);
   ```

 * _PRIMARY KEY_: Este comando é usado para definir uma coluna como chave primária, que deve ser única para cada linha na tabela e pode ser usada para identificar exclusivamente cada linha.

Exemplo:
```sql
CREATE TABLE produtos (
    id INT PRIMARY KEY,
    nome VARCHAR(100),
    preco DECIMAL(10,2)
);
```

* _AUTO_INCREMENT_: Este comando é usado em conjunto com uma coluna INT para criar uma sequência automática de valores numéricos para essa coluna. É comumente usado com chaves primárias para criar identificadores únicos para cada linha.

Exemplo:
```sql
CREATE TABLE alunos (
    id INT AUTO_INCREMENT PRIMARY KEY,
    nome VARCHAR(50),
    idade INT
);
```
* _NOT NULL_: Este comando é usado para especificar que uma coluna não pode aceitar valores nulos, ou seja, cada linha deve ter um valor para essa coluna.

Exemplo:
```sql
CREATE TABLE pedidos (
    id INT PRIMARY KEY,
    nome_cliente VARCHAR(100) NOT NULL,
    total_pedido DECIMAL(10,2)
);
```
* _DEFAULT_: Este comando é usado para definir um valor padrão para uma coluna, que será usado quando nenhum valor é especificado durante a inserção de uma nova linha.

Exemplo:
```sql
CREATE TABLE funcionarios (
    id INT PRIMARY KEY,
    nome VARCHAR(50),
    cargo VARCHAR(50) DEFAULT 'Funcionário'
);
```
* _UNIQUE_: Este comando é usado para garantir que os valores em uma coluna sejam exclusivos, ou seja, nenhum valor duplicado é permitido.

Exemplo:
```sql
CREATE TABLE emails (
    id INT PRIMARY KEY,
    email VARCHAR(100) UNIQUE,
    data_registro DATE
);
```
* _FOREIGN KEY_: Este comando é usado para criar uma chave estrangeira que estabelece uma relação entre duas tabelas. Ele garante a integridade referencial entre as tabelas.

Exemplo:
```sql
CREATE TABLE pedidos (
    id INT PRIMARY KEY,
    id_cliente INT,
    total_pedido DECIMAL(10,2),
    FOREIGN KEY (id_cliente) REFERENCES clientes(id)
);
```
