# Rap Lyric Generator Using Deep Learning and LLM models

## Introduction
This project aims to explore rap music and hip hop as genre. We take a dig on phonetics and rhyming scheme for the rap music and generate rap lyrics with the help of three models :-
1. distilgpt2-rap : hugging face link(https://huggingface.co/dzionek/distilgpt2-rap)
2. GPT2-finetuned-lyric-generation : hugging face link(https://huggingface.co/SpartanCinder/GPT2-finetuned-lyric-generation)
3. Ngrams - created by our own

We fine tune these models on our curated dataset collected from musicmatch api.

Then we compare and contrast above models based on different quantitative metrics.


## Objectives
* Data Collection and Preprocessing: Sourcing data from Musixmatch API, with preprocessing including grapheme-to-phoneme conversion. It contains around 30 artists with 50 songs each.
* Model Experimentation: The project involved Hyperparamter fine-tuning on train datasets on different models such as distilgpt2-rap, GPT2-finetuned and N-grams with phoneme-grapheme conversions.


## Model Training
* Training involved multiple sessions on Google Colab using Tesla V100 GPUs, utilizing the capability to reload from checkpoints for continuous training.
https://drive.google.com/file/d/1JEK95SayQL8wMx6JAHpzOmzKd6GUsKW_/view?usp=sharing

## Deployment Architecture and Accessibility
Due to cost and resource limitations, we did not deploy the project yet. But look forward to do so in the future.

## Cost and Time Consideration
Balancing cost-efficiency and performance, the project's execution was done on Google Collab. Initially, everything was executed and fine tuned with smaller datasets on free tiers but later we purchased google collab pro and apparantly we burnt out all our computational resources, system ram and GPUs. Fine tuning on larger datasets is a computationally heavy and costly task.

## Evaluation and Future Improvements
* Lyric Quality: The model's ability to rhyme and maintain meter is an ongoing developmental focus. But We were able to produce decent results, and it is fine to produce non copyrighted music with the help of AI
* Future Research : Ongoing research and development on adding and auto tuning background music with AI so that it can be used as a copyright free music suite.

## Conclusion
This capstone project represents an ambitious foray into combining machine learning with artistic creativity. It demonstrates the challenges and potential of using natural language processing in the creative domain of Hip Hop lyricism.
