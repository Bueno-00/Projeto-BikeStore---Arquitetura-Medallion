# Projeto BikeStore — Arquitetura Medallion

Bem-vindo ao projeto **BikeStore com Arquitetura Medallion**, desenvolvido no **Databricks**.  
Este repositório contém a implementação de pipelines de dados seguindo as boas práticas de **Engenharia de Dados**, utilizando **Lakehouse, Apache Spark, SQL e Databricks**.

---

## 🏗 Arquitetura do Projeto

O projeto segue a **Arquitetura Medallion**, com três camadas principais:

1. **Bronze**  
   - Dados brutos importados de diferentes fontes (CSV, APIs, etc).  
   - Nenhuma transformação complexa, apenas ingestão e armazenamento inicial.

2. **Silver**  
   - Dados limpos, validados e integrados.  
   - Transformações aplicadas para corrigir inconsistências e padronizar informações.  
   - Exemplo: validação de clientes, produtos e pedidos.

3. **Gold**  
   - Dados agregados e prontos para análise.  
   - Voltados para **Business Intelligence**, dashboards e relatórios.  
   - Exemplo: vendas consolidadas por região, métricas de desempenho, KPIs.

---

## 📂 Estrutura do Repositório

Projeto-BikeStore---Arquitetura-Medallion/
│
├── 01.bronze/ # Dados brutos importados
├── 02.silver/ # Dados validados e transformados
├── 03.gold/ # Dados finais prontos para análise
└── README.md # Este arquivo

yaml
Copiar código

---

## ⚙ Tecnologias Utilizadas

- **Databricks**  
- **Apache Spark (Python/SQL)**  
- **Lakehouse Architecture**  
- **SQL**  
- **ETL e Pipelines**  
- **Git/GitHub** (para versionamento)

---

## 🚀 Como Executar

1. Clone este repositório no Databricks usando **Repos**:

```bash
https://github.com/Bueno-00/Projeto-BikeStore---Arquitetura-Medallion.git
Abra os notebooks em cada camada (Bronze → Silver → Gold).

Execute os notebooks na ordem da Arquitetura Medallion:

Bronze → Silver → Gold

Confira os resultados e tabelas criadas na workspace do Databricks.

📊 Pipeline Visual
O pipeline foi implementado utilizando Lakehouse Jobs e segue a seguinte sequência:

rust
Copiar código
Bronze (raw) -> Validação Bronze -> Silver -> Validação Silver -> Gold -> Validação Gold
Print do pipeline no Databricks disponível nos notebooks e imagens do projeto.

✨ Próximos Passos
Incluir novas fontes de dados (APIs externas, arquivos JSON/Parquet).

Criar dashboards com Power BI ou Databricks SQL.

Automatizar pipelines com Agendamentos/Jobs no Databricks.

📌 Contato
Rafael Bueno
GitHub: https://github.com/Bueno-00
Email: rafapbueno29@gmail.com
