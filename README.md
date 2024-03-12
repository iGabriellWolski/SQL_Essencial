# Comandos para Criação de Tabelas no MySQL

No MySQL, você pode usar os seguintes comandos para criar tabelas em um banco de dados:

* **CREATE TABLE**: Este é o comando principal usado para criar uma nova tabela no banco de dados. Você define o nome da tabela e lista as colunas e seus tipos de dados.

   Exemplo:
   ```sql
   CREATE TABLE usuarios (
       id INT AUTO_INCREMENT PRIMARY KEY,
       nome VARCHAR(50),
       idade INT
   );
   ```

 * PRIMARY KEY: Este comando é usado para definir uma coluna como chave primária, que deve ser única para cada linha na tabela e pode ser usada para identificar exclusivamente cada linha.

Exemplo:
```sql
CREATE TABLE produtos (
    id INT PRIMARY KEY,
    nome VARCHAR(100),
    preco DECIMAL(10,2)
);
```

* AUTO_INCREMENT: Este comando é usado em conjunto com uma coluna INT para criar uma sequência automática de valores numéricos para essa coluna. É comumente usado com chaves primárias para criar identificadores únicos para cada linha.

Exemplo:
```sql
CREATE TABLE alunos (
    id INT AUTO_INCREMENT PRIMARY KEY,
    nome VARCHAR(50),
    idade INT
);
```
* NOT NULL: Este comando é usado para especificar que uma coluna não pode aceitar valores nulos, ou seja, cada linha deve ter um valor para essa coluna.

Exemplo:
```sql
CREATE TABLE pedidos (
    id INT PRIMARY KEY,
    nome_cliente VARCHAR(100) NOT NULL,
    total_pedido DECIMAL(10,2)
);
```
