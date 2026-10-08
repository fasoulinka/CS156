# 777 Radio — CS156 First Pipeline (draft)

This repository contains an early research pipeline based on my existing image-to-music app, **777 Radio**.

## Research question
Can a model learn to generate my personal aesthetic song tags from measured audio, reducing manual annotation while preserving image-to-song recommendation quality?

## Current evidence
- `music-dataset.csv`: 162 manually tagged songs from my app.
- `777_radio_exploration.ipynb`: executed exploratory notebook with CSV inspection, tag frequencies, and a held-out song split.
- `assignment_draft.pdf`: proposal and experiment design.
- `unit_review_slide.pptx`: one-slide review of train/test split and overfitting.

## Important limitations
The CSV contains **no audio recordings**. The original app's energy, tempo, and valence are randomly generated placeholders, not measured acoustic features. **No sound-based classifier has been trained or evaluated yet.**

## Planned experiment
1. Obtain legally accessible audio.
2. Extract real acoustic features per song.
3. Predict multiple aesthetic tags using baseline, logistic regression, and SVM.
4. Compare held-out predictions with human labels.
5. Optionally replace the paid image-description API with a locally run pretrained image encoder.

## Run notebook
```bash
pip install pandas numpy matplotlib scikit-learn jupyter
jupyter notebook 777_radio_exploration.ipynb
```

## References
- My existing 777 Radio source archive, `vibe-match-app-3.zip` (not bundled here).
- CS156 Generated Forum Code Workbook (course material).
