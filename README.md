# INDV-MOD-4
Trabalho individual módulo 4

1-Existem outras entidades além dessas três?
Sim, temos Professores, funcionários e etc.

2-Quais são os principais campos e tipos?
Dentro de "Cursos" temos: "ID do curso" (varchar) e "Disciplinas" (varchar). Dentro de "Turmas" temos: "ID da turma" (varchar) e "quantidade de alunos" (int). Dentro de "Alunos" temos: "Matrícula" (int) e "Notas" (int).


3-como essas entidades estão relacionadas?
curso - fornece - turmas
alunos - estuda -turma

*Cardinalidade
Um curso pode ter várias turmas (0,n). Uma turma pode ter somente um curso (0,1). Uma turma tem muitos alunos (0,n). Um aluno pode ter uma turma (0,1).

Script para criar o banco de dados:

1- Código para ativar o mysql: mysql -u root -p

2- Criar o banco de dados: create database resilia;

3- Usar o banco de dados: use resilia;

4- Criar a tabela: create table cursos ( ID_do_cursoo int primary key, disciplinas varchar(10));

create table turmas ( ID_Turma int primary key, quantidade_de_alunos int);

create table alunos ( matricula int primary key, notas int, nome varchar(250), contato varchar(10));

5- Visualizar as tabelas: show tables;

6- Descrever a estrutura da tabela: describe cursos; describe turmas; describe alunos;
