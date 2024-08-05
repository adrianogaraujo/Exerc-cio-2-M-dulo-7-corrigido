### README do Projeto: Análise de Crédito usando Árvore de Decisão

#### Descrição Geral
Este projeto envolve a criação e avaliação de um modelo de árvore de decisão para classificar propostas de crédito como 'aprovadas' ou 'reprovadas'. Utilizando dados de um arquivo CSV com informações sobre posse de veículo, imóvel, quantidade de filhos, tipo de renda, educação, estado civil, entre outros, o modelo visa ajudar na tomada de decisões de crédito de forma mais eficiente e automatizada.

#### Preparação dos Dados
1. **Carregamento da Base de Dados:** A base de dados é carregada e pré-processada para garantir que todos os dados categóricos sejam convertidos em formatos numéricos através do método de One-Hot Encoding, e que nenhum valor faltante persista no conjunto de dados.

2. **Divisão da Base:** A base é dividida em 70% para treinamento e 30% para validação. Cada conjunto é separado em variáveis explicativas e a variável resposta (`mau`).

#### Modelo de Árvore de Decisão
1. **Criação e Treinamento do Modelo:** Um modelo de árvore de decisão é definido com uma profundidade máxima de 5 e treinado com os dados de treinamento.

2. **Visualização:** A árvore de decisão é visualizada para entender as decisões tomadas pelo modelo.

3. **Avaliação com Matriz de Confusão:** A matriz de confusão é utilizada para avaliar o desempenho do modelo no conjunto de treinamento, e a acurácia é calculada.

#### Avaliação do Modelo
1. **Teste do Modelo:** O modelo é aplicado ao conjunto de validação para prever as classificações e a acurácia é calculada e comparada com a acurácia de treinamento.

2. **Treinamento de uma Nova Árvore de Decisão:** Uma nova árvore é treinada com diferentes parâmetros para explorar outros aspectos do desempenho do modelo.

3. **Proporção de Classificações:** A proporção de proponentes classificados como 'maus' é calculada para a nova árvore.

4. **Experimento de Classificação:** Um experimento é conduzido para determinar a acurácia se todos os contratos fossem classificados como 'bons', mostrando a importância do modelo na identificação de proponentes de risco.

#### Conclusões
O projeto demonstra como a árvore de decisão pode ser utilizada para automatizar decisões de crédito, com alto nível de acurácia no conjunto de treinamento e validação. Futuras iterações podem explorar outros modelos e ajustes de parâmetros para otimizar ainda mais o desempenho.

### Como Executar o Projeto
- Garanta que todas as dependências, como pandas e scikit-learn, estejam instaladas.
- Execute o script em um ambiente Python adequado, preferencialmente um que suporte visualizações gráficas para a árvore de decisão e matrizes de confusão.
- O código pode ser executado diretamente, desde que o arquivo CSV esteja disponível no caminho especificado no script.

Este README oferece uma visão abrangente sobre a preparação, modelagem e avaliação no projeto de análise de crédito utilizando árvores de decisão.
