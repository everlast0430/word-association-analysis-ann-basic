word associate analysis using ANN Basic
# Summary

Prediction based Embedding 기반의 기본적인 ANN(Artifical Neural Network) 신경망을 활용하여 Word2Vec을 진행하였고 그 결과를 유클리디안 거리를 이용해 “OO”이라는 단어와 가장 잘 조합되고 연결되어 사용될 수 단어는 무엇이 있는지를 분석하였음

# Problem

도메인 경험적으로 “OO”이라는 대분류 속에 하위 분류가 무엇이 존재할 수 있는지 판단해볼 수도 있지만 데이터적으로 판단이 필요하였음 

Frequency based Embedding 기반의 TF-IDF 는 특정 주제 또는 단어의 변화추이 및 어떤것이 주요한 이슈가 되는지 알 수 있지만 주제 또는 단어간의 자주 조합되거나 연결되는 것이 무엇이지 파악하기 어려움

예를 들어, “엄마”와 “아빠”라는 단어는 “엄마”와 “케첩” 또는 “아빠”와 “버터”라는 단어들 보다 서로 가까이 존재하고 있어야 함

즉, “OO”과 밀접하게 조합되고 연결되어 사용될 수 있는 단어임에도 불구하고 Frequency based Embedding 방식은 해당 단어들이 서로 가까이 있는지 없는지 알 수 없었음

# Goal

“OO”이라는 단어와 가장 자주 나타나고 연관될 수 있는 단어는 무엇 그 단어들이 얼마나 가까이 존재하고 있는지 판단하는 것이 목표

# Process

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/ecafc9d5-2001-4bd1-8e09-7614012478e3/e980fa57-b3e7-4f79-9af2-8c1ebf195acb/Untitled.png)

전체 프로세스

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/ecafc9d5-2001-4bd1-8e09-7614012478e3/162ff69d-6265-4bf8-bd88-9f4780b9495b/Untitled.png)

# Reference

https://medium.com/@hari4om/word-embedding-d816f643140
https://cmry.github.io/notes/euclidean-v-cosine
https://towardsdatascience.com/creating-word-embeddings-coding-the-word2vec-algorithm-in-python-using-deep-learning-b337d0ba17a8
https://towardsdatascience.com/all-you-need-to-know-to-build-your-first-llm-app-eb982c78ffac
