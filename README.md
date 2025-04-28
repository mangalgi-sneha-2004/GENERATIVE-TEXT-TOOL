# GENERATIVE-TEXT-TOOL

COMPANY:CODTECH IT SOLUTIONS

NAME:MANGALGI SNEHA

INTERN-ID:CTO4WT53

DOMAIN:ARTIFICIAL INTELLIGENCE

DURATION:4 WEEKS

DESCRIPTION:

This Python script implements a robust text generation system using Hugging Face's GPT-2 model, designed for reliability across different hardware configurations. The code focuses on three core components: model 

loading, text generation, and memory management.

The system begins by automatically detecting available hardware (GPU/CPU) and loading the GPT-2 model with appropriate precision settings (float16 for GPU, float32 for CPU). It includes a fallback mechanism that 

attempts to load a smaller DistilGPT-2 model if the standard version fails, ensuring operation even on resource-constrained systems. The tokenizer is configured to use the end-of-sequence token as padding for 

consistent processing.

For text generation, the implementation uses nucleus sampling (top-p) with a temperature setting of 0.85, creating balanced outputs that are creative yet coherent. Key parameters like no_repeat_ngram_size prevent 

phrase repetition, while early_stopping terminates generation at natural breakpoints. The generate_text_gpt() function handles the entire process with comprehensive error catching, including specific handling for 

out-of-memory situations.

Memory management is a critical feature, with dedicated functions to clear GPU cache and Python's garbage collection between operations. This prevents the "CUDA out of memory" errors common in text generation 

tasks. The system also includes safety checks to verify model loading success before generation attempts.


The user interface offers both batch processing of example prompts and an interactive mode for custom inputs. Example prompts cover AI, autonomous vehicles, and neural networks, demonstrating the system's 

capabilities. During interaction, the code provides clear error messages and recovery suggestions when issues occur.



Technical safeguards include:

1.Automatic device mapping for GPU/CPU

2.Memory optimization through precision adjustment

3.Fallback to smaller models

4.Comprehensive error handling

5.Resource cleanup between generations


This implementation balances performance with reliability, making it suitable for both experimentation and production use. The modular design allows easy adaptation to different GPT variants or custom fine-tuned 

models, while the safety features ensure stable operation across diverse deployment environments. The code demonstrates best practices for deploying large language models in resource-constrained scenarios.


OUTPUT:

