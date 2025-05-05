# README

## Project Title

**Comparing LIME vs SHAP: Model Interpretability Analysis on the Adult Dataset**

## Author

Puyuan Tian (pt2654)

## Project Overview

This project analyzes the interpretability of two popular explanation methods, **LIME** (Local Interpretable Model-agnostic Explanations) and **SHAP** (SHapley Additive exPlanations), in the context of both traditional and neural network models trained on the UCI Adult Census Income dataset.

We benchmark these methods in terms of:

-   Accuracy and ROC-AUC performance of models
-   Explanation stability and consistency
-   Computation time and scalability
-   Visualization of both global and local feature importance

## Key Files

| File | Description |
|----|----|
| `index.qmd` | Project introduction and motivation |
| `data.qmd` | Data description, preprocessing steps |
| `methods.qmd` | Model training and interpretability methodology |
| `results.qmd` | Evaluation results including metrics, visualizations, and insights |
| `visualization.qmd` | Additional plots: UMAP, correlation, parallel coordinates |
| `discussion.qmd` | Reflections, strengths/limits, and takeaways |
| `_quarto.yml` | Project configuration file for Quarto book |

## Repository

GitHub URL: <https://github.com/PuyuanTian37/5293FinalProject>

## Setup Instructions

1.  **Install R and RStudio** (or use VS Code with Quarto plugin).

2.  Clone this repo:

    ``` bash
    git clone https://github.com/PuyuanTian37/5293FinalProject.git
    ```

3.  Install the required R packages:

    ``` r
    install.packages(c("tidyverse", "caret", "randomForest", "neuralnet", "nnet", "lime", "iml", "pROC", "ggplot2", "shapr", "GGally", "uwot"))
    ```

4.  Render the book:

    ``` bash
    quarto render
    ```

## Dataset

-   [UCI Adult Census Income Dataset](https://archive.ics.uci.edu/ml/datasets/adult)
-   Task: Binary classification – predict whether income \>50K

## Highlighted Methods

-   **Random Forest**: interpretable baseline with intrinsic feature importance.
-   **Neural Network (1-layer MLP)**: a moderately complex model to test explanation fidelity.
-   **LIME**: Local perturbation-based explanation.
-   **SHAP**: Game-theoretic model explanation framework.

## License

MIT License.

## Acknowledgments

This project was inspired by discussions from interpretable machine learning coursework and guided by the work of Ribeiro et al. (2016) for LIME and Lundberg & Lee (2017) for SHAP.

------------------------------------------------------------------------

For questions or suggestions, please contact **Puyuan Tian** or open an issue on the GitHub repo.
