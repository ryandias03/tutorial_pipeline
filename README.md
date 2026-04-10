# 🚀 Data Engineering Pipeline com Python, Airflow e PostgreSQL

Pipeline de dados desenvolvido para simular um fluxo real de Engenharia de Dados, incluindo ingestão, transformação, persistência e orquestração automatizada.

## 📌 Visão Geral

Este projeto implementa um pipeline completo de dados utilizando Python, com orquestração via Apache Airflow e armazenamento em PostgreSQL. O objetivo é reproduzir um cenário real de processamento de dados em ambiente moderno de dados.

## 🧱 Arquitetura

O pipeline segue o modelo clássico de Engenharia de Dados:

- Ingestão: coleta de dados via API externa
- Processamento: transformação e limpeza com Python e Pandas
- Persistência: armazenamento estruturado em PostgreSQL
- Orquestração: automação das etapas com Apache Airflow

## ⚙️ Tecnologias Utilizadas

- Python — processamento e lógica do pipeline
- Pandas — transformação e manipulação de dados
- Requests — ingestão via API
- Apache Airflow — orquestração e agendamento
- PostgreSQL — armazenamento de dados
- Docker Compose — ambiente isolado e reproduzível
- Git & GitHub — versionamento

## 📁 Estrutura do Projeto

.
├── dags/                # DAGs do Airflow (orquestração)
├── src/                 # Scripts de ETL (extract, transform, load)
├── config/              # Configurações e variáveis de ambiente
├── data/                # Dados locais (entrada/saída)
├── notebooks/           # Exploração e testes
├── docker-compose.yaml  # Infraestrutura local
├── main.py              # Execução local do pipeline
└── requirements.txt     # Dependências do projeto

## 🔄 Fluxo do Pipeline

1. Extract
   Coleta de dados a partir de uma API externa

2. Transform
   Limpeza, tratamento e padronização dos dados

3. Load
   Inserção dos dados estruturados no PostgreSQL

4. Orquestração
   Execução automatizada e agendada via Airflow

## 🚀 Como Executar

1. Clone o repositório:

git clone https://github.com/ryandias03/tutorial_pipeline.git
cd tutorial_pipeline

2. Crie um arquivo .env com as variáveis necessárias

3. Suba os serviços:

docker compose up -d

4. Acesse o Airflow no navegador

5. Execute a DAG do pipeline

## 📊 Resultado

Pipeline automatizado capaz de:
- Coletar dados externos
- Processar e estruturar informações
- Persistir dados em banco relacional
- Executar fluxos de forma automatizada

## 🔮 Evoluções Futuras

- Integração com Apache Spark ou Databricks
- Implementação de logging estruturado
- Monitoramento e alertas de falhas
- Testes automatizados de pipeline
- Evolução para arquitetura com Data Lake ou Lakehouse

## 👨‍💻 Autor

Ryan Augusto Dias da Cruz
GitHub: https://github.com/ryandias03