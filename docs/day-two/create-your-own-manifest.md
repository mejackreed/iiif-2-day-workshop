---
title: "Create Your Own Manifest"
---

## Building your own manifest

To start navigate to:

https://iiif.bodleian.ox.ac.uk/manifest-editor/

This is a demo/hosted version of the [iiif-manifest-editor](https://github.com/bodleian/iiif-manifest-editor).

1. Click "New Manifest"
1. Click "Add Canvas" and then click on the "Empty Canvas"

    ![add canvas](/img/add_canvas.png)

1. Now we need to add an image to this canvas. Click "Add Image to Canvas"
1. And we want to use an image we already hosting, so we select the "From info.json URI" option, and input our info.json URI from our local IIIF server. Then click "Submit URI"

    `http://127.0.0.1:8182/iiif/2/eddie.jpg/info.json`

    ![info json uri](/img/info_json_uri.png)

1. We should now have an image in our view!
1. Finally, let's download the manifest, by clicking "Save Manifest" at the top of the page, and "Save"

  Great job! You now have created and downloaded a IIIF Presentation API manifest.
