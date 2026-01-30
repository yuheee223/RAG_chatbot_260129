# RAG chatbot - 旅遊不便險

一個基於 **Retrieval-Augmented Generation (RAG)** 架構的聊天機器人，能夠結合大型語言模型（LLM）與自有文件／知識庫，提供**更準確、可追溯、具上下文的回答**。

---

## Features

* 🔎 **Document Retrieval**：從向量資料庫中檢索最相關的文件片段
* 📄 **metadata**：自動判斷保險事件類型
* 🧠 **LLM Augmentation**：將檢索結果與使用者問題一起送入 LLM 生成回答
* 🛡️ **Reduced Hallucination**：回答基於實際文件內容

---

## System Architecture

```
User Query
   ↓
Embedding Model
   ↓
Vector Database 
   ↓
Relevant Documents
   ↓
LLM (with Prompt + Context)
   ↓
Final Answer
```

---

## Tech Stack

* **Language**: Python
* **LLM**:  HuggingFace 
* **Embedding**: Sentence-Transformers 
* **Vector DB**: FAISS / Chroma 
* **Framework**: LangChain 

---

## Project Structure

```
.
├── data/                # 原始文件
├── RAG_main.py/         
└── README.md
```

---

## Example Usage

```
User: 
Bot: 
```

---

## Future Improvements

* [ ] Conversation memory
* [ ] 

---

## Acknowledgements

* LangChain
* FAISS / Chroma
* HuggingFace

---

## 小筆記

- ChromaDB metadata 不支援 list，使用 JSON 或拆條存儲
