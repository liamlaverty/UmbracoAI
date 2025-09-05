---
description: 'Validate page rendering'
targets: ["*"]
---

# Validate that an Umbraco page renders

* Ensure the Home page renders by using the 'puppeteer' MCP tool to browse to the absolute URL of the published document and ensure there are no errors.
  * The absolute URL will be http://localhost:14737 + the relative path/URL of the published document which you can discern from its JSON definition or by calling 'get-document-urls'.
  * If there are errors, there will be a 'div' element with an id of 'stackpage'.
  * If there is an error, read what the error is that is rendered on the page and fix it in the Template.
  * Do not take screenshots to determine an error, you will need to read or evaluate the HTML content.