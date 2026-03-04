# image-annotate-template

image-annotate-template is a simple website template for creating a presentation with annotated images.
It uses Jekyll static site generation, Bootstrap 5, and the Annotorious JS library.

## Get Started

- Set up your website:
    - Create a copy of the template.
    - Add your images to the "objects" folder.
    - Activate GitHub Pages to create your live site.
    - For more detailed instructions see "docs/create-website.md"
- Annotate images:
    - Visit Annotate page.
    - Select image and use the interface to create/edit annotations.
    - Download annotation data as JSON.
    - Add the annotation JSON file to project repository "objects" folder.
- Publish annotated images:
    - Create or edit a content page (see "docs/create-website.md" for details).
    - Add `annotation-viewer: true` to the front matter.
    - Use the "annotated-image.html" include to add annotated images to the page. Check the comments in the include for all supported options.

## Guidelines

- Supported image types include JPG and PNG. Ensure your file extensions are lowercase, `.jpg`, `.jpeg`, or `.png` only.
- For ease of use, create meaningful filenames without spaces.
- You can set the default annotation styles (fill, opacity, stroke color, stroke width) in "_config.yml" or as front matter on each page.
- If you have issues with the "Annotate Image" page caching old versions of your annotations, open the page in a new browser window.
- Unpublish the "Annotate Image" page when you are done annotating images and don't want it to display publicly by removing the `nav:` option from the front matter (or just deleting "pages/annotate.html").
