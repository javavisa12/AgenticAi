# AgenticAi

* Extension * : continue
* Run * :  python -m llama_cpp.server --model Ai-Agent\models\Qwen3.5-2B-Q8_0.gguf --n_ctx 8192




config.yaml

name: Local Config
version: 1.0.0
schema: v1

models:
  - name: Qwen Local
    provider: openai
    model: Ai-Agent\models\Qwen3.5-2B-Q8_0.gguf
    apiBase: http://localhost:8000/v1
    apiKey: dummy
    roles:
      - chat
      - edit
      - apply
    systemMessage: "You are a helpful coding assistant. Be concise."
