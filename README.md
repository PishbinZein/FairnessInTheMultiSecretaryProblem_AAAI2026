# Fairness in the Multi-Secretary Problem

Repository for the paper **"Fairness in the Multi-Secretary Problem"**, coauthored by G. Papasotiropoulos and Z. Pishbin, accepted at the **40th AAAI Conference on Artificial Intelligence (AAAI), 2026**. 

This paper bridges two perspectives: it studies the multi-secretary problem through the fairness lens of social choice, and examines multi-winner elections from the viewpoint of online decision making. After identifying the limitations of the prominent proportionality notion of Extended Justified Representation (EJR) in the online domain, the work proposes a set of mechanisms that merge techniques from online algorithms with rules from social choice---such as the Method of Equal Shares and the Nash Rule---and supports them through both theoretical analysis and extensive experimental evaluation.

This repository contains Python implementations of the methods proposed in the paper: (i) the Greedy Budgeting Rule, (ii) the online Method of Equal Shares and the online Method of Equal Shares with Bounded Overspending and (iii) the Online Nash Rule. It also includes the source code used to generate the empirical evaluation results presented in the paper (Section 5). All code is provided in a single Jupyter Notebook.
