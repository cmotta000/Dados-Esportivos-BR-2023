# 📊 Análise de Dados Esportivos - Brasileirão 2023

Este projeto realiza o pipeline completo de dados (ETL) dos resultados e estatísticas do Campeonato Brasileiro de 2023. O objetivo é transformar dados brutos em insights estratégicos sobre a performance dos clubes.

---

## 🛠️ Tecnologias Utilizadas

* **Processamento:** [Databricks](https://databricks.com/) (PySpark)
* **Armazenamento/Fonte:** BigQuery (Base dos Dados)
* **Linguagem:** Python
* **Visualização:** Power BI
* **Versionamento:** Git/GitHub

---

## 🚀 Arquitetura do Projeto (Medallion)

O projeto foi organizado seguindo a arquitetura de medalhões para garantir a qualidade do dado:

1.  **Extração (Bronze):** Captura dos dados brutos via API da `basedosdados` diretamente no Databricks.
2.  **Transformação (Silver):** Limpeza, tratamento de nulos, padronização de nomes de clubes e cálculo de métricas básicas usando Spark.
3.  **Enriquecimento (Gold):** Tabelas agregadas prontas para consumo, com KPIs de vitórias, aproveitamento e média de gols por mando de campo.

---

## 📂 Estrutura do Repositório

* 📁 **Notebooks:** Contém os scripts `.py` exportados do Databricks.
    * `01_Extracao_BigQuery`: Script de ingestão.
    * `02_Transformacao_ETL`: Processamento e limpeza.
    * `03_Camada_Ouro`: Criação das tabelas de negócio.
* 📊 **Dashboard:** Arquivo `.pbix` com o relatório interativo.
* 🖼️ **Visualização:** Imagem estática do dashboard final para visualização rápida.

---

## 📈 Insights Principais
Domínio do Campeão: O Palmeiras apresentou a maior eficiência ofensiva da competição, consolidando o título com o melhor saldo de gols e uma arrancada histórica no segundo turno.

A Força da Arena: Times como Grêmio e Fluminense mantiveram um aproveitamento superior a 70% jogando em casa, evidenciando o impacto do mando de campo na tabela final.

Eficiência Defensiva: O Atlético-MG terminou o campeonato com uma das defesas menos vazadas, o que permitiu ao time uma recuperação sólida para garantir a vaga direta na Libertadores.

Equilíbrio na Baixa: A luta contra o rebaixamento foi decidida por detalhes, onde a média de pontos para permanência foi uma das mais altas dos últimos anos, refletindo o equilíbrio técnico da série A.

---

## 🎨 Preview do Dashboard
<img width="769" height="429" alt="Captura de tela 2026-04-16 214415" src="https://github.com/user-attachments/assets/86532255-2957-4177-8ade-4d20ac8e1f51" />



---

## 👨‍💻 Autor

Luís Miguel da Cruz Motta:
https://www.linkedin.com/in/lu%C3%ADs-miguel-da-cruz-motta-a01203265/
