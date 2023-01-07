#  Projeto Azure

-- Construção DW Superstore
Projeto de criação de um DW baseado no Dataset Superstore Marketing Campaign disponibilizado via Kaggle.

As seguintes etapas foram realizadas durante o projeto:
* Criação de um Datalake no Azure
* Criação de um Banco de Dados SQL e um Servidor SQL Server no Azure
* Carga do Dataset em CSV no Datalake
* ETL via Data Factory:
    1. Cópia dos dados no Datalake para o Banco SQL: Nessa etapa os dados foram transferidos do DL para uma Stage no SQL Server com criação dinamica do Schema.
    2. Processo de ETL via Data Factory:
        a. Criação da Tabela dClientes. Foi separado da Stage os dados relacionados aos clientes e carregados em uma tabela individual com sua respectiva sk.
        b. Criação da Tabela fCompras. Foi separado os valoresd e quantidade de compras realizadas pelos clientes.

-- Azure Synapse
As seguintes etapas foram realizadas durante o projeto:
* Criação de Pool de SQL Dedicado
* Carga de Dados no Pool de SQL Dedicado por um CSV disponibilizado no Datalake

Projeto Cotação Dolar
* Carga no Datalake das cotações do dolar retirados diretamente do site do Banco Central do Brasil, com link dinamico para definição da data
* Consulta SQL para Análise dos Dados utilizando T-SQL
* Carga dos Dados em uma Tabela Externa do SQL Serveless
* Conexão com PowerBI para gerar relatório.

Proejto DW Contoso --Em Andamento--
* Cargado dos Arquivos CSC no Datalake
* Geração dos Scrits Iniciais de Consultas
* Elaboração da Modelagem do DW
* Carga do DW Sql Pool Dedicado utilizando Pool Spark
