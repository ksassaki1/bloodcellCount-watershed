# 🧬 **Projeto de Contagem de Células com Processamento de Imagem**

Este projeto utiliza técnicas de **processamento de imagens** e **visão computacional** para realizar a **contagem e segmentação de células** em imagens de microscópio. Os métodos aplicados envolvem suavização de imagens, limiarização, operações morfológicas e segmentação usando o algoritmo **Watershed** para identificar e segmentar as células, permitindo avaliar o número de células presentes.

## 🎯 **Objetivo**
- Desenvolver uma rotina para **segmentar** células utilizando técnicas de **limiarização**, **operações morfológicas** e **segmentação (`Watershed`)**.
- Aplicar o algoritmo **Watershed** para realizar a segmentação precisa de células em imagens de microscópio.

---

## 🛠 **Tecnologias e Ferramentas Usadas**
- **Linguagem:** Python
- **Bibliotecas:**
  - `OpenCV`: Para processar as imagens e aplicar técnicas de detecção e segmentação.
  - `NumPy`: Para manipulação de arrays e operações matemáticas.
  - `Matplotlib`: Para visualização dos resultados.

---

## 📂 **Estrutura do Projeto**
### **Arquivos e Diretórios**
- **`blood_cell_count_watershed`**: Notebook principal contendo:
  - **Carregamento e pré-processamento** das imagens de células.
  - **Limiarização e operações morfológicas** para remover ruídos.
  - **Segmentação** de células usando o algoritmo `Watershed`.
  - **Visualização** dos resultados.

---

## 🧠 **Métodos Implementados**
- **Limiarização da Imagem**:
  - A técnica de **limiarização de Otsu** é usada para transformar a imagem em uma versão binária, destacando áreas de foreground e background.

- **Operações Morfológicas**:
  - **Abertura (`Opening`)** é aplicada para remover pequenos ruídos e **fechamento (`Closing`)** é usado para unir bordas desconectadas. Além disso, a **dilatação** e **transformada de distância** são aplicadas para definir áreas certas de fundo e foreground, facilitando a segmentação precisa.

- **Watershed para Segmentação**:
  - A técnica de **Watershed** é utilizada para segmentar as células a partir dos marcadores gerados, permitindo identificar áreas sobrepostas e realizar uma segmentação precisa.

---

## 📊 **Resultados Encontrados**
Durante os experimentos, as técnicas de limiarização, operações morfológicas e segmentação com Watershed foram aplicadas a diversas imagens de células, permitindo segmentar as células presentes.

**Conclusão Geral**: As técnicas de processamento de imagem utilizadas foram capazes de identificar e segmentar células de forma promissora, permitindo realizar a contagem.

---

## 📊 **Exemplo da imagem segmentada**
Abaixo está a imagem segmentada após a aplicação dos processos:

### Imagem Segmentada com Watershed
![Imagem Segmentada com Watershed](img_watershed.png)

**Nota**: A imagem foi retirada do dataset disponível em [all_CELL_data](https://github.com/akshaylamba/all_CELL_data).

---

## 🚀 **Próximos Passos**
- **Melhorar a Precisão** na Detecção:
  - Ajustar os parâmetros de Watershed e as operações morfológicas para obter uma segmentação ainda mais precisa.
- **Dashboard Interativo**:
  - Desenvolver um dashboard utilizando **Streamlit** para permitir ao usuário visualizar as células segmentadas e obter estatísticas de forma interativa.


---

## 👤 **Autor**
Guilherme Koiti Tanaka Sassaki  
[LinkedIn](https://www.linkedin.com/in/guilherme-sassaki-10b81ba7/)

