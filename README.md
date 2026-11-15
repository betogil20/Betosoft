**Instituição:** Universidade Katyavala Bwila\
**Curso:** Mestrado em Engenharia Informática

# Projecto de Deep Learning

## Detecção de Textos Produzidos por Inteligência Artificial

**Identificação:** submissao1-grupo3-s1\
**Grupo:** 3

  Integrante
  -------------------
  Alberto Cavimbe
  Edgar Tchissingui
  Joelma Domingos

------------------------------------------------------------------------

## 1. Descrição do projecto

Este projecto tem como finalidade desenvolver e avaliar modelos de Deep
Learning e aprendizagem automática para a classificação de textos,
distinguindo textos produzidos por seres humanos daqueles produzidos por
Inteligência Artificial.

A implementação utiliza Python e NumPy, com foco na compreensão dos
mecanismos de aprendizagem, cálculo dos gradientes, optimização dos
parâmetros e avaliação dos modelos.

## 2. Objectivos

-   Construir um conjunto de dados para classificação de textos Human vs
    AI.
-   Realizar o processamento e a preparação dos dados textuais.
-   Implementar modelos de classificação utilizando NumPy.
-   Treinar e validar os modelos.
-   Comparar o desempenho dos modelos através de métricas.
-   Classificar os textos fornecidos para a submissão.

## 3. Tecnologias utilizadas

  Tecnologia              Aplicação
  ----------------------- -------------------------------
  Python                  Linguagem de programação
  NumPy                   Implementação dos modelos
  Pandas                  Manipulação dos dados
  Matplotlib              Visualização dos resultados
  Google Colab            Ambiente de desenvolvimento
  Hugging Face Datasets   Recolha de dados
  GitHub                  Versionamento e armazenamento

## 4. Estrutura do projecto

``` text
Betosoft/
├── 01_Dados/
│   ├── dados_brutos/
│   │   ├── CSV/
│   │   └── EXCEL/
│   ├── dados_externos/
│   ├── dados_limpos/
│   ├── dados_originais/
│   │   └── dataset3_inputs.csv
│   └── dados_processados/
│       ├── dataset3_inputs_classificado.csv
│       ├── dataset3_inputs_limpo.csv
│       ├── dataset3_inputs_numpy.npz
│       ├── dataset_unificado.csv
│       ├── treino.csv
│       ├── validacao.csv
│       └── teste.csv
├── 03_Modelos/
│   ├── modelo_logistico_grupo3.npz
│   └── vocabulario_grupo3.json
├── 04_Resultados/
│   ├── classificacao_dataset3_grupo3.csv
│   ├── classificacao_final_regressao_logistica.csv
│   ├── comparacao_modelos_grupo3.csv
│   ├── metricas_teste_grupo3.csv
│   └── metricas_validacao_grupo3.csv
└── 05_Submissoes/
    └── Submissao1/
        └── submissao_grupo3.csv
```

## 5. Conjunto de dados

O conjunto unificado contém 1.000 registos:

-   450 textos Human provenientes da fonte externa.
-   450 textos AI provenientes da fonte externa.
-   100 textos de entrada fornecidos para a submissão.

Os 100 textos de entrada foram classificados inicialmente por um
detector externo e possuem pseudo-etiquetas. Estas previsões não
constituem confirmação da autoria real dos textos.

Fonte externa: [Hugging Face ---
dmitva/human_ai_generated_text](https://huggingface.co/datasets/dmitva/human_ai_generated_text).

## 6. Preparação dos dados

O processamento inclui:

1.  Carregamento dos ficheiros.
2.  Limpeza dos textos.
3.  Remoção de textos vazios.
4.  Tokenização.
5.  Construção do vocabulário.
6.  Vectorização dos textos.
7.  Divisão em treino, validação e teste.

## 7. Modelos e implementação

Os modelos são implementados com operações NumPy, sem recorrer a
frameworks de Deep Learning para a implementação dos algoritmos de
treino.

O projecto contempla:

-   Regressão Logística.
-   Redes Neuronais Profundas (DNN).
-   Redes Neuronais com Dropout.

A Regressão Logística utiliza a função Sigmoid, Binary Cross Entropy e
regularização L2.

## 8. Avaliação dos modelos

A avaliação considera as seguintes métricas:

-   Accuracy.
-   Precision.
-   Recall.
-   F1-score.
-   Matriz de confusão.
-   Loss de treino e validação.

Os resultados experimentais encontram-se na pasta `04_Resultados`.

## 9. Submissão

O ficheiro de submissão encontra-se em:

`05_Submissoes/Submissao1/submissao_grupo3.csv`

O ficheiro contém os identificadores dos textos e as respectivas
classificações.

## 10. Identificação da versão

**Versão:** submissao1-grupo3-s1\
**Estado:** Primeira submissão\
**Grupo:** 3

## 11. Repositório

[GitHub --- Betosoft](https://github.com/betogil20/Betosoft)

------------------------------------------------------------------------

**Projecto de Deep Learning --- Mestrado em Engenharia Informática**\
**Universidade Katyavala Bwila --- Grupo 3**
