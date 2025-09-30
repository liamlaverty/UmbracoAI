---
root: true
targets: ["*"]
description: "Rules for using MCP tools"
globs: ["**/*"]
---

# Rules for using tools

## Umbraco MCP

* If the Umbraco MCP tool is not running, do not attempt to modify Umbraco content.
* The Umbraco MCP tool may not work if the website is not running.
* If, the website is running and the MCP tool fails, notify the user, do not attempt to complete Umbraco tasks without it.

## Puppeteer MCP

* Do not take screenshots to determine a page rendering error, you will need to read or evaluate the HTML content.