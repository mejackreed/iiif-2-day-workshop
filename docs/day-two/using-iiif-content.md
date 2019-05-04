---
title: Using IIIF Content
---

Many organizations publish IIIF content on the web. There are an estimated 1 billion images now published using IIIF. How do I get access to this content and start using it?


## Drag and drop

Some organizations provide a "drag and drop" link which can be used to access the image in a IIIF viewer.

1. If you see a IIIF logo with a link, it may be dragged and dropped. Stanford's digital collections site has this enabled. [https://exhibits.stanford.edu/fitch/browse/martin-luther-king-jr-1965-1966?view=list](https://exhibits.stanford.edu/fitch/browse/martin-luther-king-jr-1965-1966?view=list)

    ![](/img/iiif-dnd.jpg)

1. Drag this logo/link into a IIIF viewer.

    ![](/img/iiif-dnd.gif)


> The link that you are dragging and dropping will have the manifest URL as a parameter `manifest`. You can always inspect and use that manifest URL. https://library.stanford.edu/projects/international-image-interoperability-framework/viewers?manifest=https://purl.stanford.edu/tn799ny4732/iiif/manifest -> https://purl.stanford.edu/tn799ny4732/iiif/manifest

Some example sites that use the drag and drop pattern.

 - [Stanford's digital exhibits site](https://exhibits.stanford.edu)
 - [Digital Bodleian Library](https://digital.bodleian.ox.ac.uk)

## Internet Archive

Any images uploaded to the [Internet Archive](https://archive.org) already are served using IIIF.

You can access the IIIF version of the resource by modifying the URL.

```txt
https://archive.org/details/mma_view_of_beirut_438634

# Becomes

https://iiif.archivelab.org/iiif/mma_view_of_beirut_438634

# Information Response

https://iiif.archivelab.org/iiif/mma_view_of_beirut_438634/info.json
```
