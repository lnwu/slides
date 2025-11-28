---
theme: default
title: MCP & Custom Agent Instructions
info: |
  ## Understanding MCP and Customizing Agent/Plan Mode
  A presentation about Model Context Protocol and how to customize agent behavior
class: text-center
transition: slide-left
---

# What is MCP?

Model Context Protocol

<div class="pt-12">
  <span class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Press Space for next page →
  </span>
</div>

---
layout: default
---

# What is MCP?

MCP (Model Context Protocol) is an **open protocol** that standardizes how applications provide context to LLMs.

<v-clicks>

- 🔌 **Universal Connectivity** - Connect AI assistants to any data source
- 🛠️ **Tool Integration** - Expose functionality as tools for AI to use
- 📊 **Context Management** - Provide relevant context to improve responses
- 🔒 **Secure Communication** - Standardized, secure data exchange

</v-clicks>

---
layout: default
---

# MCP Architecture

### Host Application
- Contains the LLM integration
- Manages MCP client connections
- Examples: Claude Desktop, IDE extensions

### MCP Server
- Provides resources/tools/prompts
- Runs locally or remotely
- Can access local files, databases, APIs

---

# MCP Server Capabilities

| Capability | Description |
|------------|-------------|
| **Resources** | Expose data like files, database records, API responses |
| **Tools** | Provide executable functions the AI can call |
| **Prompts** | Pre-defined prompt templates for common tasks |

<br>

### Example: GitHub MCP Server
- Browse repositories and files
- Search code across repos
- Manage issues and pull requests
- Execute workflows

---
layout: section
---

# Customizing Agent Instructions

---

# What are Custom Agent Instructions?

Custom instructions let you **modify AI behavior** for specific contexts.

<v-clicks>

### Use Cases:
- 🎯 **Coding Style** - Enforce team conventions
- 📝 **Documentation** - Standardize formats
- 🔐 **Security** - Add security review steps
- 🧪 **Testing** - Define test requirements

</v-clicks>

---

# Plan Mode vs Agent Mode

### Plan Mode 📋
- Creates detailed execution plans
- Reviews changes before making them
- Good for complex, multi-step tasks
- More deliberate and cautious

### Agent Mode 🤖
- Executes actions directly
- Faster for straightforward tasks
- Autonomous decision-making
- Better for well-defined operations

---

# Customizing Instructions

### Where to Define Custom Instructions

```
.github/
├── copilot-instructions.md      # General instructions
├── agents/
│   ├── plan-mode.md             # Plan mode specific
│   └── agent-mode.md            # Agent mode specific
```

### Example: Custom Coding Agent

```markdown
# Custom Agent Instructions
- Always use TypeScript for new files
- Add JSDoc comments to public functions
- Run linter before committing
- Write unit tests for new features
```

---

# Best Practices

<v-clicks>

1. **Be Specific** - Clear, actionable instructions
2. **Keep Updated** - Maintain as project evolves
3. **Team Alignment** - Share with your team
4. **Iterate** - Refine based on results
5. **Document** - Explain the "why"

</v-clicks>

---
layout: center
class: text-center
---

# Summary

<div class="text-left inline-block">

✅ MCP standardizes AI-to-data connections

✅ Custom instructions tailor AI behavior

✅ Plan mode for complex tasks, Agent mode for direct execution

✅ Use `.github/` folder for project-specific configurations

</div>

---
layout: center
class: text-center
---

# Thank You!

Learn more at [modelcontextprotocol.io](https://modelcontextprotocol.io)
