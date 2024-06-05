<h1 align="center">Modelos para Monitoramento de Sonolência</h1>

<div align="center">

  [Projeto](#projeto) 
  &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  [Tecnologias](#tecnologias)
  &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  [Licença](#license)

</div>

<p align="center">
  <img alt="License" src="https://img.shields.io/static/v1?label=license&message=MIT&color=49AA26&labelColor=000000">
</p>


## 💻 Projeto <a name = "projeto"></a>

Este projeto foi desenvolvido para a Feira da disciplina de Redes Neurais do curso de Engenharia de Software. O objetivo é criar um sistema de detecção de sonolência utilizando redes neurais, visando aumentar a segurança em atividades críticas como a condução de veículos e operações de máquinas pesadas.

### Objetivos

- Detecção de Sonolência em Rostos: Analisar imagens faciais para identificar sinais de sonolência.
- Identificação de Olhos Fechados: Detectar olhos fechados como um indicativo de sonolência.

### Metodologia

- Coleta de Dados: Imagens de rostos e olhos de datasets do [Kaggle](kaggle.com/).
- Treinamento: Uso de TensorFlow e Keras, com técnicas de aumento de dados com ImageGenerator.
- Validação: Conjuntos de dados separados para avaliar a precisão.

### Arquitetura dos Modelos

As arquiteturas podem ser vistas e analisadas camada por camada utilizando a ferramenta [Netron](https://netron.app), basta fazer o upload do modelo dentro da ferramenta e ela gera toda a arquitetura com possibilidade de analisar cada camada apenas clicando nela.

Utilize esses dois modelos para visualização:
- [Drowsiness](./src/models/drowsy/drowsiness_model.h5)
- [Eyes](./src/models/eyes/eyes_model_acc_99.8.h5)

#### Modelo de Detecção de Sonolência:

- Entrada: Imagens de rostos.
  - Rede Neural: Convolucional (CNN).
- Saída: Probabilidade de sonolência ("Sonolento" ou "Não Sonolento").

#### Modelo de Identificação de Olhos Fechados:

- Entrada: Imagens da região dos olhos, separadamente.
  - Rede Neural: Convolucional (CNN).
- Saída: Classificação binária ("Olhos Fechados" ou "Olhos Abertos").

### Resultados

Precisão:
- Detecção de Sonolência: 99.86%.
- Identificação de Olhos Fechados: 99.8%.

<br>
<br>

## 🚀 Tecnologias <a name = "tecnologias"></a>

- Python: Linguagem de programação versátil usada para ciência de dados e aprendizado de máquina.
- TensorFlow: Biblioteca para construção e treinamento de modelos de aprendizado profundo.
- Keras: Interface de alto nível para redes neurais, integrada ao TensorFlow.
- Split-folders: Facilita a divisão de conjuntos de dados em treino, validação e teste.
- Scikit-Learn: Ferramentas para mineração de dados e análise de dados.
- Matplotlib: Biblioteca para criação de visualizações estáticas e interativas.
- Seaborn: Interface de alto nível para gráficos estatísticos baseados no Matplotlib.
- Pandas: Estruturas de dados flexíveis para manipulação e análise de dados tabulares.
- Numpy: Suporte para arrays e operações matemáticas de alto desempenho.
- Pillow (PIL): Processamento e manipulação de imagens em vários formatos.
- Glob: Pesquisa de arquivos utilizando padrões de correspondência.
- tqdm: Criação de barras de progresso para loops e processos demorados.

<br>
<br>


##  🔒 Licença

Esse projeto está sob a licença MIT.

<hr>
