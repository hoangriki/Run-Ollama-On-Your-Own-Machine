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

💬 Run a Chat Session

```
ollama run qwen2.5
```
You can now interact with the model directly in your terminal.

Type your prompt and press Enter.

Exit with:
```
/bye
```
