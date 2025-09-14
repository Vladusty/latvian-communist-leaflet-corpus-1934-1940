# Lemma Frequency Notebooks

This folder contains Google Colab–ready notebooks for monthly lemma frequency analysis on the *Latvian Communist Leaflet Corpus (1934–1940)*.

**What’s inside**
- `corpus_monthly_absolute_freq_lemma_unweighted_and_weighted_by_print_run.ipynb`  
  Absolute counts per month (unweighted) and print-run–weighted counts.
- `corpus_monthly_relative_freq_lemma_unweighted_and_weighted_by_print_run_per1000.ipynb`  
  Relative counts per 1,000 tokens per month (unweighted and print-run–weighted).

**Method highlights**
- Lemmatization: Latvian **Stanza** (`tokenize, lemma`), no stopword removal.
- Manual mapping list lets you force inflected/adjectival forms to the target lemma.
- Date handling: exact dates, `[start..end]` midpoint, `[start…]`/`[…end]` boundary; `[.]` skipped.
- Print runs: `print_run` used as weight; unknowns use `DEFAULT_WEIGHT_FOR_UNK` (median or fixed override).

## How to use

Choose a notebook and open it directly in Colab:

- **Absolute frequency**  
  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1_xOokqW93imBj8XtGNa4HgZTZSzYiFX4?usp=sharing)  
  *(monthly absolute counts — raw and print_run–weighted)*

- **Relative frequency**  
  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/10SX4d788XJjovJ4fvBBmUAHe6vvzUxhz?usp=sharing)  
  *(monthly relative frequency per 1,000 tokens — unweighted and print_run–weighted)*

Then inside the notebook:  
1. Upload a ZIP of `.txt` leaflets (corpus format).  
2. Set `target_lemma` and optional `manual_forms`.  
3. Run all cells; export figures/tables if needed.

License: CC BY 4.0 (see repo root).
