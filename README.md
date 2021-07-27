# E-Commerce com SQL-Server

## O que é o SQL Server
//explicar aqui

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

create table PedidoItem (

	CodigoPedido int not null,
	CodigoProduto int not null,
	Preco float not null,
	Quantidade int not null
)
