# FR/NFR Classification and FR→NFR Trace Link Discovery

Code and data for the paper:

> Khaleduzzaman, Z. Che Embi, and N. K. Why, "Artificial Intelligence for Requirements Engineering: Unified FR/NFR Classification and Trace Link Discovery," *JOIV: International Journal on Informatics Visualization* (under review).

## Contents
| File | Description |
|---|---|
| `FR_NFR_Pipeline_v2_Colab.ipynb` | Full experiment notebook (produces every table and figure in the paper) |
| `Labeled_Requirements_Dataset.csv` | D1: e-commerce requirements corpus (3,357 statements) |
| `results_v2_bundle.zip` | Results of the run reported in the paper (tables as CSV, figures as PNG, `results_v2.json`) |

## Dataset D1
Columns: `Type` (FR/NFR), `Subcategory` (NFR subtype), `Requirement Text`, `Source/Module`.
The corpus was produced with Gemini 2.5 Pro and reviewed by three software engineers, who checked classification accuracy, corrected incorrect labels, and removed irrelevant or ambiguous statements.

Public datasets D2 (PROMISE_exp) and D3 (PROMISE NFR FR→NFR traces) are downloaded automatically by the notebook from
https://github.com/AleksandarMitrevski/se-requirements-classification (commit 1f5dc45).

## How to reproduce
1. Open the notebook in Google Colab.
2. Runtime → Change runtime type → **T4 GPU**.
3. Runtime → **Run all**, and upload `Labeled_Requirements_Dataset.csv` when prompted.
4. Results are saved to `results_v2_bundle.zip` (about 45–90 min).

## License
Code: MIT. Please cite the paper if you use the code or data.
