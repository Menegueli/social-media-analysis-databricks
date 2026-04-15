# 📊 Social Media Impact Analysis (Medallion Architecture)

---

## 🇧🇷 Português

### 🎯 Objetivo do Projeto
Este projeto demonstra a implementação de um pipeline de dados ponta a ponta utilizando a **Arquitetura Medalhão** no **Databricks**. O objetivo é analisar o impacto do uso de redes sociais na saúde mental e no desempenho acadêmico de estudantes ao redor do mundo.

### 🏗️ Arquitetura do Projeto
O pipeline está dividido em três camadas lógicas dentro do **Unity Catalog**:
1.  **Bronze:** Ingestão dos dados brutos de um arquivo CSV (armazenado em Volumes) para tabelas Delta.
2.  **Silver:** Limpeza de dados, padronização de tipos e criação de novas métricas (*Feature Engineering*), como faixas etárias, indicadores de uso pesado e binarização de campos.
3.  **Gold:** Modelagem dimensional (**Star Schema**) com tabelas de Fato e Dimensões, aplicando regras de negócio para classificar qualidade de sono e status de saúde mental.

### ⚙️ Tecnologias Utilizadas
* **Databricks** (Lakehouse)
* **PySpark & Spark SQL**
* **Delta Lake** (Garantindo confiabilidade e performance)
* **Databricks Workflows** (Orquestração automática)

### 🔄 Orquestração (Jobs)
O pipeline foi automatizado para rodar semanalmente, garantindo que os dados sejam processados de forma limpa (Overwrite) e sem duplicatas.

> **<img width="1013" height="415" alt="image" src="https://github.com/user-attachments/assets/14e6d70e-e349-4976-acf4-7213ddcb85f9" />
**

---

## 🇺🇸 English

### 🎯 Project Objective
This project shows an end-to-end data pipeline using the **Medallion Architecture** on **Databricks**. The goal is to analyze how social media usage impacts students' mental health and academic performance worldwide.

### 🏗️ Project Architecture
The pipeline is divided into three logical layers within the **Unity Catalog**:
1.  **Bronze:** Ingestion of raw data from a CSV file (stored in Volumes) into Delta tables.
2.  **Silver:** Data cleaning, type standardization, and **Feature Engineering** (creation of age groups, heavy user indicators, and binary fields).
3.  **Gold:** Dimensional modeling (**Star Schema**) with Fact and Dimension tables, applying business rules to classify sleep quality and mental health status.

### ⚙️ Technologies Used
* **Databricks** (Lakehouse)
* **PySpark & Spark SQL**
* **Delta Lake** (Ensuring reliability and performance)
* **Databricks Workflows** (Automatic orchestration)

### 🔄 Orchestration (Jobs)
The pipeline is automated to run weekly. It uses the "Overwrite" strategy to ensure data is clean and without duplicates.

> **<img width="1013" height="415" alt="image" src="https://github.com/user-attachments/assets/6b842ce1-f1af-43a9-a77c-7d9c4a8e7c7c" />
**

---

### 📂 Estrutura do Repositório / Repository Structure
* `01_bronze_ingestion`: Ingestão de dados brutos / Raw data ingestion.
* `02_silver_refining`: Limpeza e métricas / Cleaning and metrics.
* `03_gold_modeling`: Modelo dimensional e regras de negócio / Dimensional model and business rules.

---
**Status:** ✅ Project Complete & Automated.
