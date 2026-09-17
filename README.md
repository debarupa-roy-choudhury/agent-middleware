## 📂 Repository Structure

Agentic AI Engineering with Python: Agent Middleware

```
📁 Agent Middleware/
│   └── middleware/                 # Controlling an agent without rewriting it
│       ├── nomiddleware.py         # The baseline agent, before any middleware
│       ├── middleware-basic1.py    # The four hooks: before/after model, wrap model/tool
│       ├── dynamic-prompt-mw.py    # System prompt built per request from context
│       ├── dynamic-model-mw.py     # Route easy questions to a cheap model, hard ones to a strong one
│       ├── dynamic-tool-mw.py      # Expose different tools depending on the request
│       ├── tool-retry-mw.py        # ToolRetryMiddleware when a tool call fails
│       ├── summary-mw.py           # SummarizationMiddleware to keep long chats in budget
│       ├── custom-state.py         # Customizing agent state with our own keys
│       ├── pii-middleware.py       # Built-In PIIMiddleware for PII data
│       └── .env                    # OpenAI key goes here
│
└── 📄 README.md

```