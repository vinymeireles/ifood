# 🛵 Projeto de Engenharia de Dados: Brazilian Delivery Center IFOOD

Este repositório contém o pipeline completo de Engenharia de Dados utilizando a arquitetura **Medallion (Bronze, Silver e Gold)** com dados públicos do [Brazilian Delivery Center no Kaggle](https://www.kaggle.com/datasets/nosbielcs/brazilian-delivery-center), além da análise de KPIs de negócio visualizados em **Power BI**.

---

## 📁 Estrutura do Projeto

```bash
├── 01.Extract_bronze.ipynb         # Extração dos dados brutos (camada Bronze)
├── 02.transform_silver.ipynb       # Limpeza, normalização e enriquecimento dos dados (camada Silver)
├── 03.aggregate_gold.ipynb         # Agregações e cálculo de métricas de negócio (camada Gold)
├── 04.Analytics_Business.ipynb     # Análises de negócio e geração de insights
├── 5.Save_file_to_Power_BI.ipynb   # Exportação dos dados para visualização no Power BI
├── /data                           # Arquivos .parquet gerados em cada camada
├── /powerbi                        # Dashboard e arquivos de relatório do Power BI
└── README.md
![ifood-logo-0](https://github.com/user-attachments/assets/305f52e6-442a-4e89-871e-fd8dc2ff3061)
![ifood-logo-0](https://github.com/user-attachments/assets/305f52e6-442a-4e89-871e-fd8dc2ff3061)
