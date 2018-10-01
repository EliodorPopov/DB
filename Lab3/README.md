# LAB3

## Answers to the questions: 
### 1. a)16,2 b)116,2 
### 2. For this table to store the result of Col*Col2 expresion, the data type for Col3 is DECIMAL(2.1)

## Diagram: 
![diagram](diagram.png)

## Querry code: 
```SQL
use universitatea

create table grupe(
	Id_Grupa int primary key identity(1,1),
	Cod_Grupa varchar(10),
	Specialitate varchar(50),
	Nume_Facultate text
)

create table discipline(
	ID_Disciplina int primary key identity(100,1),
	Disciplina varchar(100),
	Nr_ore_plan_disciplina int
)

insert into grupe(Cod_Grupa, Specialitate, Nume_Facultate)
values
('CIB171','Cibernetica','Informatica si Cibernetica'),
('INF171','Informatica','Informatica si Cibernetica'),
('TI171','Tehnologii Informationale','Informatica si Cibernetica')

select * from grupe

insert into discipline(Disciplina,Nr_ore_plan_disciplina)
values
('Sisteme de operare',60),
('Programarea calculatoarelor',60),
('Informatica aplicata',46),
('Sisteme de calcul',46),
('Asamblare si depanare PC',60),
('Cercetari operationale',76),
('Programarea WEB',46),
('Baze de date',60),
('Structuri de date si algoritmi',76),
('Retele informatice',46),
('Matematica discreta',60),
('Modelarea sistemelor',46),
('Limbaje evaluate de programare(Java,.NET)',76),
('Programarea aplicatiilor Windows',60),
('Tehnologii de procesare a informatiei',46),
('Programarea declarativa',46),
('Proiectarea sistemelor informatice',60),
('Practica de licenta',80),
('Practica de productie',80),
('Integrarea informationala europeana',20),
('Programe aplicative',46)

select * from discipline

```