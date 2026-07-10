# time-series-forecasting

Minimal from-scratch implementations of ML papers in regression and time-series forecasting.

## Implementations

### `timesfm/` — A Decoder-Only Foundation Model for Time-Series Forecasting
**Paper:** [arXiv:2310.10688](https://arxiv.org/abs/2310.10688) · Das et al., Google (2023)

Pretrains a patched-decoder style attention model on a large time-series corpus. The model achieves zero-shot performance on a variety of public datasets that is competitive with state-of-the-art supervised models trained on each individual dataset. Works across different forecasting history lengths, prediction lengths, and temporal granularities.

---

### `chronos/` — Chronos: Learning the Language of Time Series
**Paper:** [arXiv:2403.07815](https://arxiv.org/abs/2403.07815) · Ansari et al., Amazon (2024)

A framework for pretrained probabilistic time-series models that tokenizes time-series values via scaling and quantization into a fixed vocabulary, then trains existing transformer-based language model architectures (T5 family, 20M–710M parameters) on these tokens using cross-entropy loss. Demonstrates strong zero-shot generalization across 42 datasets spanning both in-distribution and unseen domains.

---

### `regresslm/` — Performance Prediction for Large Systems via Text-to-Text Regression
**Paper:** [arXiv:2506.21718](https://arxiv.org/abs/2506.21718) · Akhauri et al., Google (2025)

Proposes text-to-text regression as a scalable alternative to tabular regression for predicting metric outcomes of large systems (e.g., resource efficiency on Google's Borg cluster). A 60M parameter encoder-decoder model trained from scratch achieves up to 0.99 rank correlation and 100× lower MSE than tabular baselines, while adapting to new tasks with as few as 500 examples.
