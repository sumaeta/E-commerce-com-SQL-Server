# SQL-Server

## Tabelas
create table Produtos(

	Codigo int,
	Nome varchar(100),
	Descricao varchar(200),
	Preco float
)

create table Cliente (
	
	Codigo int,
	Nome varchar(100), 
	TipoPessoa char(1)
)

create table Pedido (

	Codigo int not null,
	DataSolicitacao datetime not null,
	FlagPago bit not null,
	TotalPedido float not null,
	CodigoCliente int not null

)
