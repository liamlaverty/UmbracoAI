---
root: false
targets: ["*"]
description: "Rules for working with front-end files"
globs: ["**/*"]
---

# Rules for working with front-end files

* Html, Razor and Template authoring should be done with the Umbraco Template MCP tools.
* CSS will need to be handled by writing to the physical file system.
* CSS files should be stored at: src\MyProject\wwwroot\css.
* CSS files stored there can be referenced in HTML by the absolute path /css/*.
