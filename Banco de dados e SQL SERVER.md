# Banco de dados

 

**SGBD** significa sistema gerenciador de banco de dados.

Existem os SGBD's  **relacionais **, que são para sistemas que precisam de uma confiabilidade muito grande dos dados;  será de grande ajuda caso por exemplo, você precise tomar cuidado com dados duplicados. Alguns exemplos de sistemas são: SQL Server, Oracle, MySQL

 Existem também os bancos **NoSQL**, que são bancos de melhor performance e armazenam mais eficientemente vídeos, imagens, links e dentre outras coisas. São exemplos de sistemas NoSQL: MongoDB, Neo4j, Firebase.



# Básicos do SQL SERVER    



**int** = números inteiros 

**bigint** = números inteiros maiores

**varchar** = alfanuméricos, armazena dados de comprimento variável

**char**= alfanuméricos,  armazena dados de comprimento fixo

**float** = aceita casas decimais

**bit** = 0 e 1

**null**= aceita nulos

**not null** = não aceita nulos

**nulo** = ausência de valor



## Comandos 

**criar banco de dados**

create database nomebanco

**selecionar banco de dados** 

use nomebanco

**criar tabela**

create table nometabela 

**apagar tabela**

drop table nometabela



**selecionar tabela** 

select exemplo from nometabela 

**ver informações da tabela** 

alt f1

**inserir informação na tabela**

insert into nometabela ( selecionarColuna,       selecionarColuna) values (valorDesejado, valorDesejado)

**especificar local/linha** 

where nomeColuna = exemplo

**modificar algo já existente**

update nomeTabela set nomeColuna = condiçãoDesejada where nomeColuna = lugarDesejado

**apagar informação**

delete from Nometabela where nomeColuna = localDesejado

**pegar data e horário atual**

getdate()

**Mudar o tipo de coluna**

alter table nomeColuna add tipoDesejado

**inserir chave primaria**

alter table nomeTabela add constraint nome_desejado primary key ( nomeColuna)

**inserir chave estrangeira**

alter table nomeTabela add constraint nome_desejado foreign key ( nomeColuna) references nomeTabela (nomeColuna)



# Chaves primarias e estrangeiras

**chaves primarias** são usadas para garantir que dados em uma determinada coluna não se repitam; identifica cada registro de forma única.

**Chaves estrangeiras** fazem o mesmo, porém estabelecendo relações entre tabelas. 

mudando colunas para true indetity fazemos com que ela se atualize sozinha a cada inserção de novos dados.