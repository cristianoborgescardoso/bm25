# BM25 – Best Match 25

O BM25 é tido com uma evolução do tf-idf, sendo resultado de uma série de experimentos com variações do modelo probabilístico. Ele incorpora normalização e frequência do termo,tornando o modelo mais robusto. Como um modelo baseado em funções probabilísticas, o BM25 tenta responder qual a probabilidade de um documento _d_ ser relevante quando um usuário utiliza uma consulta _q_. 

Dada uma consulta (q), contendo os termos _t 1 , t 2 , . . . , t n_ , a função de pontuação para um documento d é dada por:
![alt text](https://github.com/cristianoborgescardoso/bm25/raw/main/bm25.png)

A fórmula do BM25 é muito similar à fórmula do tf-idf, no qual ele é baseado, sendo uma das principais diferenças o uso das constantes k, b e L para tentar equilibrar possíveis distorções, devidas a repetição de palavras, e variações no comprimento dos documentos. 

Com a normalização do tamano do documento o BM25 dá chance aos documentos pequenos de “lutar” contra documentos longos por um lugar no ranking. O valor de _b_ permite controlar o grau de normalização entre documentos longos e curtos e o valor de _k_ fornece um meio de pontuar a repetição de uma mesma palavra.
