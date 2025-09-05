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
* Don't create separate CSS files for every page. There should be one or many CSS files for the whole site. If page specific styles are required, they should be part either stored as part of the main site's CSS files, or included in the page includes as a separate page specific CSS include.