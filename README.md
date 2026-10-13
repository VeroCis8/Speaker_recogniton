# Speaker Recognition from Speech

**Dataset:** [Speaker Recognition Audio Dataset (Kaggle)](https://www.kaggle.com/datasets/vjcalling/speaker-recognition-audio-dataset)

**Two protocols are implemented:**
- **Closed-set recognition** — the same speakers appear in training, validation and test. Utterances are split, not speakers. Classic multi-class classification.
- **Open-set recognition (speaker verification)** — speakers are split into disjoint train / validation / test groups. A feature extractor is trained on the training speakers only; unseen (test) speakers are then verified by comparing a query embedding to enrolled speaker templates

**Classifiers explored:** SVM and Random Forest on handcrafted statistical features, a CNN on log-mel spectrograms, and an LSTM on MFCC sequences


> Environment: this notebook is written for **Google Colab**
