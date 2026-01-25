# Available Agents

This directory contains specialized agent configurations for GitHub Copilot. Each agent is an expert in a specific domain and provides guidance, best practices, and code generation capabilities.

## How to Use Agents

Agents are invoked through GitHub Copilot by referencing them in your interactions. Place this repository as a submodule in your project's `.github/instructions/` directory to make these agents available.

## Agent List

### C# Expert Developer (`csharp-expert.instructions.md`)

**Purpose**: Expert C# developer who excels at writing simple, clean, and fully tested executable solutions.

**Best For**:
- Creating new C# applications or libraries
- Writing testable C# code with comprehensive test coverage
- Implementing solutions following .NET best practices
- Setting up C# project structures with testing infrastructure
- Code reviews for C# code quality and simplicity

**Key Features**:
- Emphasizes simplicity and clarity over complexity
- Provides fully tested solutions (minimum 80% coverage)
- Follows modern C# conventions (C# 10+)
- Includes project setup and build instructions
- Uses TDD approach with xUnit/NUnit/MSTest
- Applies SOLID principles appropriately

**When to Use**:
- You need a C# solution with comprehensive tests
- You want to follow C# best practices
- You need help structuring a C# project
- You want simple, executable code examples

## Adding New Agents

To add a new agent:

1. Create a new `{agent-name}.instructions.md` file in this directory
2. Document the agent's expertise, principles, and usage patterns
3. Update this AGENTS.md file with the new agent information
4. Submit a pull request for review

## Agent Template Structure

Each agent file should include:
- Agent description and core principles
- Code standards and conventions
- Common patterns and examples
- Usage instructions
- When to use this agent

See `csharp-expert.instructions.md` for a complete example.
