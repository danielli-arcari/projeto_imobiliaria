# projeto_imobiliaria

🏢 Análise de Mercado Imobiliário - Rio de Janeiro

📌 Visão Geral:
Este projeto simula a atuação de uma cientista de dados em uma empresa imobiliária do Rio de Janeiro, executando um pipeline completo de limpeza, exploração e preparação de dados.
O objetivo foi transformar uma base bruta de preços de aluguel em um dataset estruturado, pronto para alimentar modelos de Machine Learning e dashboards de tomada de decisão.

🎯 Objetivo do Projeto:
Preparar dados de imóveis para suportar dois times dentro da organização:
a)Time de Machine Learning: deseja dados limpos e tratados para treinar modelos preditivos
b)Time de Desenvolvimento: deseja boa estrutura de dados para integração no site da empresa

📊 Dataset:
AspectoDescriçãoOrigemBase de dados de aluguel de imóveis do Rio de JaneiroTamanhoDiversos tipos de imóveis (apartamentos, casas, comércios, etc.)PeríodoDados reais de mercado RJLinkaluguel.csv

📋 Variáveis Principais:

-Preços: Aluguel, condomínio, IPTU
-Características do imóvel: Quartos, suítes, vagas de garagem, tipo de imóvel
-Localização: Bairros e regiões do Rio de Janeiro

🔧 Metodologia
O projeto foi desenvolvido em 7 etapas principais:

1️⃣ Importação e Exploração Inicial:

-Carregamento da base de dados com Pandas
-Visualização das primeiras linhas e informações gerais
-Identificação de tipos de dados e dimensões do dataset

2️⃣ Análise Exploratória (EDA):

-Estatísticas descritivas (média, mediana, desvio padrão)
-Distribuição de preços por tipo de imóvel
-Análise de correlações entre variáveis numéricas
-Visualizações para identificar padrões e outliers

3️⃣ Tratamento de Valores Nulos:

-Identificação de missing values
-Estratégias de preenchimento ou remoção conforme necessário
-Documentação de decisões tomadas

4️⃣ Remoção de Registros Inconsistentes:

-Validação de valores lógicos
-Remoção de duplicatas
-Tratamento de outliers significativos

5️⃣ Aplicação de Filtros:

-Seleção de dados relevantes para análise
-Criação de subconjuntos para diferentes cenários de negócio

6️⃣ Criação de Novas Colunas:

-Variáveis numéricas: Razões entre preços, custos totais, etc.
-Variáveis categóricas: Segmentação de preços, classificação de imóveis

7️⃣ Salvamento de Dados Tratados:

-Exportação do dataset limpo e estruturado
-Pronto para uso em pipelines analíticos e modelos ML


📈 Principais Insights:

Através desta análise, foi possível:

-Identificar os bairros mais caros e mais baratos do Rio de Janeiro
-Analisar tipos de aluguel com maior demanda e valor
-Segmentar imóveis por categoria de preço e características
-Preparar dados com alta qualidade para alimentar modelos preditivos
-Documentar todo o processo de tratamento para reprodutibilidade


💻 Tecnologias Utilizadas:

🐍 Python 3
📊 Pandas - Manipulação e limpeza de dados
📈 NumPy - Operações numéricas
📉 Matplotlib & Seaborn - Visualizações
🔗 Google Colab - Ambiente de desenvolvimento

🚀 Como Reproduzir:

Pré-requisitos:
pythonimport pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

Execução:

-Clone o repositório
-Abra o notebook no Jupyter ou Google Colab
-Execute as células na ordem sequencial
-Os dados tratados serão salvos automaticamente


📁 Estrutura do Projeto:

📦 analise-imovel-rj/
├── 📓 analise_imovel_rj.ipynb    # Notebook principal
├── 📄 README.md                  # Este arquivo
├── 📊 aluguel.csv               # Dataset original
└── 💾 aluguel_tratado.csv       # Dataset após tratamento

🎓 Aprendizados:

Este projeto consolidou conhecimentos em:

✅ Data Cleaning: Tratamento rigoroso de dados brutos
✅ EDA (Análise Exploratória): Interpretação de dados para insights de negócio
✅ Feature Engineering: Criação de variáveis significativas
✅ Documentação: Código limpo, comentado e reprodutível
✅ Pensamento Analítico: Solução de problemas reais de negócio


📚 Contexto:

Realizado em: 04/02/2026
Formação: ONE by Alura (G9)
Case idealizado por: Alura
Autor: Danielli Arçari


🔗 Links Relacionados:

📊 Notebook (Google Colab)
💼 LinkedIn
🌐 Portfólio Completo
📧 Email: axiadmc@gmail.com


💡 Possíveis Extensões Futuras:

📊 Criação de dashboard interativo (Power BI/Tableau)
🤖 Desenvolvimento de modelo preditivo de preços
📍 Análise geoespacial dos imóveis
🔮 Análise de tendências temporais do mercado


Este projeto demonstra capacidade de executar pipelines de dados completos, desde limpeza até preparação para uso analítico em ambiente corporativo.
Desenvolvido com foco em qualidade, reprodutibilidade e impacto de negócio.
