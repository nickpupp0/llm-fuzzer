# Prompt Mutator – AI Prompt Fuzzing Tool

## Overview

**Prompt Mutator** is a lightweight Python CLI tool designed for AI / LLM security research, prompt injection testing, and CTF-style training.

The tool takes an input prompt and generates mutated adversarial variants using OpenAI via LangChain. Mutations are controlled using:

- **Temperature** – to influence creativity and chaos
- **Keyword steering** – to inject specific concepts into the mutated prompt

The goal is to model how **adversarial prompts evolve** while preserving their original intent — a common challenge in **LLM penetration testing and red teaming**.

---

## Use Cases

This project is useful for:

### 🔐 AI / LLM Penetration Testing
- Studying how prompt injection attempts change phrasing
- Generating adversarial prompt variants for robustness testing
- Exploring instruction confusion and intent preservation
- Practicing AI-focused CTF challenges
- Understanding how prompt-based attacks escalate

⚠️ **This tool rewrites prompts only.**  
It does **not** execute instructions, decode data, or target live systems.

---

## Features

- OpenAI + LangChain integration
- Temperature-based mutation (`0.0 → 1.0`)
- Keyword injection for prompt steering

---

## Project Structure

```text
prompt-mutator/
├── fuzzer.py          
├── requirements.txt   
├── README.md          
├── .env               
└── .gitignore

