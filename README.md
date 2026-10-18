# CS156 — First Pipeline: 777 Radio

## Final submission

**[Open my completed First Pipeline notebook](CS156_Pipeline.ipynb)**

This is my final CS156 machine learning pipeline, including the executed code, saved outputs, visualizations, mathematical explanations, model comparisons, error analysis, discussion, references, and ethical considerations.

## Project overview

I built 777 Radio, an image-to-song recommendation app that uses aesthetic tags I manually assign to songs. This project investigates whether machine learning can predict those tags directly from audio, reducing the need to tag every new song by hand.

I started with 162 songs from my personal collection and matched 145 to audio recordings. I extracted 33 handcrafted audio features and 512-dimensional pretrained CLAP embeddings.

I compared logistic regression, decision trees, SVMs, and baseline approaches to predict three broad aesthetic categories. I also tested several approaches for recommending exact personal tags, including nearest neighbors, popularity-based predictions, and CLAP zero-shot matching.

The notebook includes a 115-song training set, a 30-song held-out test set, cross-validation, feature ablation experiments, and an analysis of why certain approaches performed poorly.

## Repository files

- **`CS156_Pipeline.ipynb`** — Final executed notebook. **This is the file to grade.**
- `777_radio_exploration.ipynb` — Preliminary data exploration and experiment planning.
- `music-dataset.csv` — Original personal song-tag dataset.
- `assignment_draft.pdf` — Earlier project proposal, before the experiments were completed.
- `unit_review_slide.pptx` — Previous course material, not part of this submission.

## Reproducibility and data

The notebook contains saved outputs from the completed experiments. Re-running the full audio pipeline requires access to the original audio files and appropriate Google Drive paths.

The copyrighted MP3 recordings are not distributed in this repository. The dataset contains my personal aesthetic labels, so results reflect my own preferences rather than universal descriptions of music.

## Project context

777 Radio app: https://777radio.vercel.app/
