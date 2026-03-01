🌐 Using the REST API

Ollama runs a local server at:

```
http://localhost:11434
```

Example curl request:
```
curl http://localhost:11434/api/generate -d '{
  "model": "qwen2.5",
  "prompt": "Explain local AI in simple terms"
}'
```
This is how your Python or Node apps will communicate with Ollama.
```

---

# 📄 `docs/RAG.md`

```markdown
# Retrieval-Augmented Generation (RAG)

Local models do not automatically know your personal data or documents.

RAG allows you to:
1. Retrieve relevant information from your own data
2. Inject that data into the prompt
3. Generate better, context-aware answers

---

## 🧠 Why RAG Is Important

Local models:
- Do not access the internet
- Cannot see your private files
- Only know what was in their training data

RAG solves this by supplying context manually.

---

## 🔁 Basic RAG Flow

1. Store your documents
2. Convert them into embeddings
3. Search for relevant chunks
4. Add retrieved text into the model prompt
5. Generate a response

---

## 🧩 Simple Example (Manual RAG)

Instead of full embedding pipelines, you can simulate RAG like this:

```bash
ollama run qwen2.5 "Using this context: 
Our company was founded in 2022 and builds AI tools.
Question: When was the company founded?"
```
