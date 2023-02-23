# BM25 – Best Match 25 

O BM25 é tido com uma evolução do tf-idf, sendo resultado de uma série de experimentos com variações do modelo probabilístico. Ele incorpora normalização e frequência do termo,tornando o modelo mais robusto. Como um modelo baseado em funções probabilísticas, o BM25 tenta responder qual a probabilidade de um documento _d_ ser relevante quando um usuário utiliza uma consulta _q_. 

Dada uma consulta (q), contendo os termos _t 1 , t 2 , . . . , t n_ , a função de pontuação para um documento d é dada por:
![alt text](https://github.com/cristianoborgescardoso/bm25/raw/main/bm25.png)

A fórmula do BM25 é muito similar à fórmula do tf-idf, no qual ele é baseado, sendo uma das principais diferenças o uso das constantes k, b e L para tentar equilibrar possíveis distorções, devidas a repetição de palavras, e variações no comprimento dos documentos. 

Com a normalização do tamano do documento o BM25 dá chance aos documentos pequenos de “lutar” contra documentos longos por um lugar no ranking. O valor de _b_ permite controlar o grau de normalização entre documentos longos e curtos e o valor de _k_ fornece um meio de pontuar a repetição de uma mesma palavra.

# Sobre o Chat GPT
Eu fiz o curso de Mineração de Dados Completos(MDC) no IC e já conhecia como funcionava o BM25 e tenho uma implementação dele em R. Se fosse pra me basear só nas explicações do ChatGPt seria bem mais dificil esse trabalho. O ChatGPT é muito útil pra dar uma ajuda específica no códgio, por exemplo, como fazia tempo que eu não programava em Python, o ChatGPT em criar um esqueleto do código. Mas não foi muito mais que isso, com muita frequencia os codigos não executavam corretamente, ele mandava importrar uns pacotes que não pertenciam as bibliotecas, chamava funções com parametros errados e por aí vai. Ainda assim, só por fornecer o esqueleto da soluções algumas respostas específicas ja me poupou muito tempo.

Eu não havia percebido que a solução deveria usar a base de dados CISI, e já estava com uma solução pronta, usando uma coleção de documentos simples quando me dei conta que desse requisito vi que usando só o ChatGPT seria demorado terminar a tempo, então procurei mais informações em outroas fontes. As principais fontes foram o materia das aulas do curso de MDC, [Stanford CS124 class Week 4](https://www.youtube.com/channel/UC_48v322owNVtORXuMeRmpA), codigos [https://www.kaggle.com/](Kaggle) e [github](https://github.com/williamscott701/Information-Retrieval/blob/master/2.%20TF-IDF%20Ranking%20-%20Cosine%20Similarity%2C%20Matching%20Score/TF-IDF.ipynb).   
