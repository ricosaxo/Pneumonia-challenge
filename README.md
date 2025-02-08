# Pneumonia Detection in Chest X-rays: A CNN Approach

## Description

This project implements a Convolutional Neural Network (CNN) to classify chest X-ray images for pneumonia detection. It utilizes the "paultimothymooney/chest-xray-pneumonia" dataset from Kaggle Hub. The CNN is trained and evaluated to recognize new images outside of the training set. The project includes data preprocessing, image augmentation, CNN design, training, evaluation, and visualization of results.

## Installation

1.  **Clone the repository:**

    ```bash
    git clone <repository_url>
    cd pneumonia-challenge
    ```

2.  **Create a virtual environment (recommended):**

    ```bash
    python -m venv .venv
    source .venv/bin/activate  # On Linux/macOS
    .venv\Scripts\activate   # On Windows
    ```

3.  **Install the dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

## Usage

1.  **Download the dataset:**

    - The notebook automatically downloads the dataset from Kaggle Hub.
    - Ensure you have a `kagglehub` configured with your Kaggle API key (create `~/.kaggle/kaggle.json` file). [See Kaggle API documentation](https://github.com/Kaggle/kaggle-api) for details.

2.  **Run the Jupyter Notebook:**

    ```bash
    jupyter notebook pneum.ipynb
    ```

3.  **Follow the notebook instructions:**

    - The notebook guides you through data loading, preprocessing, model design, training, and evaluation.
    - Adjust hyperparameters and experiment with different CNN architectures as needed.
    - Interpret and analyze the evaluation metrics, confusion matrix, and ROC curve.

## Contributors

- Rik Sas

## Timeline

2 days

## File Structure:

- `.gitignore`: Specifies intentionally untracked files that Git should ignore.
- `pneum.ipynb`: Jupyter Notebook containing the source code.
- `README.md`: This file.
- `requirements.txt`: Python package dependencies.

## Model improvements

- Try different CNN architectures (e.g., ResNet, DenseNet)
- Use more data
- Explore other data augmentation techniques.

## Notes:

- Due to the lack of GPU the image size has been reduced in the first step and some dataset has been removed to make the code more optimal when running. A GPU is recommended.
- The `val` folder is used as validation.
- Remember to adjust the hyperparameter grid and cross-validation settings based on your available resources and the specific requirements of your pneumonia detection task.
