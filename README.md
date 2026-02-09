# 🏢 Análise de Mercado Imobiliário - Rio de Janeiro

## 📌 Visão Geral

Este projeto simula a atuação de uma **cientista de dados em uma empresa imobiliária do Rio de Janeiro**, executando um pipeline completo de limpeza, exploração e preparação de dados.

O objetivo foi transformar uma base bruta de preços de aluguel em um dataset estruturado, pronto para alimentar modelos de Machine Learning e dashboards de tomada de decisão.

---

## 🎯 Objetivo do Projeto

Preparar dados de imóveis para suportar dois times dentro da organização:
- **Time de Machine Learning**: dados limpos e tratados para treinar modelos preditivos
- **Time de Desenvolvimento**: estrutura de dados para integração no site da empresa

---

## 📊 Dataset

| Aspecto | Descrição |
|--------|-----------|
| **Origem** | Base de dados de aluguel de imóveis do Rio de Janeiro |
| **Tamanho** | Diversos tipos de imóveis (apartamentos, casas, comércios, etc.) |
| **Período** | Dados reais de mercado RJ |
| **Link** | [aluguel.csv](https://raw.githubusercontent.com/alura-cursos/pandas-conhecendo-a-biblioteca/main/base-de-dados/aluguel.csv) |

### 📋 Variáveis Principais
- **Preços**: Aluguel, condomínio, IPTU
- **Características do imóvel**: Quartos, suítes, vagas de garagem, tipo de imóvel
- **Localização**: Bairros e regiões do Rio de Janeiro

---

## 🔧 Metodologia

O projeto foi desenvolvido em **7 etapas principais**:

### 1️⃣ **Importação e Exploração Inicial**
   - Carregamento da base de dados com Pandas
   - Visualização das primeiras linhas e informações gerais
   - Identificação de tipos de dados e dimensões do dataset

### 2️⃣ **Análise Exploratória (EDA)**
   - Estatísticas descritivas (média, mediana, desvio padrão)
   - Distribuição de preços por tipo de imóvel
   - Análise de correlações entre variáveis numéricas
   - Visualizações para identificar padrões e outliers

### 3️⃣ **Tratamento de Valores Nulos**
   - Identificação de missing values
   - Estratégias de preenchimento ou remoção conforme necessário
   - Documentação de decisões tomadas

### 4️⃣ **Remoção de Registros Inconsistentes**
   - Validação de valores lógicos
   - Remoção de duplicatas
   - Tratamento de outliers significativos

### 5️⃣ **Aplicação de Filtros**
   - Seleção de dados relevantes para análise
   - Criação de subconjuntos para diferentes cenários de negócio

### 6️⃣ **Criação de Novas Colunas**
   - **Variáveis numéricas**: Razões entre preços, custos totais, etc.
   - **Variáveis categóricas**: Segmentação de preços, classificação de imóveis

### 7️⃣ **Salvamento de Dados Tratados**
   - Exportação do dataset limpo e estruturado
   - Pronto para uso em pipelines analíticos e modelos ML

---

## 📈 Principais Insights

### 📊 Dataset em números:
- **Total de registros**: 32.960 imóveis
- **Tipos de imóvel**: 22 categorias diferentes
- **Bairros mapeados**: 162 bairros do Rio de Janeiro
- **Variação de preços**: De R$ 0 a R$ 120 milhões mensais

### 🏆 Descobertas Principais:

**Por Tipo de Imóvel (Maior Aluguel Médio):**
1. **Prédio Inteiro**: R$ 498.637 (maior valor)
2. **Indústria**: R$ 120.000
3. **Galpão/Depósito/Armazém**: R$ 53.407
4. **Terreno Padrão**: R$ 32.568

**Por Tipo de Imóvel (Maior Demanda - Apartamentos):**
- **Apartamento**: Média de R$ 4.744
- **Quitinete**: Média de R$ 1.246 (entrada do mercado)
- **Loft**: Média de R$ 2.557

**Características do Dataset:**
- ✅ Imóveis com **1 a 100 quartos** (outliers identificados)
- ✅ Vagas de garagem variam de **0 a 1.966**
- ✅ Áreas de **0 a 90.000 m²**
- ✅ Condominais de **R$ 0 a R$ 6.5 milhões**

### 🔧 Processamento Realizado:

- ✅ **32.960 registros analisados** e validados
- ✅ **Valores nulos tratados** e documentados
- ✅ **Registros inconsistentes removidos** (garagens com 1.966 vagas, áreas de 90.000m²)
- ✅ **Novas variáveis criadas**: Valor por mês, Valor por ano, Descrição, Possui suite
- ✅ **Dados estruturados** para pipelines de ML e web (22 tipos, 162 bairros)
- ✅ **Padrões identificados** entre características e valores de aluguel

---

## 💻 Tecnologias Utilizadas

```
🐍 Python 3
📊 Pandas - Manipulação e limpeza de dados
📈 NumPy - Operações numéricas
📉 Matplotlib & Seaborn - Visualizações
🔗 Google Colab - Ambiente de desenvolvimento
```

---

## 🚀 Como Reproduzir

### Pré-requisitos
```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
```

### Execução
1. Clone o repositório
2. Abra o notebook no Jupyter ou Google Colab
3. Execute as células na ordem sequencial
4. Os dados tratados serão salvos automaticamente

---

## 📁 Estrutura do Projeto

```
📦 analise-imovel-rj/
├── 📓 analise_imovel_rj.ipynb    # Notebook principal
├── 📄 README.md                  # Este arquivo
├── 📊 aluguel.csv               # Dataset original
└── 💾 aluguel_tratado.csv       # Dataset após tratamento
```

---

## 🎓 Aprendizados

Este projeto consolidou conhecimentos em:
- ✅ **Data Cleaning**: Tratamento rigoroso de dados brutos
- ✅ **EDA (Análise Exploratória)**: Interpretação de dados para insights de negócio
- ✅ **Feature Engineering**: Criação de variáveis significativas
- ✅ **Documentação**: Código limpo, comentado e reprodutível
- ✅ **Pensamento Analítico**: Solução de problemas reais de negócio

---

## 📚 Contexto

- **Realizado em**: 04/02/2026
- **Formação**: ONE by Alura (G9)
- **Case idealizado por**: Alura
- **Autor**: Danielli Arçari

---

## 🔗 Links Relacionados

- 📊 [Notebook (Google Colab)](https://colab.research.google.com/drive/18j3lyj1iHOhvCv0-28zUvkAuTeoPNiJe)
- 💼 [LinkedIn](https://www.linkedin.com/in/danielli-arcari/)
- 🌐 [Portfólio Completo](https://danielli-arcari.github.io/)
- 📧 **Email**: axiadmc@gmail.com

---

## 💡 Possíveis Extensões Futuras

- 📊 Criação de dashboard interativo (Power BI/Tableau)
- 🤖 Desenvolvimento de modelo preditivo de preços
- 📍 Análise geoespacial dos imóveis
- 🔮 Análise de tendências temporais do mercado

---

**Este projeto demonstra capacidade de executar pipelines de dados completos, desde limpeza até preparação para uso analítico em ambiente corporativo.**

*Desenvolvido com foco em qualidade, reprodutibilidade e impacto de negócio.*
