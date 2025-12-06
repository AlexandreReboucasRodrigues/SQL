<h1>SQL</h1>

<h2>SQL com SQLite</h2>

<h3>Consultas</h3>

<h4> CREATE TABLE </h4>

~~~ SQL
CREATE TABLE aluno (
  id INTEGER NOT NULL PRIMARY KEY AUTOINCREMENT,
  nome TEXT NOT NULL,
  telefone TEXT NOT NULL, 
  curso TEXT NOT NULL,
  turma INTEGER NOT NULL,
  unidade TEXT NOT NULL,
  pcd BOOLEAN NOT NULL DEFAULT false
);
~~~

- `CREATE TABLE`: comando para criar uma tabela
- `aluno`: nome da tabela
- `id`,`nome`,`telefone`,`curso`,`turma`,`unidade`,`pcd`;colunas da te=abela
- `INTEGER`,`TEXT`,`BOOLEAN`: tipos de dados da coluna
- `NOT NULL`: não permite ausência de valor na coluna
- `DEFAULT`: insere um valor padrão na coluna

<h4>INSERT INTO</H4>

~~~sql
INSERT INTO aluno (nome, telefone, curso, turma, unidade)
VALUES ('Alex','(85) 992855525', 'Full Stack', 26, 'Sul');
~~~

-`INSERT INTO`: comando para inserir dados na tabela
-`aluno`: nome da tabela
-`(nome, telefone, curso, turma, unidade)`: colunas da tabela que serão inseridos dados
-`VALUES`: define os valores a serem inseridos
-`('Alex','(85) 992855525', 'Full Stack', 26, 'Sul')`: valores para cada coluna da tabela referente a ordem especificada

<h4|>Slecionar Tabela</h4>

~~~ sql
SELECT * FROM aluno;
~~~

-`SELECT`: comandpo para selecionar a coluna
-`*`: indica todas as colunas tabela
-`FROM`:indica qual a coluna será slecionada
-`aluno`: nome da tabela

<h4>Alterar o valor na tabela</h4>

~~~ sql
UPDATE aluno SET turma = 11 WHERE id = 2;
~~~

-`UPDATE`: comando para atualzar valor na tabela
-`aluno`: nome da tabela
-`SET`: comando para definir coluna e valor para atualização
-`turma = 11`: coluna e novo valor
-`WHERE`: Ccomando para filtrar a linha da tablea
-`id = 2`: coluna e valro filtrado

-`DELETE`: comando para deletar valor na tabela
-`FROM`indica qual tabela 
-`aluno`: nome da tabela
-`WHERE`: Ccomando para filtrar a linha da tablea
-`id = 3`: coluna e valro filtrado