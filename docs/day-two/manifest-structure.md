---
title: "Manifest Structure"
---

To explain a manifest we'll start at the innermost part of the manifest and work our way out.

## Content

The content we have is an image. In our case we'll also have an image server service for that image. Just having an image though doesn't allow for things like a scholar to apply annotations to the image.

![](/img/presentation-chart-content.png)

## Canvas

The next layer up and out we have our shared canvas that can have our image content painted onto it.

![](/img/presentation-chart-canvas.png)

## Sequence

Many resources are made of more than one image, so a sequence is used to group and order canvases.

![](/img/presentation-chart-sequence.png)

## Manifest

The manifest contains the information needed to display (e.i. present) the resource to users. The manifest wraps up the sequence(s) that encapsulate the canvases that have the image content painted on. The manifest includes other properties, but it is the sequences property that encapsulates the image content.

![](/img/presentation-chart-manifest.png)

## Collection

Another level up it is possible to group manifests into collections.

![](/img/presentation-chart-collection.png)

## Fuller Picture

The above images are all you'll need for this workshop. The fuller picture is a bit more complicated. There are other types within IIIF that you ought to at least know their names exist.

We'll skip over ranges, layers, and annotation lists for now, but will point out that rather than applying content directly to the canvas we usually will be using an annotation to place the image content on the canvas.

![](/img/presentation-chart-complicated.png)

Adapted from [jronallo/iiif-workshop](https://raw.githubusercontent.com/jronallo/iiif-workshop-new/master/content/presentation-api/manifest/manifest-structure.md)
