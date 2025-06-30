# Custom Chat Modes for GitHub Copilot

This repository contains a collection of custom chat modes for GitHub Copilot Chat. These modes are designed to tailor Copilot's behavior for specific software development tasks, making it a more efficient and specialized assistant.

## What are Chat Modes?

Custom chat modes allow you to define specific contexts and behaviors for GitHub Copilot. By specifying instructions and a curated set of tools, you can create specialized "experts" for different scenarios. You can learn more about them in the [official Visual Studio Code documentation](https://code.visualstudio.com/docs/copilot/chat/chat-modes).

## Available Modes

To use these modes, copy the desired `.chatmode.md` files into the `.github/chatmodes` directory of your own project.

Here are the modes available in this collection:

### Plan (`plan.chatmode.md`)
- **Description**: Generates a detailed implementation plan for new features or refactoring tasks without writing any code. It outlines the overview, requirements, implementation steps, and testing strategy.
- **Tools**: `codebase`, `fetch`, `findTestFiles`, `githubRepo`, `search`, `usages`

### Learn (`learn.chatmode.md`)
- **Description**: Helps you understand a new codebase, library, or technical concept. It provides explanations and examples but does not make code edits.
- **Tools**: `codebase`, `fetch`, `search`, `usages`

### Refactor (`refactor.chatmode.md`)
- **Description**: Focuses on improving and restructuring existing code. It can read, modify, and test code to enhance quality, readability, and performance without adding new features.
- **Tools**: `codebase`, `edit`, `findTestFiles`, `search`, `usages`

### Research (`research.chatmode.md`)
- **Description**: Gathers information from the web to answer questions and solve problems. It summarizes its findings before offering solutions.
- **Tools**: `fetch`, `search`

### Debug (`debug.chatmode.md`)
- **Description**: Assists in identifying and resolving bugs. It gathers context, asks clarifying questions, and proposes precise fixes.
- **Tools**: `codebase`, `edit`, `findTestFiles`, `search`, `usages`

### Yolo (`yolo.chatmode.md`)
- **Description**: Makes bold, direct changes to the codebase with minimal confirmation. This mode is for when you want swift, proactive action and are comfortable with a higher degree of automation.
- **Tools**: `codebase`, `edit`, `fetch`, `findTestFiles`, `githubRepo`, `search`, `usages`
