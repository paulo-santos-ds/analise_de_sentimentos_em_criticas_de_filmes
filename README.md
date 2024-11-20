# Análise de Sentimentos em Críticas de Filmes

## 📋 Descrição do Projeto
Este projeto visa desenvolver um sistema para filtrar e categorizar resenhas de filmes. O objetivo é treinar um modelo de Aprendizado de Máquina para detectar automaticamente resenhas negativas, utilizando um conjunto de dados de resenhas de filmes do IMDB com rotulagem de polaridade (positiva ou negativa).

## 📊 Estrutura dos Dados
O conjunto de dados possui os seguintes campos:

- `tcost`: Total cost (não presente nos dados fornecidos)
- `title_type`: Tipo do título
- `primary_title`: Título principal
- `original_title`: Título original
- `start_year`: Ano de início
- `end_year`: Ano de término
- `runtime_minutes`: Duração em minutos
- `is_adult`: Indicação se é conteúdo adulto
- `genres`: Gêneros
- `average_rating`: Avaliação média
- `votes`: Número de votos
- `review`: Revisão
- `rating`: Classificação
- `sp`: Não definido
- `pos`: Posição
- `ds_part`: Não definido
- `idx`: Índice

## 🛠️ Ferramentas e Bibliotecas Utilizadas
- **Python**: Linguagem principal utilizada para a análise.
- **Pandas** e **Numpy**: Bibliotecas para manipulação e análise de dados.
- **Sklearn** e **lightgbm**: Bibliotecas para construção de modelos de Machine Learning.
- **Matplotlib.pyplot** e **Seaborn**: Bibliotecas para construção de gráficos.
- **re**: Biblioteca para trabalhar com expressões regulares.
- **spacy**: Biblioteca de software de código aberto para processamento avançado de linguagem natural.

## 🔍 Metodologia
1. **Análise Exploratória de Dados**:
   - Importação das bibliotecas necessárias
   - Carregamento e visualização dos dados
   - Análise de dados ausentes e duplicados

2. **Análises**:
   - Número de filmes e resenhas ao longo dos anos
   - Distribuição do número de resenhas por filme
   - Distribuição de resenhas negativas e positivas ao longo dos anos

3. **Predição**:
   - Criação de uma função para treinar, testar e avaliar modelos de Machine Learning
   - Normalização de textos
   - Teste de modelos: Dummy, NLTK + TF-IDF + Regressão Linear, spaCy + TF-IDF + Regressão Linear, spaCy + TF-IDF + LGBMClassifier

4. **Aplicação dos Modelos**:
   - Análise de novas resenhas de filmes usando os modelos treinados

## Resultados
O modelo NLTK + TF-IDF + Regressão Linear apresentou os melhores resultados, com métricas superiores aos demais modelos testados, como F1-score, APS e ROC AUC.

## 📈 Aprendizados
- Análise exploratória de dados
- Preparação de dados para Machine Learning
- Construção e aplicação de funções
- Trabalho com textos (expressões regulares, vetorização, tokenização, lematização)
- Análise de sentimentos de textos
- Aplicação de modelos de Machine Learning
- Documentação de projetos
- Utilização de bibliotecas e ferramentas do ecossistema Python
- Tomada de decisões baseada em dados

## 🚀 Como Usar

1. Clone o repositório
```bash
 git clone https://github.com/paulo-santos-ds/previsao_total_corridas_taxi
```

2. Instale as dependências
```bash
pip install -r requirements.txt
```

3. Execute o notebook principal
```bash
Modelo_Preditivo_Corrida_Taxi.ipynb
```
