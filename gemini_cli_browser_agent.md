# Demo: Gemini CLI Browser Agent (v0.31.0)

This walkthrough demonstrates the new **Experimental Browser Agent** in Gemini CLI, which allows you to interact with live web pages directly from your terminal.

## Use Case
A developer needs to extract the latest pricing information from a competitor's website or check the status of a cloud service without leaving their terminal.

## Steps

### 1. Update Gemini CLI
Ensure you are on the latest version (v0.31.0+).
```bash
gemini update
gemini --version
```

### 2. Enable the Browser Agent
The browser agent is an experimental feature that uses a headless browser to "see" and "interact" with web pages.

### 3. Extract Information from a Web Page
Ask Gemini to visit a URL and perform a task.
```bash
gemini "Visit https://cloud.google.com/bigquery/pricing and summarize the latest pricing for 'Global Queries' in a table."
```

### 4. Interactive Web Task
You can even ask it to perform actions like searching.
```bash
gemini "Go to the Google Cloud Blog, search for 'MCP Server', and give me the titles of the top 3 results from February 2026."
```

## Things to remember or know
- **Contextual Intelligence**: The agent doesn't just "fetch" the HTML; it "renders" the page to understand dynamic content (JavaScript).
- **Developer Productivity**: Drastically reduces context switching between the IDE/Terminal and the Browser.
- **Agentic Workflows**: This can be integrated into larger shell scripts for automated market research or system health checks.
