Este é o meu primeiro projeto prático com Redes Neurais Artificiais (ANN). O objetivo foi criar um modelo que conseguisse analisar as propriedades químicas de um vinho tinto e "adivinhar" a sua nota de qualidade (de 0 a 10).

utilizei o dataset Wine Quality e construí uma arquitetura de Perceptron Multicamadas (MLP). Tentei manter o equilíbrio entre uma rede inteligente, mas que não fosse apenas "memória", usando técnicas de regularização.

A "Anatomia" da minha Rede:

    Camadas Escondidas: Usei duas camadas para processar os dados.

    Funções de Ativação: Utilizei ReLU e Tanh. Elas ajudam a rede a entender padrões complexos que não são apenas linhas retas.

    Combate ao Overfitting: Adicionei uma camada de Dropout (20%). Basicamente, forcei a rede a não ficar dependente de poucos neurónios, o que a torna melhor a avaliar vinhos que nunca viu antes.

    Treino: O algoritmo de Backpropagation (via otimizador Adam) foi ajustando os pesos a cada erro cometido.

 Resultados

O treino correu muito bem! Como podes ver no gráfico de perda (Loss), a rede aprendeu rapidamente nas primeiras épocas e depois estabilizou.

    Erro Médio (MAE): Cheguei a um valor próximo de 0.45.
