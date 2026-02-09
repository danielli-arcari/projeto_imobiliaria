# Análise de Dados do Mercado Imobiliário do Rio de Janeiro

## Por que fiz esse projeto

Eu estava na formação ONE by Alura e recebi um desafio: preparar dados de imóveis para um time de Machine Learning e outro de Desenvolvimento Web. Achei interessante porque mostra bem como a realidade de um cientista de dados - você não recebe dados limpos, você precisa transformar dados brutos em algo que realmente funcione.

## Os dados

Trabalhei com um dataset de mais de 32 mil imóveis do Rio de Janeiro. Cada um tinha informações sobre:
- Tipo: apartamento, casa, quitinete, comercial, etc (22 categorias diferentes)
- Localização: 162 bairros do RJ
- Preço: aluguel mensal, valor de condomínio, IPTU
- Características físicas: número de quartos, suítes, vagas de garagem, área

## O que fiz

### 1. Exploração inicial
Comecei entendendo o tamanho do dataset, quais colunas tinha, tipos de dados, valores faltantes. O dataset tinha mais de 32 mil linhas - não é pequeno.

### 2. Limpeza pesada
- Identifiquei e removi quase 45 mil registros inconsistentes (valores extremos como garagens com 1.966 vagas, áreas de 90 mil m²)
- Tratei valores nulos de forma inteligente - algumas colunas simplesmente não aplicam a certos tipos de imóvel
- Retirei duplicatas
- No final fiquei com 284.627 registros validados

### 3. Análise exploratória
Comecei a fazer perguntas: qual tipo de imóvel é mais caro? Como os preços variam por bairro? Qual é a média de aluguel por categoria?

### 4. Feature engineering
Criei colunas novas que fizessem sentido:
- Valor por mês (agregando aluguel + condomínio + IPTU)
- Valor por ano (para ter visão anual)
- Descrição padronizada (tipo, bairro, número de quartos)
- Flag se tem suite ou não

### 5. Salvamento dos dados
Exportei tudo limpo e pronto para os times de ML e desenvolvimento usarem sem dor de cabeça

## O que vi nos dados

### Os tipos de imóvel mais caros em média
- Prédios inteiros (faz sentido): R$ 498.637
- Indústria: R$ 120.000
- Galpões: R$ 53.407
- Terrenos: R$ 32.568

### Pelo outro lado
- Quitinetes: R$ 1.246 (entrada do mercado)
- Lojas/Salões: R$ 13.769
- Lofts: R$ 2.557

### Cobertura geográfica
- 162 bairros diferentes mapeados (cobertura bem boa)
- 19 regiões integradas de segurança (RISP)

## Desafios que enfrentei

O maior desafio foi lidar com os outliers. Quando você tem 32 mil registros, sempre vai ter alguém que digitou algo errado. Tive que ser cuidadoso para não descartar dados legítimos, mas também não deixar valores claramente impossíveis deturpar a análise.

Os valores nulos também foram interessantes - em alguns casos significavam "não aplicável" (tipo, um comercial não tem "suítes"), em outros eram dados que realmente faltavam.

## Por que isso importa

Dados sujos = análises ruins = decisões ruins. Esse tipo de limpeza é trabalho que normalmente ninguém vê, mas é essencial. Um time de desenvolvimento não pode usar dados com 1.966 garagens registradas em um imóvel residencial. Um modelo de ML vai aprender errado.

## Ferramentas

Pandas para manipulação, NumPy para cálculos, Matplotlib e Seaborn para visualizar. Tudo no Google Colab porque era parte da formação ONE.

## O resultado

Entreguei dados estruturados, documentados, e prontos para uso. Qualidade que os times conseguem confiar.

## Links

- [Notebook no Colab](https://colab.research.google.com/drive/18j3lyj1iHOhvCv0-28zUvkAuTeoPNiJe?usp=sharing)
- [Repositório no GitHub](https://github.com/danielli-arcari/projeto_imobiliaria)
- [Meu portfólio](https://danielli-arcari.github.io/)
- [LinkedIn](https://www.linkedin.com/in/danielli-arcari/)
