[GitHub Models docs:](https://docs.github.com/en/github-models)

[Available models:](https://github.com/marketplace/models)

[Rate limits:](https://docs.github.com/en/rest/rate-limit)

    Tools and Model Context Protocol (MCP)
    Workflows use tools through the Model Context Protocol (MCP, a standardized protocol for connecting AI agents to external tools and services) for GitHub operations, external APIs, file operations, and custom integrations.

    Agentic workflows (workflows that have agency-the ability to make autonomous decisions) use AI to understand context, make decisions, and generate content by interpreting natural language instructions flexibly. They combine deterministic GitHub Actions infrastructure with AI-driven decision-making, adapting their behavior based on the specific situation they encounter.   

# Security Design

    Agentic workflows implement a defense-in-depth security architecture that protects against prompt injection, rogue MCP servers, and malicious agents. The architecture operates across multiple layers: compilation-time validation, runtime isolation, permission separation, network controls, and output sanitization.


