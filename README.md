# Instruction-Fine-Tuned-LLM-using-LoRA-PEFT-
Fine-tuning a Large Language Model (LLM) for instruction-following tasks using LoRA (Low-Rank Adaptation) and the Alpaca dataset, with an interactive Gradio demo.

---

# 🧠 Instruction Fine-Tuned LLM using LoRA (PEFT)

This project demonstrates how to fine-tune a **Large Language Model (LLM)** for instruction-following tasks using **LoRA (Low-Rank Adaptation)** on the **Alpaca dataset**, with an interactive **Gradio web interface**.

---

## 📌 Project Overview

The goal of this project is to convert a pretrained language model into an **instruction-following assistant** using **parameter-efficient fine-tuning**.

- **Base Model:** DistilGPT-2  
- **Fine-Tuning Method:** LoRA (PEFT)  
- **Dataset:** Alpaca (instruction–input–response format)  
- **Interface:** Gradio  

The model learns to respond correctly to structured prompts containing:
- Instruction  
- Optional Input (constraints)  
- Response  

---

## 🎯 Key Features

- Instruction-tuned language model
- LoRA-based parameter-efficient fine-tuning
- Base model vs fine-tuned model comparison
- Input-controlled response length and style
- Interactive Gradio UI for testing

---

## 🧩 Dataset

**Alpaca Dataset** (`tatsu-lab/alpaca`)

Each training example follows this format:

Instruction:
<Task>
Input:
<Optional context>
Response:
<Expected answer> ```

This structure helps the model learn instruction alignment instead of prompt repetition.


