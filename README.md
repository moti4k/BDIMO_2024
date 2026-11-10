# Video recommendations with implicit feedback

Team competition solution for the **2023–2024 National Technology Olympiad, Big Data and Machine Learning** track. The original repository records a top-six result for this solution.

## Approach

The notebook prepares user–video interactions, constructs a RecTools dataset, fits a BM25 item-to-item recommender and generates recommendations. It also includes experiments with alternative similarity models and evaluation utilities.

The saved final configuration uses `BM25Recommender(K=5, K1=0.5, B=0.03)` through `ImplicitItemKNNWrapperModel`. Data preparation includes filling missing city values.

## Repository guide

- `main2.ipynb` — data preparation, model experiments and recommendation generation.
- `user_cleaned.csv` — prepared user data.
- `vid_n_own.csv` — video-related data used by the notebook.
- `LICENSE` — repository licence.

## Working with the notebook

Open `main2.ipynb` in Jupyter and review the input paths before running it. The notebook uses Python, NumPy, pandas, tqdm, RecTools and implicit. Reproduction requires the competition inputs referenced in the notebook and compatible library versions.

The original dataset reference is available on [Google Drive](https://drive.google.com/file/d/18MsjwrIF0dls8L4yPXS5I6UABnoC4R_P/view?usp=share_link).

## Context

This repository preserves the team's competition experiments. The interpretation of timestamps and viewing sequences was an important part of the task. The historical notebook remains available for inspecting the actual model and data-processing decisions.
