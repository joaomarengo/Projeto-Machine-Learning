![Logo das Instituições](images/logos_instituicoes_colorido.png)

<h1 style="text-align:center; font-weight:bold;">
  Abordagem Baseada em Aprendizado de Máquina para o Diagnóstico de Doenças Eritemato-Escamosas
</h1>

---

## Descrição do Projeto

Este projeto foi desenvolvido como trabalho final da disciplina **Aprendizado de Máquina**, do **Bacharelado em Ciência e Tecnologia da Ilum Escola de Ciência** (2025.2).

O objetivo é aplicar técnicas de classificação supervisionada para apoiar o diagnóstico diferencial de doenças eritemato-escamosas, grupo de enfermidades dermatológicas com características clínicas e histopatológicas muito semelhantes.

Seis modelos de aprendizado supervisionado foram implementados e comparados, abrangendo tanto algoritmos clássicos quanto métodos baseados em vizinhança e votação de intervalos:

* **Baseline**
* **K-Nearest Neighbors (KNN)**
* **Voting Feature Intervals (VFI)**
* **Support Vector Machine (SVM)**
* **Decision Tree**
* **Random Forest**

O projeto demonstra como algoritmos de aprendizado de máquina podem auxiliar na prática médica , ampliando a precisão diagnóstica e reduzindo a necessidade de exames invasivos.

## Dataset

O conjunto de dados utilizado é o **Dermatology Dataset** (*ILTER; GÜVENIR, 1998*), disponível no [UCI Machine Learning Repository](https://doi.org/10.24432/C5FK5P).

Ele contém 366 amostras e 34 atributos (12 clínicos e 22 histopatológicos), distribuídos em 6 classes correspondentes a diferentes doenças dermatológicas:

| Código | Doença                |
| :-----: | :--------------------- |
|    1    | Psoríase              |
|    2    | Dermatite Seborreica   |
|    3    | Líquen Plano          |
|    4    | Pitiríase Rósea      |
|    5    | Dermatite Crônica     |
|    6    | Pitiríase Rubra Pilar |

## Metodologia

1. **Coleta e Leitura dos Dados** — importação direta do repositório UCI via `ucimlrepo`.
2. **Pré-processamento** — tratamento de valores ausentes utilizando `KNNImputer`.
3. **Divisão dos Conjuntos** — partição em 90% treino e 10% teste, com semente fixa para reprodutibilidade.
4. **Normalização e Redução de Dimensionalidade** — aplicação de `StandardScaler` e `PCA` quando necessário.
5. **Otimização de Hiperparâmetros** — uso da biblioteca `optuna` com validação cruzada estratificada.
6. **Avaliação de Desempenho** — aplicação de matriz de confusão e relatório de classificação para cada modelo.
7. **Interpretação dos Resultados** — análise da importância das variáveis via *Permutation Importance*.

## Requisitos e Execução

O projeto foi desenvolvido em **Python 3.10** e requer as seguintes bibliotecas principais:

```bash
scikit-learn
optuna
pandas
numpy
matplotlib
seaborn
ucimlrepo
```

Para instalar as dependências:

```bash
pip install -r requirements.txt
```

Para executar o notebook, acesse a pasta `notebook/` deste repositório e baixe o arquivo `projeto_final.ipynb`.

## Contribuidores

* [**João Gabriel Lima Marengo**](https://github.com/joaomarengo)
* [**Lázaro Santana Ribeiro**](https://github.com/lazaroribeiro)
* [**Victor Emanuel Ruas Lima**](https://github.com/victormanuli)

## Professor Responsável

**Daniel Roberto Cassar**

Doutorado e Pós-Doutorado em Ciência e Engenharia de Materiais (UFSCar). Área de atuação: Informática de materiais.

## Referências

* CASSAR, D. R.  *Dados sintéticos e pipeline* . Jupyter Notebook, Ilum Escola de Ciência, 2025.
* CASSAR, D. R.  *Otimização de hiperparâmetros com Optuna* . Jupyter Notebook, Ilum Escola de Ciência, 2025.
* CASSAR, D. R.  *Redução de dimensionalidade com PCA* . Jupyter Notebook, Ilum Escola de Ciência, 2025.
* CASSAR, D. R.  *Validação cruzada e otimização de hiperparâmetros* . Jupyter Notebook, Ilum Escola de Ciência, 2025.
* GÜVENIR, H. A. et al.  *Learning differential diagnosis of erythemato-squamous diseases using voting feature intervals* .  **Artificial Intelligence in Medicine** , v.13, n.3, p.147–165, 1998.
* ILTER, N.; GÜVENIR, H.  *Dermatology [dataset]* . UCI Machine Learning Repository, 1998. [https://doi.org/10.24432/C5FK5P](https://doi.org/10.24432/C5FK5P).
