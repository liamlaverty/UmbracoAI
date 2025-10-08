---
root: false
targets: ["*"]
description: "Rules for using MCP tools"
globs: ["**/*"]
---

# Rules for using MCP tools

## Common Rules

* If a task/command asks to use a specific MCP tool and the tool fails, DO NOT try to use an alternative.

## Umbraco MCP

* Not installed, do not attempt to install it

## Browser commands

- Use the "playwright" MCP server for browser commands.
- When navigating to browser URLs, use the "browser_navigate" mcp server command.
- When zooming in the browser, use the "browser_evaluate" mcp server command + javascript. Example: `document.body.style.zoom='75%'`
- When scrolling in the browser, use the "browser_evaluate" mcp server command + javascript. Example: `window.scrollTo(0, document.body.scrollHeight)` to scroll to the bottom of the page and `window.scrollTo(0, 0)` to scroll to the top of the page.
- When waiting for a period of time when loading web pages with "playwright", is the browser_wait_for command.

### Closing the browser

- When you are done with browser commands, close the browser using the "browser_close" mcp server command.