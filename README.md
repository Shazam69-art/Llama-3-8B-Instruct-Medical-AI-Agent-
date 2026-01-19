# Medical AI Agent

## Overview
Medical question-answering system using Llama 3 8B with external medical knowledge integration.  
[Project Repository](https://github.com/Shazam69-art/Llama-3-8B-Instruct-Medical-AI-Agent-/tree/main)

## Features
- Medical chain-of-thought reasoning  
- Clinical guideline search (WHO, NICE, CDC)  
- Drug information lookup  
- Accuracy verification pipeline  
- Real-time medical web search  

## Requirements
- NVIDIA GPU with 24GB+ VRAM (RTX 4090 / A5000 recommended)  
- 32GB+ system RAM  
- Python 3.8+  
- CUDA 11.8+  

## Installation
```bash
git clone https://github.com/Shazam69-art/Llama-3-8B-Instruct-Medical-AI-Agent-/tree/main
cd Llama-3-8B-Instruct-Medical-AI-Agent-
pip install torch transformers requests regex
huggingface-cli login
python medical_agent.py
Usage
python
Copy code
from medical_agent import MedicalAgent

agent = MedicalAgent()
result = agent.process_medical_query("Explain insulin resistance in Type 2 Diabetes")
print(result)
Architecture
Base Model: Meta-Llama-3-8B-Instruct

Medical Search: NIH, Mayo Clinic, WHO sources

Verification: Accuracy scoring with refinement

Output: Evidence-based medical answers

Important Note
For educational/research use only. Not for clinical use. Always verify information with healthcare professionals.
