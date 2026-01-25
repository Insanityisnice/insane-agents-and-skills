# Insane Agents and Skills

This repository contains reusable GitHub Copilot agents and skills for modular use across multiple projects. 

## Usage
- Add this repository as a submodule in your project's `.github/instructions/` directory to share agents and skills.
- Agents and skills are organized in `.github/instructions/` for modular, progressive disclosure.

## Structure
- `.github/instructions/agents/` — Modular agent definitions (`*.instructions.md` and `AGENTS.md`)
  - `AGENTS.md` — Documentation of available agents
  - `csharp-expert.instructions.md` — Expert C# developer agent for simple, fully tested solutions
- `.github/instructions/skills/` — Modular skill files (`*.instructions.md`)

## Available Agents

### C# Expert Developer
An expert C# developer who excels at writing simple, clean, and fully tested executable solutions.

**Key Features:**
- Emphasizes simplicity over complexity
- Provides comprehensive test coverage (minimum 80%)
- Follows modern C# conventions and .NET best practices
- Includes project setup and build instructions
- Uses TDD approach with xUnit/NUnit/MSTest

See `.github/instructions/agents/AGENTS.md` for detailed documentation.

## Contribution
Please submit pull requests for new agents or skills. See CODEOWNERS for review requirements.
