# Week 8 Assignment – Single Agent System with Tool Routing

## Overview

This project implements a rule-based Single Agent System that intelligently routes user queries to different tools based on predefined conditions. The agent analyzes the user's input, identifies the requested task, and invokes the appropriate tool while returning responses in a structured JSON format.

---

## Objective

The objective of this assignment is to:

- Build a simple single-agent system.
- Implement conditional task routing.
- Route mathematical queries to a calculator tool.
- Route text queries to a keyword extraction tool.
- Handle general queries through a fallback response.
- Return structured JSON outputs.
- Validate the system using predefined test cases.
- Test the agent interactively using a continuous input loop.

---

## Features

- Mathematical expression evaluation
- Keyword extraction from text
- Conditional query routing
- Structured JSON responses
- Error handling for invalid inputs
- Automated validation test cases
- Interactive command-line interface

---

## Project Workflow

1. Import required libraries.
2. Create the Calculator Tool.
3. Create the Keyword Extraction Tool.
4. Implement the Agent Routing Function.
5. Validate the agent using test queries.
6. Test the agent interactively using a `while True` loop.

---

## Routing Logic

| User Query | Tool Used |
|------------|-----------|
| Contains **calculate** | Calculator Tool |
| Contains **keywords** | Keyword Extraction Tool |
| Any other query | General Response |

---

## JSON Output Format

Every response follows the structure:

```json
{
    "type": "calculation / keywords / general / error",
    "result": "output"
}
```

---

## Validation Examples

### Calculation

Input

```
calculate 25*6
```

Output

```json
{
    "type": "calculation",
    "result": 150
}
```

### Keyword Extraction

Input

```
keywords Machine Learning is transforming healthcare
```

Output

```json
{
    "type": "keywords",
    "result": [
        "machine",
        "learning",
        "transforming",
        "healthcare"
    ]
}
```

### General Query

Input

```
Hello
```

Output

```json
{
    "type": "general",
    "result": "I can help with calculations and keyword extraction."
}
```

### Error Handling

Input

```
calculate
```

Output

```json
{
    "type": "error",
    "result": "No mathematical expression found."
}
```

---

## Technologies Used

- Python
- Regular Expressions (`re`)
- JSON Module (`json`)
- Google Colab

---

## Conclusion

This project demonstrates a simple rule-based agent capable of routing user queries to specialized tools. The implementation includes conditional routing, structured JSON responses, validation testing, interactive execution, and robust error handling, fulfilling the requirements of the Week 8 assignment.
