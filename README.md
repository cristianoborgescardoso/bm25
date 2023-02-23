# BM25 – Best Match 25 

O BM25 é tido com uma evolução do tf-idf, sendo resultado de uma série de experimentos com variações do modelo probabilístico. Ele incorpora normalização e frequência do termo,tornando o modelo mais robusto. Como um modelo baseado em funções probabilísticas, o BM25 tenta responder qual a probabilidade de um documento _d_ ser relevante quando um usuário utiliza uma consulta _q_. 

O BM25 é o modelo de busca padrão de várias _search engines_ como: [Apache Lucene](https://lucene.apache.org/), [Elastic](https://www.elastic.co/) e [Apache Solr](https://solr.apache.org/)

Dada uma consulta (q), contendo os termos _t 1 , t 2 , . . . , t n_ , a função de pontuação para um documento d é dada por:
![alt text](https://github.com/cristianoborgescardoso/bm25/raw/main/bm25.png)

A fórmula do BM25 é muito similar à fórmula do tf-idf, no qual ele é baseado, sendo uma das principais diferenças o uso das constantes k, b e L para tentar equilibrar possíveis distorções, devidas a repetição de palavras, e variações no comprimento dos documentos. 

Com a normalização do tamano do documento o BM25 dá chance aos documentos pequenos de “lutar” contra documentos longos por um lugar no ranking. O valor de _b_ permite controlar o grau de normalização entre documentos longos e curtos e o valor de _k_ fornece um meio de pontuar a repetição de uma mesma palavra.

# Sobre o Chat GPT
Eu fiz o curso de Mineração de Dados Completos(MDC) no IC, já conhecia, mas não lembrava como funcionava o BM25, tive que revisar o material do curso. Por isso quase não usei o ChatGPT para aprender sobre o BM25. Ele me ajudou muito em geração de códigos específicos para o meu problema, por exemplo, como fazia tempo que eu não programava em Python, o ChatGPT criou vários esqueletos do código, que muitas vezes não executavam corretamente, apresentava problemas de importação, pacotes não pertenciam as bibliotecas, chamada funções com parametros errados etc. Ainda assim, só por fornecer o esqueleto da soluções algumas respostas específicas já me poupou muito tempo.

Eu não havia percebido que a solução deveria usar a base de dados CISI e já estava com uma solução pronta, usando uma coleção de documentos simples. Quando me dei conta da obrigatoriedade do uso do CISI, pensei que só ChatGPT não seria suficiente para terminar o trabalho a tempo, então procurei mais informações em outras fontes. As principais fontes foram o materia das aulas do curso de MDC, [Stanford CS124 class Week 4](https://www.youtube.com/channel/UC_48v322owNVtORXuMeRmpA), codigos [https://www.kaggle.com/](Kaggle) e [github](https://github.com/williamscott701/Information-Retrieval/blob/master/2.%20TF-IDF%20Ranking%20-%20Cosine%20Similarity%2C%20Matching%20Score/TF-IDF.ipynb).   
