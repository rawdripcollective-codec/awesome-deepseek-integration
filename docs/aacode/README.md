# aacode

[aacode](https://github.com/kandada/aacode) is a Python-based CLI coding agent, similar to Claude Code and OpenCode, but lighter and more flexible, featuring pluggable model support for DeepSeek and beyond.

## Features

- **Lightweight ReAct Architecture**: Core logic is simple and relies on the model's own capabilities.
- **File-based Context**: Dynamic discovery using Markdown and other files as primary storage.
- **Versatile Bash Adapter**: Flexible system access through security guardrails.
- **Smart Context Management**: Intelligent reduction strategies inspired by Cursor and Manus.
- **Layered Tool System**: Atomic tools, code packages, and skills.
- **Security Guardrails**: Comprehensive command and path security checks.
- **Extensible Architecture**: Support for custom tools and model backends.

## Integration with DeepSeek

aacode supports DeepSeek as a primary model provider. You can configure it by setting the following environment variables:

```shell
export LLM_API_KEY="your-deepseek-api-key"
export LLM_API_URL="https://api.deepseek.com/v1"
export LLM_MODEL_NAME="deepseek-chat" # or deepseek-reasoner
export LLM_GATEWAY="openai"
```

## Available Tools

- **Atomic Tools**: `read_file`, `write_file`, `run_shell`, `list_files`, `search_files`.
- **Code Tools**: `execute_python`, `run_tests`, `debug_code`.
- **To-Do List Tools**: `delegate_task`, `add_todo_item`, `update_todo_item`.
- **Network Tools**: `web_search`.
