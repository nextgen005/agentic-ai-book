# Chapter 6 — Advanced Tool Patterns
### Parallel Execution, Chaining, Browser Automation, and Observability

## Files
chapter6/

├── parallel_tools.py    ← asyncio parallel tool calling

├── chain.py             ← Tool chaining pipeline

├── resilient_tool.py    ← Retry + exponential backoff

├── tools/

│   └── browser.py       ← Playwright browser automation

├── observability.py     ← Tool call logger

└── universal_api.py     ← REST API to tool template

## What You Learn
- 4 tool execution patterns
- Parallel tool calling with asyncio (3x-10x faster)
- Tool chaining pipelines
- Retry logic with exponential backoff
- Browser automation with Playwright
- Converting any REST API to a tool
- Logging every tool call (observability)

## Setup
```bash
pip install playwright asyncio langchain-core requests
playwright install chromium
```

## Run
```bash
python parallel_tools.py     # See 3x speed improvement
python chain.py              # Full research pipeline
python observability.py      # View tool call logs
```
