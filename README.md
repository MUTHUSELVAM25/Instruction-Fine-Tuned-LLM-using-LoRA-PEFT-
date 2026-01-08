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

---
⚙️ Model Architecture

| Component            | Details                  |
| -------------------- | ------------------------ |
| Base Model           | DistilGPT-2              |
| Fine-Tuning          | LoRA (PEFT)              |
| Trainable Parameters | < 1%                     |
| Task Type            | Causal Language Modeling |

---

🧪 Base Model vs Fine-Tuned Model
❌ Base Model (Without LoRA)

=> Repeats prompt structure
=> Does not follow instructions
=> Produces incoherent or looping outputs

✅ LoRA Fine-Tuned Model

=> Understands instruction–response format
=> Generates meaningful answers
=> Responds differently based on input constraints

This confirms successful instruction tuning.

---

🧠 Input Conditioning Behavior

The Input field directly affects response style and length:

| Input Example                   | Output Behavior                |
| ------------------------------- | ------------------------------ |
| `say simple and correct answer` | Short, concise response        |
| `none`                          | Longer, more detailed response |

This demonstrates conditional generation, a core property of instruction-tuned LLMs.


---


🖥️ Gradio Demo

An interactive Gradio UI allows users to:

=> Enter an instruction
=> Provide optional constraints
=> Observe real-time model responses
=> This makes the project suitable for demos and portfolios.

---


📈 Learning Outcomes

=> Instruction tuning concepts
=> LoRA / PEFT fine-tuning
=> Prompt formatting for LLMs
=> Decoding strategies for text generation
=> Deploying LLMs with Gradio

---






