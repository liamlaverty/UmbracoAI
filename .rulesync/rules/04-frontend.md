---
root: false
targets: ["*"]
description: "Rules for working with front-end files"
globs: ["**/*"]
---

# Rules for working with front-end files

Page design should be consistent between all pages.

## Umbraco Templates

* When creating Umbraco Templates, this must be done via the Umbraco Template MCP tools.
* After Umbraco Templates have been created, modifying the cshtml file content directly via the file system is acceptable.
* Rendering Umbraco content in the cshtml files does NOT require additional plugins. Even for markdown editors, etc... Umbraco has all of the functionality built in to render this correctly using the standard syntax: `@Model.Value("propertyName")`

## Partial Views

* Razor partial views or components will need to be manually authored via the file system and stored at: src\MyProject\Views\Partials

## CSS

* CSS will need to be handled by writing to the physical file system.
* CSS files should be stored at: src\MyProject\wwwroot\css.
* CSS files stored there can be referenced in HTML by the absolute path /css/*.
* Don't create separate CSS files for every page. There should be one or many CSS files for the whole site. If page specific styles are required, they should be part either stored as part of the main site's CSS files, or included in the page includes as a separate page specific CSS include.