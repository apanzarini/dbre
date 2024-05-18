DDL - Data Definition Language
=================================

Definição de DDL
-----------------------------------

A Data Definition Language(linguagem de definição de dados) é um subconjunto da SQL (linguagem de consulta estruturada) que lida com a estrutura e o esquema do banco de dados, e não com os dados em si. Ela fornece comandos para definir, modificar ou excluir estruturas de banco de dados, como tabelas, esquemas, índices e restrições.

A DDL não lida com dados individuais. Em vez disso, ela se concentra no esquema geral e na arquitetura do banco de dados. Quando uma instrução DDL é executada, ela atualiza o catálogo do sistema do banco de dados, que armazena o esquema do banco de dados, mas nenhum dado é manipulado.

Veja a seguir os principais comandos DDL:

* CREATE: Usado para estabelecer novos objetos de banco de dados.
* ALTER: modifica as estruturas de banco de dados existentes.
* DROP: Remove as estruturas do banco de dados.
* TRUNCATE: remove todos os registros de uma tabela, mas mantém sua estrutura.

Quando usar DDL
-----------------------------------

Você pode gerar DDL em um script para objetos de banco de dados para:
* Manter uma imagem da estrutura do banco de dados
* Configurar um sistema de teste no qual o banco de dados funciona como o sistema de produção, mas não contém dados
* Produzir modelos para novos objetos que você pode criar com base nos existentes. Por exemplo, gerar o DDL para a tabela Customer e, em seguida, editar o DDL para criar a tabela Customer_New com o mesmo esquema.

Ao gerar DDL, você pode usar as instruções gravadas em um arquivo para recriar tudo em um banco de dados, exceto seu conteúdo. Você pode gerar a DDL para recriar completamente o banco de dados ou optar por recriar apenas determinados aspectos dele, como as estatísticas atuais. Você também pode limitar as instruções geradas para que apenas um segmento do banco de dados seja recriado, por exemplo, as estatísticas de um subconjunto de tabelas.

Vantagens da DDL
--------------

* A DDL permite o design e a modificação sistemáticos do esquema do banco de dados.
* Garante uniformidade nas definições da estrutura do banco de dados.
* Com as devidas precauções, a DDL permite que os usuários alterem a estrutura do banco de dados sem afetar os dados nela contidos.

Desvantagens da DDL
-----------------

* Algumas operações DDL, como DROP, não podem ser revertidas e podem levar à perda de dados.
* A execução de determinadas instruções DDL, especialmente em conjuntos de dados grandes ou estruturas complexas, pode levar muito tempo.
* A alteração da estrutura de uma tabela pode levar a erros se outros objetos ou aplicativos no banco de dados dependerem dela.

Um exemplo de DDL seria:

````SQL

DROP VIEW SAMPLE_VIEW;

DROP TABLE SAMPLE_TABLE;

CREATE TABLE SAMPLE_TABLE (
		FIELD_KEY INTEGER,
		FIELD_VALUE INTEGER
);


CREATE VIEW SAMPLE_VIEW AS
 		(SELECT FIELD_VALUE FROM SAMPLE_TABLE)

````

_fonte: https://www.ibm.com_