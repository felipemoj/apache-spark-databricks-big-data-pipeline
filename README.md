
# Big Data Processing with Apache Spark and Databricks

**Data Engineering Project | Apache Spark, PySpark, Spark SQL, Delta Lake**

[🇧🇷 Versão em Português](#versão-em-português)

## Overview

This academic project was developed during the Data Engineering, Big Data and AI postgraduate program at Instituto Infnet.

The project implements a batch ETL pipeline using Apache Spark and Databricks to process sales data from multiple CSV files, integrate datasets, and generate analytical insights.

It follows the Medallion Architecture, organizing data into Bronze, Silver, and Gold layers.

## Tech Stack

- Python
- Apache Spark and PySpark
- Spark SQL
- Databricks
- Delta Lake
- Unity Catalog
- ETL and Data Processing

## Data Architecture

**CSV Files → Bronze → Silver → Gold → Analytics**

### Bronze Layer — Data Ingestion

- Ingestion of 12 CSV datasets.
- Initial schema inspection and data profiling.
- Storage of source datasets as managed tables.

### Silver Layer — Data Transformation

- Integration of orders, order items, products, categories, and customers.
- Data transformations using PySpark DataFrames.
- Creation of an integrated sales dataset.
- Storage of processed data in Delta tables.

### Gold Layer — Data Analytics

- Sales aggregation by product category.
- Category ranking using Window Functions.
- Pivot analysis by city and category.
- Revenue analysis using Spark SQL.

## Performance and Governance

- Execution plan analysis using `EXPLAIN FORMATTED`.
- Join strategies and Spark execution optimization.
- Catalog, schema, and table inspection.
- Data governance and permissions using Unity Catalog.

## Project Results

- Approximately **1.59 million source records** processed.
- **12 CSV datasets** ingested.
- Approximately **600,000 sales records** consolidated in the Silver layer.
- Analytical transformations using JOINs, aggregations, Window Functions, and Pivot operations.

## How to Run

This project was developed in Databricks and requires a compatible workspace with Apache Spark, Delta Lake, and appropriate catalog permissions.

1. Import `Databricks_projeto_Spark.ipynb` into Databricks.
2. Upload the required CSV datasets to the configured storage location.
3. Adjust the `RAW_PATH` variable and catalog/schema names if necessary.
4. Run the notebook cells in sequence.

**Note:** Source datasets are not included in this repository. The pipeline requires the original datasets to execute end-to-end.

---

# Versão em Português

## Visão Geral

Este projeto acadêmico foi desenvolvido durante a pós-graduação em Engenharia de Dados: Big Data e IA do Instituto Infnet.

O objetivo é implementar um pipeline ETL batch utilizando Apache Spark e Databricks para processar dados de vendas, integrar diferentes conjuntos de dados e gerar informações analíticas.

O projeto utiliza a arquitetura Medallion, dividida nas camadas Bronze, Silver e Gold.

## Tecnologias Utilizadas

- Python
- Apache Spark e PySpark
- Spark SQL
- Databricks
- Delta Lake
- Unity Catalog
- ETL e Processamento de Dados

## Arquitetura de Dados

**Arquivos CSV → Bronze → Silver → Gold → Análises**

### Camada Bronze — Ingestão

- Ingestão de 12 conjuntos de dados CSV.
- Inspeção de schemas e análise inicial dos dados.
- Armazenamento dos dados de origem em tabelas gerenciadas.

### Camada Silver — Transformação

- Integração de pedidos, itens, produtos, categorias e clientes.
- Transformações utilizando DataFrames do PySpark.
- Construção de uma tabela consolidada de vendas.
- Armazenamento dos dados processados em tabelas Delta.

### Camada Gold — Análise

- Agregação de vendas por categoria de produtos.
- Ranking de categorias utilizando Window Functions.
- Análise Pivot por cidade e categoria.
- Consultas de faturamento utilizando Spark SQL.

## Performance e Governança

- Análise de planos de execução com `EXPLAIN FORMATTED`.
- Estudo de estratégias de JOIN e otimização do Spark.
- Inspeção de catálogos, schemas e tabelas.
- Governança e permissões de acesso utilizando Unity Catalog.

## Resultados do Projeto

- Processamento de aproximadamente **1,59 milhão de registros** na origem.
- Ingestão de **12 arquivos CSV**.
- Consolidação de aproximadamente **600 mil registros de vendas** na camada Silver.
- Transformações analíticas com JOINs, agregações, Window Functions e Pivot.

## Como Executar

O projeto foi desenvolvido no Databricks e requer um workspace compatível com Apache Spark, Delta Lake e permissões adequadas no catálogo.

1. Importe `Databricks_projeto_Spark.ipynb` no Databricks.
2. Disponibilize os arquivos CSV necessários.
3. Ajuste a variável `RAW_PATH` e os nomes de catálogo/schema, se necessário.
4. Execute as células do notebook em sequência.

**Observação:** Os datasets originais não estão incluídos neste repositório.

---

## Author / Autor

**Felipe Martins de Oliveira Júnior**

Computer Science Graduate | Data Engineering Postgraduate Student

- LinkedIn: https://linkedin.com/in/felipemoj
- GitHub: https://github.com/FelipeJunior20

Academic project developed at Instituto Infnet.
