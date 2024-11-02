🧬 Projeto de Segmentação de Células Sanguíneas com Watershed

Este projeto utiliza técnicas de processamento de imagem e o algoritmo Watershed para realizar a segmentação de células sanguíneas em imagens. O objetivo é identificar e contar as células presentes na imagem, aplicando uma série de operações de processamento para melhorar a segmentação e obter estatísticas sobre as células.

🎯 Objetivo

Utilizar o algoritmo Watershed para segmentar células sanguíneas em imagens microscópicas.

Aplicar diferentes operações de pré-processamento e morfologia matemática para definir as áreas de fundo e foreground.

Calcular estatísticas relevantes, como o número total de células detectadas.

🛠 Tecnologias e Ferramentas Usadas

Linguagem: Python

Bibliotecas:

opencv-python-headless: Para operações de processamento de imagem e segmentação.

numpy: Para manipulação de arrays e operações matemáticas.

matplotlib: Para visualização dos resultados e gráficos.

📂 Estrutura do Projeto

Carregamento e Pré-processamento da Imagem:

Carrega a imagem em escala de cinza e aplica um filtro de suavização (gaussian, bilateral ou median) para reduzir o ruído e melhorar a segmentação.

Limiarização e Operações Morfológicas:

Utiliza limiarização adaptativa para separar o foreground (células) do background. Também aplica uma operação morfológica de abertura para remover pequenos ruídos.

Definição dos Marcadores para Watershed:

Define as áreas de fundo e foreground usando operações morfológicas, Transformada de Distância, e closing para unir bordas quebradas. Cria os marcadores que serão utilizados pelo algoritmo Watershed.

Aplicação do Algoritmo Watershed:

Segmenta as células utilizando os marcadores gerados. As bordas das células são destacadas em vermelho para facilitar a visualização.

Cálculo de Estatísticas das Células:

Calcula o número total de células detectadas e imprime o resultado.

🧠 Etapas do Projeto

1. Carregar e Pré-processar a Imagem

A imagem de células sanguíneas é carregada em escala de cinza e um filtro de suavização é aplicado. Isso ajuda a reduzir o ruído e a melhorar a segmentação subsequente. Os tipos de filtros disponíveis são:

Gaussian Blur: Suavização por média ponderada.

Bilateral Filter: Suavização que preserva bordas.

Median Blur: Suavização baseada na mediana dos pixels vizinhos.

2. Aplicação de Limiarização Adaptativa

Utiliza a limiarização adaptativa para converter a imagem em binária, separando as áreas de foreground (células) do background. Também são aplicadas operações morfológicas para reduzir ruídos e melhorar a qualidade da segmentação.

3. Definir Marcadores para Watershed

Utiliza operações de Transformada de Distância e closing para definir as áreas de foreground, background e áreas desconhecidas. Os marcadores criados são usados pelo algoritmo Watershed para segmentar as células.

4. Aplicar o Algoritmo Watershed

Com os marcadores definidos, o algoritmo Watershed é aplicado para segmentar as células na imagem original. As bordas detectadas são destacadas em vermelho.

5. Calcular Estatísticas das Células

Calcula e exibe o número total de células detectadas na imagem.

📊 Resultados Encontrados

Durante os experimentos, o algoritmo Watershed foi aplicado para segmentar as células sanguíneas e calcular o número total de células. A imagem foi pré-processada e segmentada, e os seguintes resultados foram obtidos:

Imagem Pré-processada: A suavização ajuda a reduzir ruídos e melhora a segmentação.

Imagem Limiarizada: A limiarização adaptativa separa foreground e background.

Segmentação com Watershed: O algoritmo Watershed identifica e separa as células, destacando as bordas.

Exemplos de Resultados

Imagem Pré-processada



Imagem Limiarizada



Segmentação com Watershed



🚀 Próximos Passos

Ajustar Hiperparâmetros das Operações Morfológicas:

Testar diferentes tamanhos de kernel e número de iterações para melhorar a segmentação.

Implementar Widgets Interativos:

Utilizar ipywidgets para ajustar dinamicamente os parâmetros de limiarização e operações morfológicas no Jupyter Notebook.

Avaliação de Qualidade:

Adicionar métricas de avaliação da segmentação, como Coeficiente de Similaridade de Dice, para quantificar a precisão da segmentação.

📊 Base de Dados Utilizada

Este projeto utilizou imagens de células sanguíneas do dataset All Cell Data. As imagens foram processadas em escala de cinza e pré-processadas para melhorar a qualidade da segmentação.

👤 Autor

Guilherme Koiti Tanaka SassakiLinkedIn
