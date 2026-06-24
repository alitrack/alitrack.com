+++
title = "OpenFusion"
description = "Open-source multi-model fusion engine — self-hosted OpenRouter alternative"
repo = "https://github.com/alitrack"
lang = "Go"
+++

开源多模型融合编排引擎。在自己基础设施上运行，不绑定任何模型供应商。

- Pluggable backends (Anthropic, OpenAI, DeepSeek, Ollama...)
- Cost/latency/rule-based routing
- Response streaming, caching, rate limiting
- OpenAI-compatible API endpoint

```go
router := fusion.New(
    fusion.WithModel("claude-sonnet-4", anthropicBackend),
    fusion.WithModel("deepseek-v4", deepseekBackend),
    fusion.WithStrategy(fusion.CostOptimized),
)
```
