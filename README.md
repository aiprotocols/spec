# AI Protocols Spec

**The canonical specification for AI Protocols — a unified standard for interacting with AI models across providers and languages.**

## 🧠 Overview

AI Protocols defines a consistent, language-agnostic interface for:

- Sending requests to AI models
- Receiving structured responses
- Streaming outputs in real-time
- Defining and executing tools/functions
- Managing conversation state and metadata

This repository contains the **canonical JSON Schema definitions**, along with documentation and examples.

## 📦 Repository Structure

```
schema/     → JSON Schema definitions (source of truth)
docs/       → Human-readable documentation for each schema
examples/   → Example payloads and usage patterns
```

## 🧩 Specification Structure

### Core Schemas

- [`ai-request.json`](schema/ai-request.json) → Model input definition
- [`ai-response.json`](schema/ai-response.json) → Model output structure
- [`stream-event.json`](schema/stream-event.json) → Streaming event protocol
- [`message.json`](schema/message.json) → Message structure
- [`tool.json`](schema/tool.json) → Tool/function definition
- [`conversation.json`](schema/conversation.json) → Optional conversation structure

## 📚 Documentation

Each schema is fully documented:

* [`docs/ai-request.md`](docs/ai-request.md)
* [`docs/ai-response.md`](docs/ai-response.md)
* [`docs/stream-event.md`](docs/stream-event.md)
* [`docs/message.md`](docs/message.md)
* [`docs/tool.md`](docs/tool.md)
* [`docs/conversation.md`](docs/conversation.md)

## ⚡ Examples

Real-world usage examples:

[`examples/`](examples/)

## 🎯 Design Principles

### Provider-agnostic

Abstracts differences between AI providers into a unified format.

### Language-agnostic

JSON Schema enables generation of types and models across ecosystems.

### Streaming-first

A unified event-based streaming protocol across all providers.

### Tool-native

Standardized function/tool calling interface.

### Conversation-aware & observable

Supports structured context through:

- `conversation_id`
- `context_key`

## 🛣 Versioning

* `v0.x` — experimental, subject to breaking changes
* `v1.0` — stable contract

## ⚠️ Status

This specification is in **early development (v0.x)**.
Breaking changes are expected until v1.0.

## 🤝 Contributing

Contributions are welcome.

Before contributing:
- Follow existing schema structure
- Keep changes provider-agnostic
- Update documentation and examples alongside schema changes

## 📜 License

[MIT](LICENSE)
