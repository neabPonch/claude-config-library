---
name: brguru90__multi_tool_executer_mcp
source: https://github.com/brguru90/multi_tool_executer_mcp/blob/b599dbd45e79b10c28a463f20ea2138eda37aba3/CLAUDE.MD
repo: brguru90/multi_tool_executer_mcp
kind: claude-md
stars: 0
last_pushed: 2025-10-11T19:54:35Z
license: unknown
score: 7
domains: [agents-ai, cli-tools, wasm]
tags: [mcp, rustpython, wasmedge, dynamic-execution]
curated: 2026-06-14
curated_by: config-scout
---

# brguru90/multi_tool_executer_mcp — claude-md

**Why it's worth keeping:** Provides extreme technical precision for complex runtime environments (WASM/RustPython) and exact function templates for tool orchestration.

**Summary:** Defines a highly specialized MCP server architecture using WasmEdge and RustPython to execute dynamic Python code within a virtual file system.

**Source credibility:** Low; based on an unstarred, undocumented repository with no clear author context.

**Recency:** Current; utilizes modern MCP and FastMCP standards.

**Source:** [brguru90/multi_tool_executer_mcp/CLAUDE.MD](https://github.com/brguru90/multi_tool_executer_mcp/blob/b599dbd45e79b10c28a463f20ea2138eda37aba3/CLAUDE.MD) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# the goal of project is to support python requests,sockets and FastMCP libraries to write MCP server which can execute python code.

## Detailed instruction to achieve the goal,
1. install wasmedge or compile & install wasmedge if some additional feature has to be enabled
2. compile and install RustPython with the python packages like requests,sockets and fastmcp
3. make use of webassembly virtual file system(VFS),create FastMCP server within virtual file system and FastMCP server should able to dynamically write python scripts and executes at runtime
4. when FastMCP server start with should create the UID for its instance
5. wasm program should either accept command line arguments or as environment variable with key as MCP_SERVERS_CONFIGS: Dict[Dict](input will be JSON string)
below is the vscode configuration
{
    "servers": {
        "multi_mcp_tool_executer": {
            "type": "stdio",
            "command": "wasmedge",
            "args": [
                "wasm_mcp_tool_executer.wasm",
            ],
            "env": {
                // below is MCP config for tool itself to call the tools internally
                "MCP_SERVERS_CONFIGS": "{
                    \"con
```

</details>
