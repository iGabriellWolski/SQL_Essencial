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

