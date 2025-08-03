# Mira Code Assistant

This project is a command-line AI agent powered by the Gemini API, designed to help you with your code. It can understand your code, help you fix bugs, and act as a miniature version of a code assistant like Claude Code.

## Features

*   **AI-powered:** Uses the Gemini API to understand and respond to user prompts related to code.
*   **File System Interaction:** Can read and analyze files from your local file system to understand the context of your code.
*   **Code Assistance:** Helps you fix bugs, understand code, and provides suggestions for improvements.
*   **Extensible:** The agent's functionality can be extended by adding new functions.

## Usage

To run the AI agent, you need to have a Gemini API key set as an environment variable.

```bash
export GEMINI_API_KEY="YOUR_API_KEY"
python main.py "your prompt here"
```

For example, you could ask it to fix a bug in the `calculator/main.py` file:

```bash
python main.py "Fix the bug in calculator/main.py"
```

You can also use the `--verbose` flag to see more detailed output.

```bash
python main.py --verbose "your prompt here"
```

## Example Project

The `calculator` directory contains a simple command-line calculator project. This is provided as an example project that you can use to test the AI agent's code-fixing capabilities.

## Project Structure

```
.
├── main.py             # Main entry point for the AI agent
├── calculator/         # Example project to test the agent on
│   ├── main.py
│   └── pkg/
│       └── calculator.py
└── functions/
    ├── get_file_content.py # Function for reading files
    └── ...             # Other functions for the agent
```
