# Building a Neural Machine Translation Demo for English to Japanese

This repository contains the code and results for a Neural Machine Translation (NMT) project that translates text from English to Japanese. This project was completed as part of the Sony Research India NMT/LLM Internship application challenge.

## 1. Introduction

### What is NMT?
Neural Machine Translation (NMT) is a modern approach to automated language translation that uses deep neural networks to map a sequence of text from a source language to a target language. Unlike older statistical methods, NMT models like mBART can learn the nuances, context, and grammar of languages, resulting in more fluid and accurate translations.

### Why does it matter?
In a connected world, high-quality translation technology is essential for breaking down communication barriers in business, entertainment, and daily life. Developing and refining these systems is a key area of AI research, with direct impacts on global products and services.

## 2. Method

This demo was built using freely available, state-of-the-art tools.

*   **Model:** We used the `facebook/mbart-large-50-many-to-many-mmt` (mBART) model from the Hugging Face Hub. mBART is a powerful multilingual sequence-to-sequence model trained on data from 50 different languages, making it highly effective for translation tasks without needing to be trained from scratch.
*   **Tools:** The project was developed in a **Google Colab** notebook, leveraging its free GPU for efficient model inference. The core logic is powered by the **Hugging Face `transformers` library**, which simplifies the process of downloading and using pre-trained models.
*   **Dataset:** The model was tested on a small, custom set of English sentences, including conversational phrases and a technical, business-oriented sentence relevant to Sony's work.

## 3. Results

The model demonstrated high-quality translation from English to Japanese. The code for this demo can be found in the `NMT_Demo_EN_JA.ipynb` notebook in this repository.

Here is a screenshot of the code and its output:

*(We will add the screenshot here in the next step)*

## 4. Challenges & What I Learned

*(This is the most important section for you to personalize!)*

During this project, I initially encountered a `RepositoryNotFoundError` when trying to access the `Helsinki-NLP` model. Instead of getting stuck, I troubleshooted the issue by successfully implementing an alternative high-performing model, mBART, which was also recommended in the task description. This experience taught me the importance of:
*   **Adaptability:** Quickly pivoting to an alternative solution when the primary plan fails.
*   **Model Selection:** Understanding that different pre-trained models have different strengths and that choosing the right one is critical for project success.
*   **Practical Implementation:** I gained hands-on experience with the end-to-end workflow of a real NMT task, from environment setup and model loading to tokenization and decoding.

## 5. Next Steps

While this demo is effective, the system could be improved in several ways:

*(Personalize these ideas or add your own)*

*   **Fine-Tuning:** The model could be fine-tuned on a specific domain (e.g., technical manuals or movie subtitles) to improve its accuracy and adopt the correct terminology for that domain.
*   **UI Deployment:** To make the model more accessible, I would deploy it as a simple web application using a framework like Streamlit or Hugging Face Spaces.
*   **Broader Evaluation:** I would evaluate the model's performance on a standardized test set (like WMT or FLORES) using metrics such as the BLEU score to quantitatively measure its translation quality.
