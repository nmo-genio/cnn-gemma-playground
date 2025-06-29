# CNN-Gemma Playground

A project combining CNN model training with Gemma 3n for image classification tasks.

## Project Structure

```
├── model/                   # Your CNN model files (from Codex)
├── inference/               # Scripts to run image classification
├── notebooks/
│   ├── cnn_training.ipynb   # Runs locally on Mac
│   └── gemma_kaggle_test.ipynb  # Gemma 3n notebook (runs on Kaggle)
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

3. For local CNN training:
   - Open `notebooks/cnn_training.ipynb`
   - Run the notebook locally on your Mac

4. For Gemma 3n testing:
   - Upload `notebooks/gemma_kaggle_test.ipynb` to Kaggle
   - Configure the notebook for Kaggle's environment

## Usage

### Local CNN Training
- Use `notebooks/cnn_training.ipynb` for training CNN models locally
- Trained models will be saved in the `model/` directory

### Gemma 3n on Kaggle
- Use `notebooks/gemma_kaggle_test.ipynb` for testing with Gemma 3n
- This notebook is optimized for Kaggle's environment

### Inference
- Add inference scripts to the `inference/` directory
- These scripts can load trained models and perform image classification

## Contributing

1. Add your CNN model files to the `model/` directory
2. Place inference scripts in the `inference/` directory
3. Use `data/sample_images/` for test images that work with both CNN and Gemma approaches
