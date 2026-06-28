# IS6620 Group Assignment - Streamlit App

键盘出海内容自动化与审核平台 (DeepSeek + Qdrant Cloud RAG)

## 功能

- ✅ 基于 DeepSeek API 生成营销内容
- ✅ 基于 Qdrant Cloud 实现 RAG 检索
- ✅ 多轮迭代优化（Drafter + Critic Agent）
- ✅ 支持中文输入，自动翻译为英文
- ✅ 合规检查（竞品词、违禁词、术语规范）

## 部署到 Streamlit Community Cloud

1. Fork 或上传此仓库到你的 GitHub
2. 访问 https://share.streamlit.io
3. 点击 "New app"，选择此仓库
4. 在 "Advanced settings" → "Secrets" 中填入：

```toml
DEEPSEEK_API_KEY = "your-deepseek-api-key"
QDRANT_URL = "your-qdrant-cluster-url"
QDRANT_API_KEY = "your-qdrant-api-key"
```

5. 点击 "Deploy"，等待 2-5 分钟

## 本地运行

```bash
pip install -r requirements.txt
streamlit run IS6620_GroupAssignment_Group21.py
```

在侧边栏填入 API Key 即可使用。

## 依赖

- streamlit
- openai
- qdrant-client
- fastembed
