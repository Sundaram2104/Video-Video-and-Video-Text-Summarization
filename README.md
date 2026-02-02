Multimodal Video Summarization (V2VT)
This repository contains V2VT, a multimodal video summarization pipeline that generates concise video and text summaries using visual, audio, and textual features extracted from raw videos.

The project is designed as a research‑style implementation for TVSum and SumMe datasets, with a focus on both quantitative evaluation and qualitative visualizations.

Key features
Multimodal inputs:

Visual features from frame‑level CNN encoders (e.g., ResNet).

Audio features from mel‑spectrograms and CNN encoders.

Text features from precomputed captions or transcripts (e.g., BERT embeddings).

Temporal modeling with sequence models (e.g., BiLSTM) for importance scoring over time.

Support for chunk-level caption alignment between video segments and text.

End‑to‑end pipeline: feature extraction → summarization → metric evaluation → visualization.

Datasets
TVSum: 50 videos across 10 categories with human importance annotations.

SumMe: 50 user videos with frame‑level importance scores.

Scripts/notebooks are provided to:

Load preprocessed features.

Align annotations.

Generate model‑ready datasets.

(You can add a note here if you are not distributing raw videos and expect users to download them separately.)

Evaluation metrics
The repository includes evaluation code for:

Frame‑level and segment‑level:

Precision, Recall, F1‑Score.

Textual summary quality:

ROUGE‑L.

Multimodal / semantic:

CLIPScore (optional, if you used it).

Additional analysis:

Compression ratio (summary length vs original).

Temporal coherence / smoothness (if implemented).

Generated plots include:

Model performance comparison across datasets.

Ablation studies on model components.

Compression ratio and runtime / FPS charts.
