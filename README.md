# Banco-de-Dados---Comandos-e-atribuicoes

CREATE DATABASE cadastroCidade;
USE cadastroCidade;

CREATE TABLE cidade(
id_cidade INT AUTO_INCREMENT PRIMARY KEY,
nome varchar(40)NOT NULL,
uf char(2) NOT NULL,
poúlação INT,
);

INSERT INTO cidade (nome, uf, populacao) VALUES

	('barueri', 'sp', '40000'),
	('rio de janeiro', 'rj', '230000'),
	('carapicuiba', 'sp', '45000'),

 

CREATE DATABASE cadastroFuncionario;
USE cadastroFuncionario;

CREATE TABLE funcionario(
id_funcionario INT AUTO_INCREMENT PRIMARY KEY,
nome varchar (255) NOT NULL,
cpf char (11) UNIQUE,
data-nascimento DATE,
departamento varchar (255),
);

INSERT INTO funcionario (nome, cpf, data-nascimento, departamento) VALUES

	('karen', '123456789', '2003-12-06', 'assessoria'),
	('leo', '987654321', '2002-01-20', 'manutencao'),
	('kelly', '234567891', '1982-07-28', 'esmalteria'),


CREATE DATABSE cadastroMercadoria;
USE cadastroMercadoria;

CREATE TABLE mercadoria(
id_mercadoria INT AUTO_INCREMENT PRIMARY KEY,
tipo_mercadoria varchar (255) NOT NULL,
quant_mercadoria int NOT NULL,
setor_mercadoria varchar (255),
);

INSERT INTO mercadoria (tipo_mercadoria, quant_mercadoria, setor_mercadoria) VALUES

	('agua', 30, 'bebida'),
	('iogurte', 7, 'laticinios'),
	('torrada', 8, 'padaria'),
	('sabonete', 10, 'higiene'),


CREATE DATABASE tabelaCliente;
USE tabelaCliente;

CREATE TABLE cliente(

id_cliente INT AUTO_INCREMENT PRIMARY KEY,
codigoCliente char(10) NOT NULL,
nomeEmpresa varchar(255),
CNPJ char (20) NOT NULL,
Endereco varchar (255),
regiao varchar (255),
CEP varchar(15)
);

INSERT INTO cliente (codigoCliente, nomeEmpresa, CNPJ, Endereco, regiao, CEP) VALUES

	('1', 'CONSULTDA' '123456789000', 'rua concha', 'sao paulo' '0631000'),
	('2', 'TRAVALANCHES', '987654321000', 'rua ostra', 'rio de janeiro', '07396260'),
