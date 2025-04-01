# ICML 2025 Submission 12437 Rebuttal Materials

||  MultiArith    | GSM8K    |  AddSub    |  AQuA  |  SingleEQ  |  SVAMP  |  MAWPS  |  Avg.  |
|-|-------------|-------------|-------------|-|-|-|-|-|
|**LIFT**| 98.66±0.71 | **49.03**±0.39 | 92.22±1.17  |**24.61**±1.29 | 95.62±0.29 |  63.15±1.00  |  **89.60**±0.46  |  **73.27**±0.45  |
|Full FT| 98.29±0.34 | 46.13±0.46 | **93.67**±0.47 | 22.34±1.66 |  96.01±0.56  |  61.93±1.21  |  89.50±0.89  |  72.55±0.50  |
|S2FT| **98.88**±0.52 | 45.05±0.94 | 92.78±0.73 | 23.62±0.28 |  **96.56**±0.95  |  59.2±0.60  |  89.39±0.46  | 72.21±0.45 |
|PiSSA| 98.17±0.41 | 43.78±0.54 | 93.04±0.66 | 24.11±1.23 |  96.06±0.24  |  59.25±0.86  |  89.60±0.75  | 72.00±0.14|
|DoRA| 97.54±0.79 | 46.97±0.76 | 91.46±0.37 | 22.93±1.32 |  93.16±0.56 |  62.65±0.72 |  88.13±1.24  |71.83±0.39 |
|LoRA| 97.17±0.47  | 47.02±1.19 | 91.01±0.46 | 24.31±2.00 |  93.21±0.53  |  **63.48**±0.61  |  87.61±0.70 |  71.97±0.18 |

*Table 8: Comparing different methods on LLaMA-2-7B fine-tuned on the MATH-10K dataset with four random seeds.*

## Memory Figures

| ![7B model](https://anonymous.4open.science/r/ICML2025_12437-B2FF/figures/memory/7b_1024.png) | ![8B model](https://anonymous.4open.science/r/ICML2025_12437-B2FF/figures/memory/8b_1024.png) |
|-------------------------------------------|-------------------------------------------|

![Memory Legend](https://anonymous.4open.science/r/ICML2025_12437-B2FF/figures/memory/memory_legend.png)

*Figure 17: Breakdown of memory consumption of Full Fine-tuning, LoRA, LIFT and LIFT_MLP on LLaMA-2-7B and LLaMA-3-8B.*

---

## Training Loss Curve

<p align="center">
  <img src="https://anonymous.4open.science/r/ICML2025_12437-B2FF/figures/loss_all.png" alt="Loss Curve" width="300">
</p>

*Figure 18: Training loss curves of different methods with LLaMA-2-7B model on MATH-10K dataset.*

---

## Effective Rank Figures

<!-- Three images in a row -->
| ![Q](https://anonymous.4open.science/r/ICML2025_12437-B2FF/figures/effective_rank/7B_q_proj_no_y.png) | ![K](https://anonymous.4open.science/r/ICML2025_12437-B2FF/figures/effective_rank/7B_k_proj_no_y.png) | ![V](https://anonymous.4open.science/r/ICML2025_12437-B2FF/figures/effective_rank/7B_v_proj_no_y.png) |
|----------------------------------------------------|----------------------------------------------------|----------------------------------------------------|

<!-- Next row (Up, Down) -->
| ![Up](https://anonymous.4open.science/r/ICML2025_12437-B2FF/figures/effective_rank/7B_up_proj_no_y.png) | ![Down](https://anonymous.4open.science/r/ICML2025_12437-B2FF/figures/effective_rank/7B_down_proj_no_y.png) |
|------------------------------------------------------|---------------------------------------------------------|

![Effective Rank Legend](https://anonymous.4open.science/r/ICML2025_12437-B2FF/figures/effective_rank/effective_rank_legend.png)

*Figure 19: Effective rank of the update matrix of different methods on LLaMA-2-7B.*