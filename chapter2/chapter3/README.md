# Chapter 3 — Tools, APIs and Giving Your Agent Hands
### Building the Interface Between AI and the Real World

## Files
chapter3/

├── tools/

│   ├── init.py       ← Tool registry

│   ├── search.py         ← Web search (Tavily)

│   ├── code_executor.py  ← Python executor

│   ├── file_tools.py     ← Read/Write files

│   ├── weather.py        ← Weather API

│   └── email_sender.py   ← Email via Gmail

└── test_tools.py         ← Test all tools

## What You Learn
- What is a tool in agentic AI
- Anatomy of a perfect tool (@tool decorator)
- Building 5 production-grade tools
- Tool selection via docstrings
- Tool design best practices

## Setup
```bash
pip install langchain-core tavily-python requests python-dotenv
```

## Environment Variables
OPENAI_API_KEY=your_key

TAVILY_API_KEY=your_key

OPENWEATHER_API_KEY=your_key

EMAIL_FROM=your@gmail.com

EMAIL_APP_PASSWORD=your_app_password

