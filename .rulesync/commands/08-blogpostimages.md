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
  * Save images to src/MyProject/wwwroot/media/downloaded_images
  * PNG, JPG image formats are supported.
  * No svg files.
* Adding images to media items in Umbraco normally requires using the umbraco mcp server's temporary files tool... DO NOT USE THIS it is broken right now.
  * Create media items for all the images, use the files from src/MyProject/wwwroot/media/downloaded_images folder and all subdirectories. Use the files directly instead of creating temporary files. Umbraco has access to these files so use the relative path for the umbracoFile property.
* Update the blog post template to render the hero image.
* Update the blog list template to show a thumbnail of the hero image.
* DO NOT try to log into the Umbraco backoffice to manually upload images.