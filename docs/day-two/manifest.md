---
title: "Manifest"
---

> http://iiif.io/api/presentation/2.1/#manifest


One of the main concepts for the Presentation API is the Manifest.

A manifest contains enough information to display content to a user. It is a container for lots of different kinds of contextual information. The manifest can give information on how images are related to each other like the order that images should display, the structure of a document like a table of contents, and descriptive information for the resource and individual images.

In one sense it is a performance optimization. Rather than a client having to follow a lot of links to pull in content, a manifest includes the information.

IIIF just specifies the shape a manifest should take to make it easy to work with. Developers will know where to look for particular content and it makes it easier to compare documents or model your own manifest on someone else's.

## IIIF Manifest Example

```json
{
  "@context": "http://iiif.io/api/presentation/2/context.json",
  "@id": "https://purl.stanford.edu/hg676jb4964/iiif/manifest",
  "@type": "sc:Manifest",
  "label": "(center) Martin Luther King Jr. & Joan Baez march to integrate schools,  Grenada, MS, 1966",
  "attribution": "Bob Fitch photography archive, © Stanford University Libraries",
  "logo": {
    "@id": "https://stacks.stanford.edu/image/iiif/wy534zh7137%2FSULAIR_rosette/full/400,/0/default.jpg",
    "service": {
      "@context": "http://iiif.io/api/image/2/context.json",
      "@id": "https://stacks.stanford.edu/image/iiif/wy534zh7137%2FSULAIR_rosette",
      "profile": "http://iiif.io/api/image/2/level2.json"
    }
  },
  "seeAlso": {
    "@id": "https://purl.stanford.edu/hg676jb4964.mods",
    "format": "application/mods+xml"
  },
  "metadata": [
    {
      "label": "Available Online",
      "value": "<a href='https://purl.stanford.edu/hg676jb4964'>https://purl.stanford.edu/hg676jb4964</a>"
    },
    {
      "label": "Title",
      "value": "(center) Martin Luther King Jr. & Joan Baez march to integrate schools,  Grenada, MS, 1966"
    },
    {
      "label": "Contributor",
      "value": "Fitch, Bob (Photographer)"
    },
    {
      "label": "Type",
      "value": "StillImage"
    },
    {
      "label": "Type",
      "value": "photographs"
    },
    {
      "label": "Type",
      "value": "documentary photographs"
    },
    {
      "label": "Date",
      "value": "1966"
    },
    {
      "label": "Format",
      "value": "1 photograph"
    },
    {
      "label": "Format",
      "value": "image/jpeg"
    },
    {
      "label": "Description",
      "value": "Contact sheet for this image is located in Box 52, Folder 1, sheet 796. Negative is located in Box 63, Folder 18, sheet 796."
    },
    {
      "label": "Subject",
      "value": "King, Martin Luther, Jr., 1929-1968"
    },
    {
      "label": "Subject",
      "value": "Baez, Joan"
    },
    {
      "label": "Coverage",
      "value": "Grenada (Miss.)"
    },
    {
      "label": "Identifier",
      "value": "M1994_MLK__0380_796-44"
    },
    {
      "label": "Identifier",
      "value": "M1994"
    },
    {
      "label": "Relation",
      "value": "Bob Fitch photography archive -- Martin Luther King Jr. gallery, 1965-1966"
    },
    {
      "label": "PublishDate",
      "value": "2018-07-25T21:40:28Z"
    }
  ],
  "description": "Contact sheet for this image is located in Box 52, Folder 1, sheet 796. Negative is located in Box 63, Folder 18, sheet 796.",
  "thumbnail": {
    "@id": "https://stacks.stanford.edu/image/iiif/hg676jb4964%2F0380_796-44/full/!400,400/0/default.jpg",
    "@type": "dctypes:Image",
    "format": "image/jpeg",
    "service": {
      "@context": "http://iiif.io/api/image/2/context.json",
      "@id": "https://stacks.stanford.edu/image/iiif/hg676jb4964%2F0380_796-44",
      "profile": "http://iiif.io/api/image/2/level2.json"
    }
  },
  "sequences": [
    {
      "@id": "https://purl.stanford.edu/hg676jb4964#sequence-1",
      "@type": "sc:Sequence",
      "label": "Current order",
      "viewingDirection": "left-to-right",
      "canvases": [
        {
          "@id": "https://purl.stanford.edu/hg676jb4964/iiif/canvas/hg676jb4964_1",
          "@type": "sc:Canvas",
          "label": "Image 1",
          "height": 3820,
          "width": 5426,
          "images": [
            {
              "@id": "https://purl.stanford.edu/hg676jb4964/iiif/annotation/hg676jb4964_1",
              "@type": "oa:Annotation",
              "motivation": "sc:painting",
              "resource": {
                "@id": "https://stacks.stanford.edu/image/iiif/hg676jb4964%2F0380_796-44/full/full/0/default.jpg",
                "@type": "dctypes:Image",
                "format": "image/jpeg",
                "height": 3820,
                "width": 5426,
                "service": {
                  "@context": "http://iiif.io/api/image/2/context.json",
                  "@id": "https://stacks.stanford.edu/image/iiif/hg676jb4964%2F0380_796-44",
                  "profile": "http://iiif.io/api/image/2/level2.json"
                }
              },
              "on": "https://purl.stanford.edu/hg676jb4964/iiif/canvas/hg676jb4964_1"
            }
          ]
        }
      ]
    }
  ]
}
```

Adapted from [jronallo/iiif-workshop](https://raw.githubusercontent.com/jronallo/iiif-workshop-new/master/content/presentation-api/manifest/_index.md)
