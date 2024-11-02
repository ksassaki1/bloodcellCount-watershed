# 🧬 **Projeto de Contagem de Células com Processamento de Imagem**

Este projeto utiliza técnicas de **processamento de imagens** e **visão computacional** para realizar a **contagem e classificação de células** em imagens de microscópio. Os métodos aplicados envolvem detecção de bordas e transformadas para identificar e segmentar as células, permitindo avaliar o número de células presentes e suas características morfológicas.


## 🎯 **Objetivo**
- Desenvolver uma rotina para **segmentar** células utilizando técnicas de detecção de bordas (`Canny`) e segmentação (`Watershed`).

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
  - **Segmentação** de células usando algoritmos de detecção de bordas e transformadas.
  - **Visualização** dos resultados.

---

## 🧠 **Métodos Implementados**
- **Detecção de Bordas com Canny:**
  - A técnica de detecção de bordas de Canny é usada para identificar as bordas das células na imagem, permitindo destacar os contornos para posterior segmentação.

- **Watershed para Segmentação:**
  - A técnica de **Watershed** é utilizada para segmentar as células a partir dos marcadores gerados, permitindo identificar áreas sobrepostas e realizar uma segmentação precisa.

- **Operações Morfológicas:**
  - **Dilatação** e **erosão** são aplicadas para remover ruídos e melhorar a segmentação das células, facilitando a detecção precisa. Além disso, a operação de **fechamento (closing)** é utilizada para unir bordas quebradas em áreas de foreground, garantindo uma melhor definição das células segmentadas.

---

## 📊 **Resultados Encontrados**
Durante os experimentos, as técnicas de detecção de bordas e segmentação com Watershed foram aplicadas a diversas imagens de células, permitindo alguma segmentação de células presentes.


**Conclusão Geral**: As técnicas de processamento de imagem utilizadas foram capazes de identificar e segmentar células de forma promissora, permitindo realizar a contagem.

---

## 📊 **Exemplo da imagem segmentada**
Abaixo está a imagem segmentada após a aplicação dos processos:

### Imagem Segmentada com Watershed
![Imagem Segmentada com Watershed](img_watershed.png)

---

## 🚀 **Próximos Passos**
- **Melhorar a Precisão** na Detecção:
  - Ajustar os parâmetros de Watershed e da detecção de bordas para obter uma segmentação ainda mais precisa.
- **Dashboard Interativo**:
  - Desenvolver um dashboard utilizando **Streamlit** para permitir ao usuário visualizar as células segmentadas e obter estatísticas de forma interativa.

---

## 👤 **Autor**
Guilherme Koiti Tanaka Sassaki  
[LinkedIn](https://www.linkedin.com/in/guilherme-sassaki-10b81ba7/)

