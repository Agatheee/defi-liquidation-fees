# Liquidation Dynamics in DeFi and the Role of Transaction Fees

Code accompanying the paper

> Agathe Sadeghi and Zachary Feinstein, *Liquidation Dynamics in DeFi and the Role of Transaction Fees*, Stevens Institute of Technology.

`reproduce_examples.ipynb` reproduces every numerical example of the paper (Examples 1–5) and regenerates Figures 3, 4, 5, 7, 8 and 9. It implements Algorithm 1 (optimal liquidation at a lending protocol whose oracle is a constant product market maker) and the sandwich-attack objective of Section 4, in closed form.

## Running

```
pip install -r requirements.txt
jupyter notebook reproduce_examples.ipynb
```

Run all cells top to bottom. Each figure is displayed and saved to `image/` under the filename used in the manuscript. The whole notebook runs in under a minute on a laptop.

## Contents

| Cell group | Paper |
|---|---|
| Core functions `algo1`, `realized`, `sandwich` | Algorithm 1, Section 3.2, equation (9) |
| Example 1 | Figure 3 |
| Example 2 | Figure 4 |
| Example 3 | Figure 5 |
| Example 4 | Figure 7 |
| Example 5 | Figures 8 and 9, critical fee γ* |

## Requirements

Python 3.10 or later with numpy, scipy and matplotlib (versions pinned in `requirements.txt`).
