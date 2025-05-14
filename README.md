# TCC2 – Sistema de Detecção de EPIs, Sonolência e Comportamentos Inseguros

Este projeto utilizando o YOLOv8, YOLOv5 e MediaPipe detecta automaticamente a presença e o uso correto de Equipamentos de Proteção Individual (EPIs), sinais de sonolência, uso de celular e alimentação, emitindo alertas sonoros conforme a situação.

## 🔍 Funcionalidades

- ✅ Detecção de EPIs: capacete, óculos, colete, máscara, touca, bota, etc.
- 😴 Detecção de sonolência com MediaPipe (malha facial)
- 📱 Detecção de uso de celular e alimentação
- 🔊 Alertas sonoros diferentes para cada situação
- 🟢 Diagnóstico com texto e cor na tela (verde: normal, vermelho: alerta)
- 💻 Suporte para execução em Raspberry Pi 4

## 🚀 Como usar

1. Instale as dependências:
```bash
pip install -r requirements.txt

## Funcionalidades
- Detecção de sonolência via malha facial
- Detecção de EPIs com YOLOv8
- Alertas sonoros por categoria (sonolência, ausência de EPIs, etc.)

## Como rodar
1. Instale as dependências:
   pip install -r requirements.txt
   
2. Execute:
   python mein.py

3. Crie uma estrutura parecida com esta:

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


📦 Modelos
O modelo YOLOv8 para detecção de EPIs pode ser treinado localmente ou baixado (ex: modelos/modelo_epi.pt). O treinamento deve ser feito com os datasets adequados para os EPIs reais utilizados no ambiente.

Autor: Denis
Projeto de TCC – Universidade Presbiteriana Mackenzie | CNPq


## ✅ ETAPA 4 – Criar e adicionar os arquivos ao repositório

No terminal:

```bash
echo "ultralytics==8.1.26" > requirements.txt
echo "_pycache_/" > .gitignore
echo "dataset_*/" >> .gitignore
echo "*.pt" >> .gitignore

git add .
git commit -m "Versão inicial do projeto com README"
git push -u origin master

5. Crie um arquivo .gitignore
   isso evita subir arquivos muito grandes ou desnecessásrios:
   
 *.mp4
 *.avi
*.DS_Store
_pycache_/
*.pyc
dataset_epi_unificado/images/*
dataset_epi_unificado/labels/*


   
