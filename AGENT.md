# Claude Code Router Agent

This project acts as a flexible router for Claude Code, enabling users to direct requests to various Large Language Model (LLM) providers and customize these interactions through a robust transformation and plugin system. It provides dynamic model switching, comprehensive management tools, and seamless integration with development workflows.

**Key Technologies/Frameworks:**
Node.js, TypeScript, Fastify, ESBuild, Claude Code, various LLM APIs (OpenRouter, DeepSeek, Ollama, Gemini, Volcengine, SiliconFlow).

**Main Features:**
- **Model Routing**: Directs requests to specific LLMs based on task requirements (e.g., background, thinking, long context).
- **Multi-Provider Support**: Integrates with numerous LLM providers.
- **Request/Response Transformation**: Customizes payloads for provider compatibility via a plugin system.
- **Dynamic Model Switching**: Allows on-the-fly model changes within Claude Code.
- **CLI & UI Management**: Offers both command-line and web-based interfaces for configuration.
- **GitHub Actions Integration**: Facilitates automation in CI/CD pipelines.
- **Environment Setup**: Simplifies environment variable configuration for seamless use.

**Architectural Patterns:**
- **Gateway/Proxy**: Intercepts and reroutes requests to different downstream services.
- **Plugin Architecture**: Extensible design for custom transformers.
- **Configuration-driven**: Centralized `config.json` for managing settings and behaviors.
- **Multi-interface**: Provides both command-line and web-based user interaction.
