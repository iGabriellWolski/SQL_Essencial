# Documentação do MySQL

## Introdução ao SQL

SQL (Structured Query Language) é uma linguagem de programação utilizada para gerenciar e manipular bancos de dados relacionais. Ela fornece uma maneira padronizada de acessar dados armazenados em um sistema de gerenciamento de banco de dados (SGBD) como MySQL, PostgreSQL, SQLite, entre outros.

Com SQL, você pode realizar diversas operações, incluindo a criação de bancos de dados e tabelas, inserção, atualização e exclusão de dados, consulta de informações específicas, entre outras.

# Tipos de Dados de Texto do MySQL

No MySQL, existem vários tipos de dados de texto que podem ser usados para armazenar strings de caracteres de comprimento variável. Abaixo está uma lista de todos os tipos de dados de texto do MySQL:

1. **CHAR**: Armazena uma cadeia de caracteres de comprimento fixo.

2. **VARCHAR**: Armazena uma cadeia de caracteres de comprimento variável.

3. **TINYTEXT**: Armazena uma sequência de caracteres de comprimento máximo de 255 bytes.

4. **TEXT**: Armazena uma sequência de caracteres de comprimento máximo de 65,535 bytes.

5. **MEDIUMTEXT**: Armazena uma sequência de caracteres de comprimento máximo de 16,777,215 bytes.

6. **LONGTEXT**: Armazena uma sequência de caracteres de comprimento máximo de 4,294,967,295 bytes.

Esses tipos de dados de texto permitem armazenar diferentes quantidades de texto, desde pequenas descrições até grandes blocos de texto, como documentos ou conteúdo de páginas da web. A escolha do tipo de dado depende do tamanho máximo esperado do texto que será armazenado.

# Tipos de Dados Numéricos do MySQL

No MySQL, existem vários tipos de dados numéricos que podem ser usados para armazenar diferentes tipos de valores numéricos. Abaixo está uma lista dos tipos de dados numéricos suportados pelo MySQL:

1. **INTEGER ou INT**: Armazena números inteiros, positivos ou negativos, sem casas decimais.
   
2. **TINYINT**: Armazena números inteiros pequenos, geralmente na faixa de -128 a 127 ou de 0 a 255.
   
3. **SMALLINT**: Armazena números inteiros maiores que o TINYINT, geralmente na faixa de -32768 a 32767 ou de 0 a 65535.
   
4. **MEDIUMINT**: Armazena números inteiros ainda maiores que o SMALLINT, geralmente na faixa de -8388608 a 8388607 ou de 0 a 16777215.
   
5. **BIGINT**: Armazena números inteiros muito grandes, geralmente na faixa de -9223372036854775808 a 9223372036854775807 ou de 0 a 18446744073709551615.
   
6. **FLOAT**: Armazena números de ponto flutuante com precisão simples.
   
7. **DOUBLE**: Armazena números de ponto flutuante com precisão dupla.
   
8. **DECIMAL**: Armazena números decimais com precisão fixa.
   
9. **NUMERIC**: Similar ao DECIMAL, armazena números decimais com precisão fixa.
   
10. **REAL**: Um sinônimo para DOUBLE, armazena números de ponto flutuante com precisão dupla.

Esses são os tipos de dados numéricos mais comuns no MySQL, e cada um deles tem suas próprias características e limites. A escolha do tipo de dado depende da faixa de valores e da precisão necessárias para armazenar os dados.

# Tipos de Dados de Datas em SQL

No SQL, incluindo o MySQL, existem vários tipos de dados para lidar com datas e horas. Abaixo está uma lista dos tipos de dados de datas comuns:

1. **DATE**: Armazena uma data no formato 'YYYY-MM-DD'. Esse tipo de dado inclui apenas a data, sem informações de hora.

2. **TIME**: Armazena um horário no formato 'HH:MM:SS'. Esse tipo de dado inclui apenas a hora, sem informações de data.

3. **DATETIME**: Armazena uma data e hora no formato 'YYYY-MM-DD HH:MM:SS'. Esse tipo de dado inclui tanto a data quanto a hora.

4. **TIMESTAMP**: Similar ao DATETIME, armazena uma data e hora no formato 'YYYY-MM-DD HH:MM:SS'. No entanto, o TIMESTAMP tem uma faixa de valores limitada e é automaticamente atualizado pelo sistema para refletir a data e hora atual do sistema quando uma linha é inserida ou atualizada.

5. **YEAR**: Armazena um ano no formato de quatro dígitos 'YYYY'. Esse tipo de dado é usado principalmente para armazenar anos.

Esses são os tipos de dados de datas comuns em SQL, cada um com suas próprias características e uso adequado dependendo dos requisitos do banco de dados e da aplicação.

# Comandos para Alteração de Tabelas no MySQL

No MySQL, você pode usar os seguintes comandos para alterar tabelas:

1. **ALTER TABLE**: Este é o comando principal usado para fazer alterações em uma tabela existente. Alguns exemplos de alterações que você pode fazer com o comando ALTER TABLE incluem adicionar, modificar ou excluir colunas, definir ou modificar restrições de chave primária e estrangeira, renomear a tabela e alterar o tipo de armazenamento da tabela.

2. **ADD COLUMN**: Este comando é usado dentro do comando ALTER TABLE para adicionar uma nova coluna à tabela existente.

3. **MODIFY COLUMN**: Este comando é usado dentro do comando ALTER TABLE para modificar uma coluna existente na tabela. Você pode modificar o tipo de dados da coluna, o tamanho, se a coluna pode aceitar valores nulos, e assim por diante.

4. **DROP COLUMN**: Este comando é usado dentro do comando ALTER TABLE para remover uma coluna existente da tabela.

5. **RENAME COLUMN**: Embora não haja um comando específico para renomear uma coluna diretamente, você pode simular a renomeação através de uma combinação de comandos. Você pode usar o comando ALTER TABLE para adicionar uma nova coluna com o novo nome, copiar os dados da coluna antiga para a nova coluna, remover a coluna antiga e, opcionalmente, renomear a nova coluna com o nome desejado usando o comando ALTER TABLE ... CHANGE COLUMN.

6. **ADD INDEX**: Este comando é usado dentro do comando ALTER TABLE para adicionar um novo índice à tabela existente.

7. **DROP INDEX**: Este comando é usado dentro do comando ALTER TABLE para remover um índice existente da tabela.

8. **RENAME TABLE**: Este comando é usado para renomear uma tabela existente.

Estes são os principais comandos que você pode usar para alterar a estrutura de tabelas em um banco de dados MySQL. Cada comando pode ser usado de várias maneiras para realizar diferentes tipos de alterações na tabela.

