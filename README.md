## Categorização de Tramitações de Projetos de Lei da Câmara dos Deputados

**Autora**: Fernanda Scovino (FGV-EMAp)

### Objetivo
---
Criar uma classificação das tramitações de Projetos de Lei da Câmara dos Deputados a partir da análise de proximidade do seus textos de descrição.

**Base de dados:** [Dados de andamento dos Projetos de Lei de 1988 a 2018, disponíveis na API dos Dados Abertos da Câmara](http://www2.camara.leg.br/transparencia/dados-abertos/dados-abertos-legislativo/webservices/orgaos/obterandamento)

### Metodologia

A partir dos dados de descrição das tramitações, vamos utilizar pacotes como `nltk`, `gensim` e `tfidf` para verificar a frequência e a similaridade de palavras nos textos para identificarmos palavras chaves. Essas palavras chaves vão servir futuramente para categorizarmos as tramitações de acordo com os *clusters* gerados pelo algoritmo de *Topic Model*.

### Referências

Análise Exploratória:

- [Notebook 8-EDA_Textual_Analysis](https://github.com/rsouza/FGV_Intro_DS/blob/master/notebooks/8-EDA_Textual_Analysis.ipynb)
- [Machine Learning, NLP: Text Classification using scikit-learn, python and NLTK](https://towardsdatascience.com/machine-learning-nlp-text-classification-using-scikit-learn-python-and-nltk-c52b92a7c73a)

Topic Model (a ser utilizado):

- [Notebook 9-ML_TopicModeling_Clustering_Documents](https://github.com/rsouza/FGV_Intro_DS/blob/master/notebooks/9-ML_TopicModeling_Clustering_Documents.ipynb)
- [Latent Dirichlet Allocation (LDA) with Python](https://rstudio-pubs-static.s3.amazonaws.com/79360_850b2a69980c4488b1db95987a24867a.html)
- [Topic Model: Beyond Bag-of-Words](http://people.ee.duke.edu/~lcarin/icml2006.pdf)
- [Unsupervised Topic Modeling for Short Texts Using Distributed
Representations of Words](http://www.aclweb.org/anthology/W15-1526)