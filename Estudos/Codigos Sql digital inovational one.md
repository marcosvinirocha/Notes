<h1>Codigos Sql digital Aula fundamentos de sistemas</h1>

**DDL**

```sql
Create table Cliente(
	codigo number(10) not null Primary key,
	nome varchar(50) not null,
	telefone varchar(15)
);
```

**DML**

```sql
insert into Cliente(codigo,nome,telefone)values(1, "lorem ipsum", "(88)9999-999")

delete from Cliente where codigo = 1

update cliente set nome "lorem ipsum" where codigo 1
```

**DQL**

```sql
select codigo, nome from cliente <where> codigo = 1
<group by> profissao <having> count(1)>0 <order by> nome, codigo
```





