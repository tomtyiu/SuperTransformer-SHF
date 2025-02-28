# SuperTransformer

Suptertransformer that auto loads Huggingface models 

# Introduction
This is a single line transformer for easy to load models from Huggingface.

# Usage
SuperTransformers download the model locally.  The super class uses AutoTokenizer and AutoModelForCausalLM.from_pretrained.

# Example of usage:
```python
# (1) Loads Huggingface model, (2) System Prompt (3) Text (4)Max tokens
SuperTransformers = SuperTransformers("EpistemeAI/ReasoningCore-3B-RE1-V2","You are a highly knowledgeable assistant with expertise in chemistry and physics. <reasoning>","What is the area of a circle, radius=16, reason step by step", 2026)
# 8-bit quantization
SuperTransformers.HuggingFaceTransformer8bit()
# or 4-bit quantization
SuperTransformers.HuggingFaceTransformer4bit()

```
