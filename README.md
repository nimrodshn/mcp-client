# MCP Client

A simple Go client for the Model Context Protocol (MCP) that connects to MCP servers and calls tools.

## Usage

```bash
go run main.go -name "World"
```

## Description

This client connects to an MCP server running on `localhost:8080` and calls a "greet" tool with the provided name parameter. The server response is then printed to the console.

## Connecting to Claude

To connect to Claude via MCP:

1. Install and configure the Claude desktop app with MCP support
2. Set up your MCP server configuration in Claude's settings
3. Update the server URL in `main.go` to point to your Claude MCP endpoint
4. Ensure your Claude instance is running and accepting MCP connections

For detailed Claude MCP setup instructions, see the [Claude MCP documentation](https://docs.anthropic.com/en/docs/build-with-claude/computer-use).

## Requirements

- Go 1.24.5+
- MCP server running on localhost:8080 (or Claude MCP endpoint)

## Dependencies

- [MCP Go SDK](https://github.com/modelcontextprotocol/go-sdk) v0.2.0