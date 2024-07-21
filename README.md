
# CodeCraft: Text-to-Code Generation Model

CodeCraft is a text-to-code generation model built using Huggingface's powerful libraries and the Llama 2 billion parameter model. This project demonstrates the process of fine-tuning 
large language models using Parameter-Efficient Fine-Tuning (PEFT) techniques and evaluates their performance on text-to-code generation tasks.

## Table of Contents

- [Installation](#installation)
- [Model Description](#model-description)
- [Training Process](#training-process)
- [Inference Pipeline](#inference-pipeline)
- [Evaluation](#evaluation)
- [Results](#results)
- [Acknowledgements](#acknowledgements)

## Installation

To get started, clone this repository and install the required dependencies:

```bash
git clone https://github.com/VarunBiyyala/Fine-tuning-Llama_2B.git

```

## Model Description

CodeCraft utilizes the Llama 2 billion parameter model from Huggingface, fine-tuned with PEFT techniques to efficiently reduce trainable parameters and optimize the model for text-to-code generation tasks.

## Training Process

1. **Imported Libraries**: Used Huggingface's Transformers and other necessary libraries.
2. **Loaded Llama Model**: Loaded the Llama 2 billion parameter model.
3. **Defined LoRA Parameters**: Configured Low-Rank Adaptation (LoRA) parameters for PEFT.
4. **Prepared Model for Fine-Tuning**: Reduced trainable parameters to less than 1%.
5. **Fine-Tuned the Model**: Trained the model on the text-to-code dataset.
6. **Saved the Model**: Saved the fine-tuned model to Huggingface.

## Inference Pipeline

An inference pipeline was created to generate code from textual descriptions. This allows for easy testing and validation of the model's performance on new data.

## Evaluation

The performance of CodeCraft was evaluated using the following metrics:

- **ROUGE Score**: To measure the quality of the generated code against reference code.
![Rouge Score Image](https://github.com/VarunBiyyala/Fine-tuning-Llama_2B/blob/main/Llama_Rouge_Score.JPG)
- **Cosine Similarity**: To assess the semantic similarity between generated and reference code snippets.
![Cosine SImilarity Image](https://github.com/VarunBiyyala/Fine-tuning-Llama_2B/blob/main/Llama_Cosine_Similarity.JPG)
## Results

The results on the test data showed promising performance, with high ROUGE scores and strong cosine similarity values, indicating that the model effectively generates accurate and semantically meaningful code from textual descriptions.

## Acknowledgements

Special thanks to Huggingface for providing the tools and models, and to the open-source community for their invaluable contributions.
