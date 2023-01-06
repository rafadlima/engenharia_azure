# Construção DW Superstore

Projeto de criação de um DW baseado no Dataset Superstore Marketing Campaign disponibilizado via Kaggle.

As seguintes etapas foram realizadas durante o trabalho:
* Criação de um Datalake no Azure
* Criação de um Banco de Dados SQL e um Servidor SQL Server no Azure
* Carga do Dataset em CSV no Datalake
* ETL via Data Factory:
    1. Cópia dos dados no Datalake para o Banco SQL: Nessa etapa os dados foram transferidos do DL para uma Stage no SQL Server com criação dinamica do Schema.
    2. Processo de ETL via Data Factory:
        a. Criação da Tabela dClientes. Foi separado da Stage os dados relacionados aos clientes e carregados em uma tabela individual com sua respectiva sk.
        b. Criação da Tabela fCompras. Foi separado os valoresd e quantidade de compras realizadas pelos clientes.
