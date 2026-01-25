# Usage Examples

This document provides examples of how to use the agents in this repository.

## Setting Up as a Submodule

To use these agents in your project:

```bash
# Navigate to your project root
cd /path/to/your/project

# Add this repository as a submodule
git submodule add https://github.com/Insanityisnice/insane-agents-and-skills.git .github/instructions/shared

# Or if you want to map it directly to the instructions folder:
git submodule add https://github.com/Insanityisnice/insane-agents-and-skills.git .github/instructions
```

## Using the C# Expert Agent

Once set up as a submodule in `.github/instructions/`, GitHub Copilot will automatically discover and apply the agent instructions when working on C# files. The agent's guidance influences code generation, suggestions, and best practices.

### Example: Creating a Simple Calculator

When you interact with GitHub Copilot in a C# project, the agent instructions are automatically applied:

**Prompt to Copilot:**
```
Create a simple calculator class that can add, subtract, multiply, and divide numbers. Include comprehensive tests.
```

**Expected Output Structure:**
```
Calculator/
├── src/
│   └── Calculator/
│       ├── Calculator.cs
│       ├── Program.cs
│       └── Calculator.csproj
└── tests/
    └── Calculator.Tests/
        ├── CalculatorTests.cs
        └── Calculator.Tests.csproj
```

The agent will:
1. Create a simple, clean Calculator class
2. Provide comprehensive unit tests with xUnit
3. Include example usage in Program.cs
4. Add instructions to build and run

### Example: Web API with Tests

**Prompt to Copilot:**
```
Create a minimal REST API with a User endpoint (CRUD operations) including integration tests
```

The agent will create:
- Clean API implementation using ASP.NET Core
- Entity and DTOs
- Controller with CRUD operations
- Integration tests with WebApplicationFactory
- Setup instructions

### Example: Code Review

**Prompt to Copilot:**
```
Review this C# code for best practices and suggest improvements
```

The agent will:
- Check for simplicity and clarity
- Verify test coverage
- Suggest improvements following .NET best practices
- Identify potential issues

## Benefits

1. **Consistency**: All C# code follows the same standards
2. **Quality**: Enforces best practices and comprehensive testing
3. **Speed**: Quick setup with proper project structure
4. **Learning**: Demonstrates good C# patterns and practices

## Customization

You can customize the agent behavior by:
1. Forking this repository
2. Modifying the agent instructions
3. Using your fork as the submodule source

## Feedback and Contributions

If you have suggestions for improving the agents or want to add new ones, please submit a pull request or open an issue.
