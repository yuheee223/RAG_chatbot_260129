# RAG chatbot - 旅遊不便險

這是一個基於旅行保險條款的問答系統，能夠：
- 將 PDF 條款分 chunk 並做 embedding
- 根據問題檢索相關條款
- 支援多事件（multi-event）標註
- 生成對使用者友善的答案

## 功能

- PDF 條款解析
- 自動判斷保險事件類型
- RAG 系統問答

## 注意事項

- ChromaDB metadata 不支援 list，使用 JSON 或拆條存儲
- API key 不要硬寫在程式碼中，使用環境變數
