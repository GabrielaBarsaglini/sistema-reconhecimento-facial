Reconhecimento Facial com TensorFlow, MTCNN e FaceNet

Este projeto implementa um sistema de detecção e reconhecimento facial utilizando:

MTCNN → detecção de rostos.

FaceNet (Keras-Facenet) → extração de embeddings faciais.

SVM (Scikit-learn) → classificação de rostos a partir dos embeddings.

Dataset LFW (Labeled Faces in the Wild) → base pública de rostos.


Detectar múltiplas faces em imagens.

Extrair representações vetoriais (embeddings) com FaceNet.

Treinar um classificador SVM para reconhecer as pessoas.

Avaliar o modelo e visualizar as predições com imagens e rótulos.


🔧 Tecnologias

Python 3

TensorFlow / Keras

OpenCV

MTCNN

Keras-Facenet

Scikit-learn

Matplotlib


 Pipeline

Carregamento do dataset

fetch_lfw_people do Scikit-learn.

Rostos com ≥20 aparições.

Pré-processamento

Redimensionamento para (160,160,3).

Normalização para [0,1].

Extração de embeddings

Usando FaceNet pré-treinado.

Treinamento do classificador

SVM com kernel RBF.

Avaliação

classification_report e matriz de confusão.

Visualização das predições com matplotlib.



Quer que eu monte também um guia de instalação (com requirements.txt) para rodar fora do Colab?
