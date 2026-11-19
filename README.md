
# DeepSense-X

### An Explainable and Uncertainty-Aware Hybrid LSTM–Transformer Framework for Industrial Anomaly Detection and Predictive Maintenance

DeepSense-X explores deep-learning-based anomaly detection for industrial air compressor systems using the MetroPT-3 dataset.

## Models
1. LSTM Autoencoder
2. Transformer Autoencoder
3. Hybrid LSTM–Transformer Autoencoder

## Project Phases

| Phase | Description |
|---|---|
| Phase 1 | Data preprocessing and window generation |
| Phase 2 | LSTM Autoencoder |
| Phase 3 | Transformer Autoencoder |
| Phase 4 | Hybrid LSTM–Transformer |
| Phase 5 | Uncertainty, explainability and robustness |
| Phase 6 | Final experimental evaluation |

## Dataset

MetroPT-3 dataset:
https://archive.ics.uci.edu/dataset/791/metropt+3+dataset

The original dataset is not included in this repository.

## Final Experimental Results

| Model | Precision | Recall | F1-score | Accuracy |
|---|---:|---:|---:|---:|
| LSTM Autoencoder | 54.17% | 99.42% | 70.13% | 95.63% |
| Transformer Autoencoder | 52.67% | 99.42% | 68.86% | 95.36% |
| Hybrid LSTM–Transformer | 53.83% | 99.42% | 69.84% | 95.57% |

Results are based on a sampled 10,000-window test set. Event-period detection does not establish advance failure prediction.

## Explainability and Uncertainty

Phase 5 includes:
- Monte Carlo uncertainty estimation
- Sensor perturbation importance
- Local sensor explanations
- Missing sensor experiments
- Noise and sensor drift experiments

Perturbation importance measures model sensitivity, not causality.

## Technology Stack

- Python
- TensorFlow / Keras
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Google Colab

## Repository Structure

- `notebooks/` – Six project notebooks
- `artifacts/` – Model metadata and preprocessing artifacts
- `phase5/` – Explainability and robustness results
- `phase6/` – Final evaluation results

Large datasets, model checkpoints and generated arrays are excluded from the initial GitHub upload.

## How to Run

1. Clone this repository.
2. Download the MetroPT-3 dataset from UCI.
3. Open the notebooks in Google Colab.
4. Mount Google Drive and configure the dataset path.
5. Run notebooks sequentially from Phase 1 to Phase 6.

## Author

**Udit Pattnayak**

Deep Learning | Anomaly Detection | Predictive Maintenance
