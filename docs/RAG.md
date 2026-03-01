🔒 Why RAG + Local AI Is Powerful

Full privacy

No API costs

Works offline

Custom knowledge base
```

---

# 📄 `docs/CUSTOM_PERSONA.md`

```markdown
# Creating a Custom Persona with a Modelfile

Ollama allows you to customize model behavior using a Modelfile.

This works similarly to Dockerfiles — you define how the model should behave.

---

## 📝 Create a Modelfile

Create a file named:
```
Modelfile
```

Example:
```

FROM qwen2.5

SYSTEM You are a sarcastic but helpful AI assistant who explains concepts simply.
```

---

## 🏗 Build the Custom Model

```bash
ollama create sarcastic-assistant -f Modelfile
```
▶️ Run It
```
ollama run sarcastic-assistant
```
🎯 Advanced Customization

You can:

Change base models

Add system prompts

Control temperature

Adjust parameters

Example with temperature:
```
FROM qwen2.5
PARAMETER temperature 0.2
SYSTEM You are a professional DevOps mentor.
```
