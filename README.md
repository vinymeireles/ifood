# 🛵 Projeto de Engenharia de Dados: Brazilian Delivery Center IFOOD

Este repositório contém o pipeline completo de Engenharia de Dados utilizando a arquitetura **Medallion (Bronze, Silver e Gold)** com dados públicos do [Brazilian Delivery Center no Kaggle](https://www.kaggle.com/datasets/nosbielcs/brazilian-delivery-center), além da análise de KPIs de negócio visualizados em **Power BI**.

---

## 📁 Estrutura do Projeto

```bash
├── Notebook
  ├── 01.Extract_bronze.ipynb         # Extração dos dados brutos (camada Bronze)
  ├── 02.transform_silver.ipynb       # Limpeza, normalização e enriquecimento dos dados (camada Silver)
  ├── 03.aggregate_gold.ipynb         # Agregações e cálculo de métricas de negócio (camada Gold)
  ├── 04.Analytics_Business.ipynb     # Análises de negócio e geração de insights
  ├── 5.Save_file_to_Power_BI.ipynb   # Exportação dos dados para visualização no Power BI
├── /data                           # Arquivos .parquet gerados em cada camada
├── /powerbi                        # Dashboard e arquivos de relatório do Power BI
└── README.md

⚙️ Tecnologias Utilizadas
Databricks Community Edition

Apache Spark (PySpark)

Parquet (armazenamento columnar)

Power BI (visualização)

Python 3.10

Kaggle Datasets API

🧱 Arquitetura Medallion
O projeto segue a arquitetura em camadas Medallion para processamento de dados:

🔸 Bronze
Extração direta dos arquivos .csv do dataset Kaggle.

Nenhuma transformação é aplicada nesta camada.

Armazenamento em formato Parquet para melhor performance.

🔹 Silver
Limpeza e padronização de dados:

Conversão de tipos.

Tratamento de valores nulos e duplicados.

Enriquecimento com novas colunas.

Estrutura pronta para análise.

🥇 Gold
Agregações e cálculos de indicadores de performance (KPIs):

Total de pedidos por mês.

Receita mensal por centro de entrega.

Avaliação média por entregador e centro de distribuição.

Métricas de eficiência operacional.

📊 Visualização no Power BI
O dashboard em Power BI apresenta os principais KPIs obtidos da camada Gold, com filtros interativos e visualizações:

Receita mensal

Número de entregas por centro

Tempo médio de entrega

Avaliação média dos entregadores

Comparativo entre centros de distribuição

🧾 Arquivo .pbix disponível na pasta /powerbi.

▶️ Execução
Clone o repositório:

bash
Copiar
Editar
git clone https://github.com/seu-usuario/nome-do-repositorio.git
Acesse os notebooks no Databricks Community Edition.

Execute os notebooks na ordem:

01.Extract_bronze.ipynb

02.transform_silver.ipynb

03.aggregate_gold.ipynb

04.Analytics_Business.ipynb

5.Save_file_to_Power_BI.ipynb

Importe os arquivos .parquet gerados no Power BI para análise.

📈 Exemplos de KPIs Gerados
Métrica	Descrição
Receita Total por Mês	Soma dos valores de pedido por mês
Avaliação Média por Entregador	Média das notas de avaliação dos entregadores
Volume de Pedidos por Centro	Quantidade de pedidos por local de distribuição
Tempo Médio de Entrega	Diferença média entre created_at e delivered_at

📌 Referência dos Dados
Dataset: Brazilian Delivery Center - Kaggle
Autor: Nosbiel C Santos
Licença: Creative Commons (CC BY-NC-SA 4.0)

🧑‍💻 Autor
Vinicius Meireles
Engenheiro de Dados | Análise de Negócios com Power BI
LinkedIn (atualize com seu link)

✅ Status do Projeto
✔️ Pipeline completo com camadas Bronze, Silver e Gold
✔️ Exportação para Power BI
✔️ Dashboard interativo publicado
❌ Agendamento automático (em desenvolvimento)

📌 To Do (Futuras Melhorias)
 Agendamento com Databricks Jobs

 Deploy do Power BI em workspace público

 Adição de testes automatizados no pipeline
