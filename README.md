# Classificacao_Veiculos_Machine_Learning
Classificação de veículos usando modelos de Machine Learning
Este projeto consiste em:
-Leitura do arquivo csv usando Pandas, depois salvando na variável "dados" e exibindo os 10 primeiros registros do DataFrame.

-Substituição dos nomes das colunas do DataFrame por nomes em português.

-Alteração dos valores da coluna vendido ('no', 'yes') para (0,1). Usando a função Map para realizar essa alteração.

-Utilização do datetime.today().year que retorna o ano atual e armazenando o valor na variável "ano_atual" depois criaremos uma nova coluna que receberá a subtração do ano atual menos os anos da coluna "ano_do_modelo" que resultará na coluna chamada 'idade_do_modelo'.

-Inclusão de uma nova coluna ao Dataframe que receberá todos os valores da coluna 'milhas-por_ano' que serão multiplicados pela constante (1.60934) para ocorrer a transformação dos valores em milhas para quilômetros resultando na nova coluna 'km_por_ano'.

-Excluindo as colunas que não serão usadas para o nosso projeto.

Definindo uma função que recebe o modelo:
-Divide o Dataframe em dois, um Dataframe com todas as variáveis menos a alvo e outro com a variável alvo.
-Padroniza um valor do SEED.
-Divide os DataFrames em conjuntos de treino e teste usando o tamanho dos DataFrames de teste sendo 25% do DataFrames originais, o parâmetro "stratify" faz com que os novos DataFrames gerados matenham a mesma proporção de valores em relação aos Dataframes originais.
-Usaremos um 'if' para usarmos o StandardScaler apenas nos modelos LinearSVC e SVC que consiste em um padronizador de valores para que o modelo não comporte-se mal se as características individuais não se assemelharem mais ou menos a dados padrão normalmente distribuídos.
-Printamos a quantidade de dados que serão usados para treino e para teste.
-Ajustamos o modelo aos dados de treino.
-Predizemos baseados nos dados de teste.
-Por fim, imprimimos a acurácia do modelo.

-Uso da função para o modelo SVC(Support Vector Machine).
-Uso da função para o modelo LinearSVC.
-Uso da função para o modelo DummyClassifier para vermos se nossos modelos estão com uma acurácia aceitável.
-Uso da função para o modelo DecisionTreeClassifier.
-Plotagem gráfica da árvore de decisão do modelo DecisionTreeClassifier.
