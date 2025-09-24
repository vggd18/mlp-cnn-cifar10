# Classificação de Imagens CIFAR-10 com Rede MLP e CNN

## Visão Geral do Projeto

Este projeto tem como objetivo treinar e otimizar uma Rede Neural Artificial do tipo Perceptron de Múltiplas Camadas (MLP) para a tarefa de classificação de imagens do dataset CIFAR-10. O CIFAR-10 é um conjunto de dados amplamente utilizado na área de visão computacional, composto por 60.000 imagens coloridas de 32x32 pixels, distribuídas em 10 classes distintas.

As classes a serem classificadas são:
- Airplane (Avião)
- Automobile (Automóvel)
- Bird (Pássaro)
- Cat (Gato)
- Deer (Cervo)
- Dog (Cachorro)
- Frog (Sapo)
- Horse (Cavalo)
- Ship (Navio)
- Truck (Caminhão)

Neste repositório, você encontrará o notebook Jupyter (`CIFAR10_with_MLPs.ipynb`) que detalha todo o processo de experimentação, desde o pré-processamento dos dados até o treinamento e a avaliação da MLP.

## Estrutura do Repositório

- **`CIFAR10_with_MLPs.ipynb`**: Notebook Jupyter contendo todo o código para carregamento dos dados, definição do modelo MLP, treinamento, avaliação e visualização dos resultados.
- **`README.md`**: Este arquivo de documentação.

## Como Executar os Experimentos

Para replicar os experimentos e treinar a rede, siga os passos abaixo:

1.  **Clone o repositório:**
    ```bash
    git clone https://github.com/vggd18/mlp-cnn-cifar10.git
    cd mlp-cifar10-classificador
    ```

2.  **Crie e ative um ambiente virtual (recomendado):**
    ```bash
    python -m venv venv
    # No Linux/macOS
    source venv/bin/activate
    # No Windows
    .\venv\Scripts\activate
    ```

3.  **Inicie o Jupyter Notebook:**
    ```bash
    jupyter notebook CIFAR10_with_MLPs.ipynb
    ```
    Após abrir o notebook, você pode executar as células de código para acompanhar todo o processo de experimentação.

## Experimentos e Variação de Hiperparâmetros

O notebook explora sistematicamente diversas variações de hiperparâmetros da MLP com o objetivo de encontrar a configuração que maximiza o desempenho do modelo. 

## Avaliação de Desempenho

O desempenho do modelo é rigorosamente avaliado utilizando as seguintes métricas:

-   **Acurácia Total:** Percentual geral de imagens classificadas corretamente no conjunto de teste.
-   **Precisão (Precision):** Mede a proporção de predições positivas que foram de fato corretas.
-   **Recall (Revocação):** Mede a proporção de positivos reais que foram corretamente identificados.
-   **Acurácia por Classe:** Análise individual da acurácia para cada uma das 10 classes do CIFAR-10, permitindo identificar quais classes o modelo tem maior ou menor dificuldade em classificar.

Os resultados detalhados, incluindo matrizes de confusão e gráficos de desempenho, são apresentados no notebook.