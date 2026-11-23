# bf16.ai Model Provider for Dify

Official Dify model provider plugin for [bf16.ai](https://bf16.ai), providing OpenAI-compatible inference across 1M-context uncensored open-weight models with strict zero data retention and pay-as-you-go pricing.

## Supported Models

| Model ID | Context | Max Output | Multimodal | Capabilities |
| --- | --- | --- | --- | --- |
| `zai-org/glm-5.3-uncensored` | 1M | 131,072 | Text | Tool calling, structured output, reasoning |
| `deepseek/deepseek-v4.1-flash-uncensored` | 1M | 130,000 | Text + Vision | Tool calling, structured output, reasoning |
| `deepseek/deepseek-v4.1-flash-uncensored-fast` | 1M | 130,000 | Text + Vision | Tool calling, structured output, reasoning |
| `zai-org/glm-5.3-flash-uncensored` | 1M | 131,072 | Text + Vision | Tool calling, structured output, reasoning |
| `moonshotai/kimi-k3.1-pro-uncensored` | 1M | 131,072 | Text + Vision | Tool calling, structured output, reasoning |

## Configuration

1. Create an API key in the [bf16.ai Developer Console](https://bf16.ai/dashboard/keys).
2. In Dify, go to **Settings -> Model Provider -> bf16.ai**.
3. Enter your `sk-bf16-v1-...` API key (and optionally override the API Base URL; defaults to `https://api.bf16.ai/v1`).

## Usage

1. After saving your API key in **Settings -> Model Provider -> bf16.ai**, select any bf16.ai model (such as `deepseek/deepseek-v4.1-flash-uncensored-fast` for low-latency agent loops or `moonshotai/kimi-k3.1-pro-uncensored` for complex reasoning) in your Dify **Chatflow**, **Workflow**, or **Agent** LLM node.
2. Adjust parameters such as temperature, max tokens, structured JSON output, and tool calling directly from the Dify model configuration panel.
3. All inference requests default to strict zero data retention (ZDR) and support up to 1M input context tokens.

## Documentation

- API docs: https://bf16.ai/docs
- Live pricing & rate tiers: https://bf16.ai/pricing

## Source Repository & Support

- Source repository: https://github.com/BF16-AI/bf16-dify-plugin
- Documentation & setup guide: https://bf16.ai/docs/clients/dify
- Contact: hello@bf16.ai
