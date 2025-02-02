# TOPSIS-on-Text-Conversation-Models
**Text-Conversational Model Evaluation using TOPSIS**

## Overview
This project evaluates four text-to-text (T2T) models based on fluency, relevance, coherence, creativity, and accuracy using TOPSIS (Technique for Order of Preference by Similarity to Ideal Solution). The models evaluated include:

- **DialoGPT**
- **BlenderBot**
- **GPT-2**
- **Flan-T5**

## Evaluation Metrics
The following metrics were used to assess the output of the models:

1. **Fluency**: Measures how naturally the model constructs sentences.
2. **Relevance**: Assesses how relevant the generated response is to the given input.
3. **Coherence**: Checks if the response maintains logical consistency.
4. **Creativity**: Evaluates the originality and creativity of the response.
5. **Accuracy**: Measures how closely the response matches the correct answer.

## Example Question
**Question**: "Hi, how are you?"

## Correct Answer
**Correct Answer**: "Hello, I'm fine.How are you?"

## Example Output Matrix
Here’s an example of the evaluation matrix for the models:

| Model          | Fluency | Relevance | Coherence | Creativity | Accuracy |  
|----------------|---------|-----------|-----------|------------|----------|  
| **DialoGPT**   | 0.850   | 0.833     | 1.0       | 1.0        | 0        |  
| **BlenderBot** | 0.781   | 0.196     | 1.0       | 1.0        | 0        |  
| **GPT-2**      | 0.823   | 0.293     | 1.0       | 1.0        | 0.5      |  
| **Flan-T5**    | 0.815   | 0.0       | 0.0       | 0.0        | 0        |  

## Steps Followed
1. **Model Selection**: Loaded pre-trained models using Hugging Face's Transformers library.
2. **Evaluation Metrics**: Applied BLEU, ROUGE, and BERTScore to assess the output.
3. **Accuracy**: Implemented a custom function to calculate the accuracy of each response by comparing it to the correct answer.
4. **TOPSIS Application**: Applied the TOPSIS method for model ranking based on evaluation results.
5. **Results**: Generated model rankings and displayed the evaluation scores in a structured table.

## Tools & Libraries
- **Hugging Face Transformers**: For loading pre-trained models.
- **BertScore**: For fluency evaluation.
- **BLEU and ROUGE**: For creativity, coherence, and relevance evaluation.
- **rpy2**: For running the TOPSIS algorithm in R.
