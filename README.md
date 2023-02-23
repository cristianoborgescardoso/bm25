# BM25 – Best Match 25

O BM25 é tido com uma evolução do tf-idf, sendo resultado de uma série de experimentos com variações do modelo probabilístico. Ele incorpora normalização e frequência do termo,tornando o modelo mais robusto. Como um modelo baseado em funções probabilísticas, o BM25 tenta responder qual a probabilidade de um documento _d_ ser relevante quando um usuário utiliza uma consulta _q_. 

Dada uma consulta (q), contendo os termos _t 1 , t 2 , . . . , t n_ , a função de pontuação para um documento d é dada por:
![alt text](https://github.com/cristianoborgescardoso/bm25/raw/main/bm25.png)
