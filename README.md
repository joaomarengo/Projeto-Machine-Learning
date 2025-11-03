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

Além disso, aplicou-se o método de Permutation Importance para avaliar a relevância global de cada atributo no desempenho dos classificadores, fornecendo uma medida interpretável da contribuição de cada variável clínica e histopatológica para a decisão dos modelos.

Os processos de otimização de hiperparâmetros foram conduzidos com *Optuna* , garantindo reprodutibilidade e busca sistemática pelos parâmetros ideais.

O projeto evidencia como algoritmos de aprendizado de máquina podem auxiliar na prática médica, aumentando a precisão diagnóstica e reduzindo a necessidade de exames invasivos.

## Contribuidores

* **João Gabriel Lima Marengo**
* **Lázaro Santana Ribeiro**
* **Victor Emanuel Ruas Lima**

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
