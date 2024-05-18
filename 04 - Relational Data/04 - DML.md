DML - Data Manipulation Language
=================================

Definição de DML
-----------------------------------

DML (Data Manipulation Language)  é um conjunto de  comandos que permitem aos desenvolvedores manipular dados em um banco de dados. Essa manipulação envolve a inserção de dados em tabelas de banco de dados, a recuperação de dados existentes, a exclusão de dados de tabelas existentes e a modificação de dados existentes. A DML é incorporada em toos os bancos de dados Relacionais.

A DML se assemelha à linguagem simples do inglês e aprimora a interação eficiente do usuário com o sistema. A capacidade funcional da DML é organizada em comandos de manipulação como SELECT, UPDATE, INSERT INTO e DELETE FROM, conforme descrito abaixo:

* `SELECT`: Esse comando é usado para recuperar linhas de uma tabela. SELECT é o comando DML mais amplamente usado no SQL. A sintaxe é 
  
 ````SQL 
  SELECT [nome(s) da(s) coluna(s)] from [nome da tabela] where [condições]. 
````  
  
* `UPDATE`: esse comando modifica os dados de um ou mais registros. A sintaxe de um comando de atualização é 
  
````SQL 
UPDATE [nome da tabela] SET [nome da coluna = valor] where [condição].
````

* `INSERT`: esse comando adiciona um ou mais registros a uma tabela do banco de dados. A sintaxe do comando de inserção é 
  
````SQL   
INSERT INTO [nome da tabela] [coluna(s)] VALUES [valor(es)].
````

* `DELETE`: esse comando remove um ou mais registros de uma tabela de acordo com as condições especificadas. A sintaxe do comando delete é 
  
````SQL 
* DELETE FROM [nome da tabela] where [condição].
````

Existem basicamente dois tipos de linguagem de manipulação de dados. Eles são mencionados abaixo. Nós os descrevemos na diferença entre os formatos.


****Tipos de linguagem de manipulação de dados****
-------------------------------------------

Existem basicamente dois tipos de Linguagem de Manipulação de Dados. Eles são mencionados abaixo. Nós as descrevemos na diferença entre os formatos.

1.  DML de alto nível ou não-procedimental
2.  DML de baixo nível ou processual

### DML de alto nível ou não procedural vs. DML de baixo nível ou procedural

 |DML de alto nível ou sem procedimento|DML de baixo nível ou procedural|
|:---:	|---	|
|Também é rotulada como DML orientada a conjuntos ou séries.|Também é chamada de DML de rastreamento em tempo real.|
|Pode ser usada isoladamente para especificar com precisão operações complexas no banco de dados.|Deve ser integrada a uma linguagem de programação de uso geral.|
| Sua natureza é prescritiva.|É Por natureza, associada a uma solução programada|
|Exige que o usuário indique claramente quais dados são necessários sem esclarecer como e quando obter esses dados.|Ela exige que o usuário indique claramente quais dados são necessários e como obtê-los.|
|****Por exemplo:**** Toda instrução [SQL](https://www.geeksforgeeks.org/what-is-sql/) é um comando prescritivo.|****Por exemplo:**** SQL PL do DB2, [PL/SQL](https://www.geeksforgeeks.org/plsql-introduction/) do Oracle.	|


****Características do DML****
------------------------------

Realiza consultas de dados somente de interpretação. É usada em um esquema de banco de dados para recuperar e manipular as informações. DML É um dialeto usado para selecionar, inserir, excluir e atualizar dados em um banco de dados. Os comandos da Data Manipulation Language (DML) são os seguintes:


****Vantagens da DML****
-------------------------

* As instruções de DML podem alterar os dados contidos ou armazenados no banco de dados.
* Proporciona contato humano efetivo com a máquina.
* O usuário pode especificar quais dados são necessários.
* O objetivo do DML é ter muitas variedades e funcionalidades diferentes entre os fornecedores de bancos de dados.

****Desvantagens do DML****
----------------------------

* Não podemos usar a DML para alterar a estrutura do banco de dados.
* Limitar a visualização da tabela, ou seja, ela pode ocultar algumas colunas nas tabelas.
* Acessar os dados sem ter os dados armazenados no objeto.
* Não é possível criar ou apagar listas ou seções usando DML.