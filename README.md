# Sistema de Busca por Similaridade Visual de Logos (LogoDet-3K)

Pesquisa e construção de um pipeline de busca por similaridade visual de marcas analisando Foundation Models, dados desbalanceados e Inteligência Artificial Explicável (XAI).

Este repositório contém uma série de 5 cadernos (*Jupyter Notebooks*) que ilustram o desenvolvimento passo-a-passo de um pipeline de *retrieval* visual, construído como parte de um estudo aprofundado em modelos de Visão Computacional.

## Estrutura do Estudo
1. `01_logo_similarity.ipynb`: Análise exploratória de dados e construção da *baseline* (CLIP + ResNet-50 com Triplet Loss) usando indexação FAISS.
2. `02_foundation_models.ipynb`: Um *benchmark* investigando as melhores representações zero-shot (comparando modelos como CLIP, DINOv2, SigLIP e EVA02).
3. `03_imbalanced_learning.ipynb`: Estudo focando em estratégias para lidar com o grave desbalanceamento natural da base de dados (*Focal Loss*, amostragens customizadas).
4. `04_xai_benchmark.ipynb`: Avaliação da Interpretabilidade e da Confiança (*Faithfulness*) em modelos convolucionais e transformadores gerando *heatmaps* (Grad-CAM, LIME).
5. `05_pipeline_e2e.ipynb`: O fluxo integrado para produção de *end-to-end* (Detecção com Grounding DINO $\rightarrow$ Embedding $\rightarrow$ FAISS $\rightarrow$ Extração de Texto OCR).
