## Building a Simple Information Retrieval System using BM25 and GPT-3 and evaluated in the CISI collection. ##

### Introdução ###
Este repositório apresenta a aplicação de conceitos básicos de Recuperação de Informação (IR) e do algoritmo de classificação BM25. 
O objetivo foi construir um sistema de IR simples para recuperação de documentos relevantes de um corpus pré-definido, baseado na consulta do usuário. O projeto foi desenvolvido usando notebook Google Colab, plataforma GitHub e ajuda do modelo de linguagem GPT-3 para encontrar soluções para os desafios enfrentados.

Neste relatório serão descritos os detalhes de implementação, resultados, como testar o sistema de IR e como o chatGPT ajudou no projeto.

### Implementação ###
O sistema de IR foi implementado usando o algoritmo de classificação BM25. O corpus usado foi a coleção CISI, que contém mais de 14.000 documentos. O primeiro passo foi realizar o pré-processamento do corpus, que envolveu a remoção de pontuação, stopwords e aplicação de stemming. Em seguida, os termos do corpus foram representados como vetores de frequência de termos (TF) e transformados em vetores de frequência de termos ponderados por inverso de documento (TF-IDF).

**CISI** - https://www.kaggle.com/datasets/dmaso01dsta/cisi-a-dataset-for-information-retrieval

A consulta do usuário foi processada de maneira semelhante, por meio de pré-processamento e representação como um vetor de frequência de termos ponderados por inverso de documento. Em seguida, os vetores de consulta foram comparados com os vetores de documentos usando a medida de similaridade BM25.

A implementação do sistema de IR foi feita usando a linguagem de programação Python e a biblioteca scikit-learn para a implementação do BM25.

### ChatGPT OpenAI ###

O modelo de linguagem GPT-3 foi usado para auxiliar na solução de problemas e codificação. O ChatGPT foi utilizado para fornecer ajuda em todas as fases do projeto. O modelo foi capaz de fornecer sugestões de soluções para problemas específicos e também ajudou a compreender melhor alguns conceitos do projeto. Através do chat, foi possível receber feedback e sugestões para melhorar o código e torná-lo mais eficiente.

### Resultados ###
O sistema de IR foi testado usando 30 consultas selecionadas aleatoriamente da coleção CISI. Para cada consulta, o sistema retornou uma lista de documentos ordenados por ordem de relevância. A avaliação de desempenho foi realizada usando as métricas de precisão e revocação, que medem a fração de documentos relevantes recuperados e a fração de documentos relevantes na coleção que foram recuperados, respectivamente.

Os resultados mostraram que o sistema de IR com o BM25 obteve um desempenho razoável na recuperação de documentos relevantes para as consultas. A precisão média foi de 0,14 e a revocação média foi de 0,29.

### Testando o sistema de IR ###
Para testar o sistema de IR, basta executar o código fornecido no Google Colab Notebook. O código usa a coleção CISI como corpus e as consultas de teste estão incluídas no notebook. O usuário pode modificar as consultas de teste para ver os resultados para outras consultas.

