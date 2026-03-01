# Install Ollama Locally

This guide walks you through installing Ollama on macOS, Linux, and Windows.

Ollama allows you to run large language models locally on your machine.

---

## 🖥 macOS

Install using Homebrew:

```bash
brew install ollama
```
Or download directly from:
https://ollama.com/download

Start the Ollama service:
```
ollama serve
```

🐧 Linux

Install via the official install script:
```
curl -fsSL https://ollama.com/install.sh | sh
```
Start Ollama:
```
ollama serve
```

Windows

Download the Windows installer:
https://ollama.com/download

Run the installer.

Open PowerShell and verify installation:
```
ollama --version
```
✅ Verify Installation

Check if Ollama is installed correctly:
```
ollama --version
```
You should see the installed version printed in your terminal.

⚙️ System Requirements

Minimum:

8GB RAM (16GB recommended)

10GB+ free disk space

macOS, Linux, or Windows

Performance depends heavily on:

RAM

CPU

GPU availability

🛠 Troubleshooting

If you get “command not found”:

Restart your terminal

Ensure Ollama is in your PATH

If models fail to run:

Ensure you have enough RAM

Try a smaller model like qwen2.5:0.5b

```

---

# 📄 `docs/USAGE.md`

```markdown
# Using Ollama

Once installed, you can download and run models locally.

---

## 📥 Pull a Model

Example: Pull a lightweight model

```bash
ollama pull qwen2.5:0.5b
```
This downloads the model to your machine.
