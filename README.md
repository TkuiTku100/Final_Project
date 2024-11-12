# Enhancing Retrieval-Augmented Generation with Generative Adversarial Networks for Improved Question Answering

## Introduction

This project aims to improve traditional Retrieval-Augmented Generation (RAG) pipelines by integrating a Generative Adversarial Network (GAN) approach. By treating document retrieval and answer generation as interdependent tasks within a unified model, we aim to enhance the quality of both components.

## Project Structure

├── Presentation_Video.mp4

├── Model_Training.ipynb

├── Evaluation.ipynb

├── hotpot_train_v1.1.json

├── deberta_v3_base_model1

└── bert_model1

## Getting Started

### 1. Clone the Repository

1. Open your terminal or command prompt.
2. Run the following command:
   
   ```bash
   git clone https://[your_repository_url].git
   ```

### 2. Set Up the Environment

**Install Required Packages:**

1. Ensure you have Python and `pip` installed on your system.
2. The first cell in each notebook contains the needed libraries, run the command if needed

**Configure Pinecone API Key:**

1. Create a Pinecone account and obtain your API key.
2. Open the `Evaluation.ipynb` notebook in a Jupyter notebook environment.
3. Locate the variable `PINECONE_API_KEY` and replace it with your actual API key.

### 3. Train the Model

1. **Update Dataset Path:**
   Open the `Model_Training.ipynb` notebook.
   Locate the line where the path to the `hotpot_train_v1.1.json` dataset is defined. Modify this path to match the location of the dataset on your system.

2. **Run the Notebook:**
   Execute all the cells in the `Model_Training.ipynb` notebook. This will train the model and create the `deberta_v3_base_model1` and `bert_model1` directories.

### 4. Evaluate the Model

1. **Update Model and Pinecone Paths:**
   Open the `Evaluation.ipynb` notebook.
   Locate the sections where the paths to the trained model directories and your Pinecone API key are defined. Update these paths accordingly.

2. **Run the Notebook:**
   Execute all the cells in the `Evaluation.ipynb` notebook. This will evaluate the model's performance.

## Presentation

For a visual overview of the project, watch the `Presentation_Video.mp4` file.

## Additional Notes

- The `hotpot_train_v1.1.json` dataset is required for model training. Ensure you have it downloaded before proceeding.
- If you encounter any issues or have questions, feel free to reach out to [alonaricha@campus.technion.ac.il].
