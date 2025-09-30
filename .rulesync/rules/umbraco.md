---
root: false
targets: ["*"]
description: "Umbraco best practices"
globs: ["**/*"]
---

# Umbraco best practices

## MCP Integration

When interacting with Umbraco, use the "umbraco-mcp" MCP tool.

## Running the website

* The web application will normally already be running at http://localhost:14737, if its not, it can be started by running `dotnet run --project src/MyProject/MyProject.csproj` from the root of this workspace.

## Umbraco backoffice and schema

* Do not create or modify Users.
* Do not create or modify Members.
* Do not create or modify Translations or Dictionary items.
* Do not install Packages.
* Do not create or use document blueprints.
* Do not create custom Property Editors, only use the built in ones.
* Do not be concerned about Public Access.
* Do not be concerned about Domains.
* Do not be concerned about Variants or Segments.

## How to guides

Read or reference the following articles to understand Umbraco best practices:

* What is a Property Editor? https://docs.umbraco.com/umbraco-cms/fundamentals/backoffice/property-editors 
  * Built in property editors: https://docs.umbraco.com/umbraco-cms/fundamentals/backoffice/property-editors/built-in-umbraco-property-editors 
* How to define content and document types: https://docs.umbraco.com/umbraco-cms/fundamentals/data/defining-content
* How to define media and media types: https://docs.umbraco.com/umbraco-cms/fundamentals/data/creating-media 
* How to use data types: https://docs.umbraco.com/umbraco-cms/fundamentals/data/data-types 
* Community tips for best practices: https://www.linkedin.com/advice/3/what-some-best-practices-creating-managing-1f