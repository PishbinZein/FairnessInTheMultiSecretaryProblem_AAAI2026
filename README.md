# Fairness in the Multi-Secretary Problem

**Official Repository** for the paper **"Fairness in the Multi-Secretary Problem"**, accepted to the **40th AAAI Conference on Artificial Intelligence (AAAI), 2026**.

This repository contains the full paper (`main.pdf`) and the source code used to generate the experimental results presented in the study.

## 📄 About the Paper

This work bridges the gap between **online decision-making** (specifically the multi-secretary problem) and **social choice theory** (fair multi-winner elections). While traditional secretary problems focus on utility maximization, real-world scenarios—such as hiring boards or committee selection—often require fairness among decision-makers with conflicting preferences.

We introduce a framework for **Online Multi-Winner Elections with Cardinal Ballots** and propose mechanisms that merge techniques from online algorithms with established social choice rules.

## 💻 Implementation & Experiments

The code is provided as a single Jupyter Notebook located in `code/`. It implements the proposed algorithms and reproduces the experiments found in Section 5 of the paper.

### Algorithms Implemented

The notebook contains Python implementations of:

1.  **Greedy Budgeting Rule**
2.  **Method of Equal Shares (Offline & Online)**
3.  **Bounded Overspending (Offline & Online BOS)**
4.  **Online Nash Rule**

### Datasets and Experiments

The notebook runs four key experiments:

1.  **Pabulib Instances:** Evaluates fairness (EJR+ violations) on real-world participatory budgeting data.
2.  **Sushi & MovieLens:** Compares algorithms using standard preference benchmarks (Sushi dataset and MovieLens 100k).
3.  **Synthetic Distributions:** Extensive simulations using Impartial Culture (IC), Mallows Model, and Normalized Mallows Model to measure Exclusion Ratio, Gini Coefficient, and Satisfaction. 
4.  **Polarized Instances:** Tests the algorithms on specifically designed polarized datasets to measure underperformance against proportional guarantees.

## ⚙️ Requirements

To run the notebook, you will need Python and the following libraries:

```bash
pip install numpy pandas matplotlib seaborn scipy colorama prefsampling
```

*Note: The code utilizes `prefsampling` for generating synthetic preference data (Mallows models).*

## 🚀 Usage

1.  Clone the repository:
    ```bash
    git clone https://github.com/PishbinZein/fair-multi-secretary.git
    cd fair-multi-secretary
    ```
2.  Navigate to the code directory:
    ```bash
    cd code
    ```
3.  Open the notebook:
    ```bash
    jupyter notebook online_committee_elections_EXPERIMENTS.ipynb
    ```
4.  Run the cells sequentially. The notebook is organized by experiment (Experiments 1 through 4).

## 🎓 Citation

If you use this code or paper in your research, please cite our work:

```bibtex
@inproceedings{papasotiropoulos2026fairness,
  title={Fairness in the Multi-Secretary Problem},
  author={Papasotiropoulos, Georgios and Pishbin, Zein},
  booktitle={Proceedings of the 40th AAAI Conference on Artificial Intelligence (AAAI)},
  year={2026}
}
```

## 📧 Contact

For any questions regarding the code or the paper, please refer to the authors' contact information provided in the paper or open an issue in this repository.