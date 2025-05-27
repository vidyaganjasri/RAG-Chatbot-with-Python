# Running a Local LLM with Ollama – Beginner's Guide

This guide helps you set up and run a local language model on your machine using **Ollama**.

---

## Step 1: Create a Virtual Environment (Optional but Recommended)

Isolates your Python packages to avoid conflicts.

```bash
python -m venv .venv
.\.venv\Scripts\activate   # For Windows PowerShell
```
---

## Step 2: Install Ollama
Download the installer (OllamaSetup.exe) from the official website.

Run the installer.

Find the installation folder, e.g.:
```bash
C:\Users\<YourName>\AppData\Local\Programs\Ollama
```

Add this folder to your system’s Environment Variables > Path.

Open a new command prompt and verify installation:

```bash

ollama --version
```
---

## Step 3: Download and Run a Local Model
Example: Download and run Gemma 3, 1 billion parameter model

```bash
ollama run gemma3:1b
```

Ollama will download the model layers and start an interactive session:

```text
>>> hi how are you?
Hi there! I’m doing well, thanks for asking! 😊

>>> Tell me a joke
Why don’t scientists trust atoms? Because they make up everything! 😄

>>> /bye
```
---

## Step 4: (Optional) Install LangChain and Ollama Integration
To build advanced RAG (Retrieval-Augmented Generation) apps:

```bash
pip install langchain langchain-community langchain-ollama
```
Useful Commands
Check Ollama version:

```bash
ollama --version
```
List downloaded models:

```bash
ollama list
```
