# openwebui-podman-compose

## About

Open WebUI is an extensible, feature-rich, and user-friendly self-hosted AI platform designed to operate entirely offline. It supports Ollama and OpenAI-compatible APIs, making it a powerful, provider-agnostic solution for both local and cloud-based models.

## Usage

Deploy the stack and visit [http://localhost:3000/](http://localhost:3000/).

## Configuration

### openwebui-kokoro-fastapi-cpu

| Settings                    | Value                                         |
| --------------------------- | --------------------------------------------- |
| Text-to-Speech Engine (URL) | `http://openwebui-kokoro-fastapi-cpu:8880/v1` |
| Text-to-Speech Engine (KEY) | `not-needed`                                  |
| TTS Voice                   | `zf_xiaoxiao` (for Chinese)                   |
| TTS Model                   | `kokoro`                                      |

### openwebui-searxng

| Settings          | Value                                            |
| ----------------- | ------------------------------------------------ |
| Web Search        | `<ON>`                                           |
| Web Search Engine | `searxng`                                        |
| Searxng Query URL | `http://openwebui-searxng:8080/search?q=<query>` |

### openwebui-openterminal

| Settings | Value                                  |
| -------- | -------------------------------------- |
| URL      | `http://openwebui-openterminal:8000`   |
| Auth     | `Bearer`                               |
| API Key  | `254b0775-5e72-4779-bcb3-985abf754c3f` |
