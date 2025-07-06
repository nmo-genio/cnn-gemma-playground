# CNN-Gemma Playground

A project combining CNN model training with Gemma 3n for image classification tasks.

## Project Structure

```
├── model/                   # Your CNN model files (from Codex)
├── inference/               # Scripts to run image classification
├── notebooks/
│   ├── gemma-test-kaggle-notebook-working.ipynb  # Verified Kaggle notebook
│   ├── gemma-test-kaggle-notebook.ipynb  # Original Kaggle sample
│   └── gemma3-image-norm_bugGemma.ipynb  # Normalization bug demo
├── gemma-working-test-kaggle-notebook-patched.ipynb  # Patched Kaggle notebook
├── data/
│   └── sample_images/       # For testing in both CNN and Gemma
├── README.md
└── requirements.txt
```

## Setup

1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

2. Add your sample images to `data/sample_images/`

3. Launch the Gemma 3n notebooks on Kaggle:
   - Upload `gemma-working-test-kaggle-notebook-patched.ipynb` or any notebook from `notebooks/`
   - Configure the notebook for Kaggle's environment

## Usage

### Local CNN Training
- Create your own training notebook or script under `notebooks/`
- Trained models will be saved in the `model/` directory

### Gemma 3n on Kaggle
- Use `gemma-working-test-kaggle-notebook-patched.ipynb` or `notebooks/gemma-test-kaggle-notebook-working.ipynb` for testing with Gemma 3n
- These notebooks are optimized for Kaggle's environment

### Inference
- Add inference scripts to the `inference/` directory
- These scripts can load trained models and perform image classification

## Known Issues

- **Gemma 3n Model Issue**: There is a known issue with the Gemma 3n model's handling of image inputs. For more details, please refer to the [Hugging Face discussion](https://huggingface.co/google/gemma-3n-E4B-it/discussions/8#68665baa7548e5ed1ed63af3).

## Contributing

1. Add your CNN model files to the `model/` directory
2. Place inference scripts in the `inference/` directory
3. Use `data/sample_images/` for test images that work with both CNN and Gemma approaches
