# TCC2 – Sistema de Detecção de EPIs, Sonolência e Comportamentos Inseguros com visão computacional.

Este projeto detecta automaticamente a presença e o uso correto de Equipamentos de Proteção Individual (EPIs), sinais de sonolência, uso de celular e alimentação, emitindo alertas sonoros em decorrência de comportamento de risco em ambientes industriais, civis, e laboratório, utilizando ferramentas de inteligência artificial e machine learling como YOLOv8, MediaPipe, OpenCV e alarmes sonoros.

## 🔍 Funcionalidades

- ✅ Detecção de EPIs: capacete, óculos, colete, máscara, touca, bota, protetor auricular.
- ✅ Verificação de posicionamento correto dos EPIs
- 😴 Detecção de sonolência com MediaPipe (face mash)
- 📱 Detecção de uso de celular e alimentação
- 🔊 Alertas sonoros ou visuais diferentes para cada situação
- 🟢 Diagnóstico com texto e cor na tela (verde: normal, vermelho: alerta)
- 📊 Emitir diagnóstico de taxa de confiabilidade
- 💻 Suporte para execução em Raspberry Pi 4

## 🧠 Tecnologias Utilizadas

- YOLOv8 (Ultralytics)
- MediaPipe (FaceMesh e Pose)
- OpenCV
- Python 3.10+
- Pygame (para alarmes sonoros)

## 🗂 Estrutura

TCC2/
│
├── mein.py
├── requirements.txt          ← (lista de bibliotecas usadas)
├── README.md                 ← (explicação do projeto)
├── modelos/
│   └── best.pt               ← (modelo YOLO treinado)
├── som/
│   ├── alerta_sonolencia.mp3
│   ├── alerta_epi.mp3
│   └── ...
├── dataset_epi_unificado/
│   ├── images/
│   ├── labels/
│   └── ...
├── yolov8/
│   └── ...                   ← (se você incluiu YOLO no projeto)


## 🚀 Como implementar o projeto

1. Instale as dependências:
```bash

pip install -r requirements.txt

2. Execute:
python mein.py

4.Depois de subir:
Você poderá conectar esse GitHub ao Google Colab ou Hugging Face facilmente.

Outros colaboradores também poderão acessar.

cd C:/Users/Denis/PycharmProjects/TCC1

# Inicialize o repositório (se ainda não tiver)
git init

# Adicione os arquivos
git add .

# Faça o commit
git commit -m "Primeiro commit do sistema de detecção de EPIs e sonolência"

# Conecte ao repositório no GitHub (você deve criar um lá antes)
git remote add origin https://github.com/seu-usuario/seu-repositorio.git

# Envie para o GitHub
git push -u origin master

implemente gitignore para reduzir arquivos grandes que exigem alto processamento.

*.mp4
*.avi
*.DS_Store
__pycache__/
*.pyc
dataset_epi_unificado/images/*
dataset_epi_unificado/labels/*

📦 Modelos
O modelo YOLOv8 para detecção de EPIs pode ser treinado localmente ou baixado (ex: modelos/modelo_epi.pt). O treinamento deve ser feito com os datasets adequados para os EPIs reais utilizados no ambiente.

Autor: Denis
Projeto de TCC – Universidade Presbiteriana Mackenzie | CNPq


---

## ✅ ETAPA 4 – Criar e adicionar os arquivos ao repositório

No terminal:

```bash
echo "ultralytics==8.1.26" > requirements.txt
echo "__pycache__/" > .gitignore
echo "dataset_*/" >> .gitignore
echo "*.pt" >> .gitignore

git add .
git commit -m "Versão inicial do projeto com README"
git push -u origin master








