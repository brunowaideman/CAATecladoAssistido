
# 🧠 EyeTracker com Coleta, Treinamento e Predição em Tempo Real

Este projeto implementa um sistema completo de *eye tracking* (rastreamento ocular), com coleta de dados via webcam, treinamento de modelos baseados em visão computacional e redes neurais, e utilização do modelo treinado para predição do olhar em tempo real.

---

## 📁 Estrutura do Projeto

- `1_collect_data.ipynb`: Interface para coletar imagens dos olhos, rosto e posição da cabeça, junto da posição de um alvo na tela.
- `2_train_model.ipynb`: Treinamento de um modelo de rede neural para estimar a posição do olhar a partir das imagens coletadas.
- `3_eyetracker.ipynb`: Código que utiliza o modelo treinado para prever, em tempo real, onde o usuário está olhando.
- `EyeTrackerEyeChimera.ipynb`: Alternativa com uso de detecção facial pelo modelo EyeChimera.
- `Ngram.ipynb` e `perplexidade.ipynb`: Avaliação de modelos de linguagem e complexidade de digitação, voltado para integração com teclado assistivo (opcional/experimental).

---

## ⚙️ Funcionalidades

- 📷 Coleta automática de imagens com webcam (olhos, rosto e posição da cabeça).
- 🎯 Interface gráfica com pygame para calibração e coleta de dados em diferentes regiões da tela.
- 🧠 Treinamento de modelo de aprendizado profundo com PyTorch para prever posição do olhar.
- 👁️ Rastreamento ocular em tempo real com predição do ponto de foco do usuário.
- 🧪 Visualização de cobertura da tela e taxa de coleta de dados.

---

## 🛠️ Requisitos

- Python 3.8+
- Bibliotecas:
  - `pygame`
  - `cv2` (OpenCV)
  - `numpy`
  - `scipy`
  - `torch`
  - `matplotlib`

---

## 🚀 Como usar

### 1. Coletar dados

```bash
python collect_data.py
```

- Pressione `1` para calibrar (dados em pontos fixos).
- Pressione `2` para coletar dados com alvos móveis.
- Use `c` para mostrar a câmera e `s` para mostrar estatísticas.

### 2. Treinar o modelo

Execute o notebook:

```bash
2_train_model.ipynb
```

- Treina um modelo para prever a posição do olhar com base nas imagens dos olhos e rosto.

### 3. Usar o Eye Tracker

```bash
python eyetracker.py
```

- Pressione `3` para entrar no modo de rastreamento.
- O modelo usará a webcam para estimar em tempo real onde você está olhando.

---

## 📊 Dados gerados

Os dados são armazenados em:

- `data/face/`, `l_eye/`, `r_eye/`, etc: imagens coletadas.
- `data/positions.csv`: arquivo CSV com posição do alvo e ângulo da cabeça.
- `data/region_map.npy`: mapa da distribuição de coleta de dados na tela.

---

## 📌 Observações

- O sistema foi desenvolvido para pesquisas em interação assistiva.
- Pode ser adaptado para tarefas como controle por olhar, análise de atenção e sistemas alternativos de entrada.

---

## 🤝 Agradecimentos

Agradecemos ao Centro Universitário da FEI, ao Comitê de Ética e aos voluntários participantes do experimento pelos suportes para o desenvolvimento do presente trabalho.
