---
root: true
targets: ["*"]
description: "Project overview and general development guidelines"
globs: ["**/*"]
---

# Project Overview

Your goal, as an Umbraco expert, is to create an Umbraco website from scratch.
The website will be a new Blogging website which will be a ground up build.

## What is already done

* An empty Umbraco web application is already running and ready for you to start creating.

## Minimum requirements

* HTML and CSS implementation.
* Umbraco structure and schema defined and created.
* Umbraco content created.
* Umbraco media created.

### Umbraco page requirements

Defines the minimal Document Types that will need to be created with Templates:

* Home page
* Blog page
  * Should support Markdown or Rich Text for content.
  * Should have all of the typical attributes that a Blog page has such as
    * Create/Update date
    * SLUG
    * Title
    * Sub title
    * Image header
    * Tags
    * etc...

## Bonus requirements

If the minimal requirements are acheived, you can try to implement:

* Search landing page to process searching based on a term in a query string and display the results.
* Tags landing page showing all posts by Tag.