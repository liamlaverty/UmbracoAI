---
description: 'Add images to blog posts'
targets: ["*"]
---

# Add images to blog posts

* Each blog post should have a hero image.
* Ensure the document type supports a media picker property for this.
* Create a media item for each blog post here image and upload/assign an image of your choice.
  * You can use the unsplash-mcp-server for searching for images.
  * For downloading images, you can normally use curl commands.
  * PNG, JPG image formats are supported.
  * No svg files.
* Adding images to media items in Umbraco requires using the umbraco mcp server's temporary files tool.
  * Although the create-temporary-file says the File parameter must be a 'stream', instead, just pass the path to the file you want to upload and the MCP infrastructure handles reading the file from the filesystem and streaming it to the Umbraco Management API endpoint as a multipart/form-data request.
  * You cannot upload multiple files at once, you must follow the steps to create a media item with a file and do it one by one.
  * DO NOT try manually upload the files, you MUST use the MCP tool to do this.
* Update the blog post template to render the hero image.
* Update the blog list template to show a thumbnail of the hero image.
* DO NOT try to log into the Umbraco backoffice to manually upload images.