---
title: "Serve Your Manifest"
---

## Serve your manifest

### Method 1: Use myjson

1. Click "Settings" button

    ![](/img/dig-bod-settings.jpg)

1. Click "click here to use myjson.com"

    ![](/img/dig-bod-click-here.jpg)

1. Save settings and close
1. Click "Save Manifest"
1. Select "Store manifest remotely"
1. Click "Store manifest on Server"
1. Copy myjson link. This is the manifest url.

    ![](/img/dig-bod-manifest-url.jpg)

> If you make any changes to your manifest in the editor, you can use the "Update Manifest on Server" button to persist the changes.

### Method 2: Serve your Manifest Locally

* Serving manifest locally
  * Install http-server, `npm install -g http-server`, or live-server, `npm install -g live-server`
  * Then in the directory with the manifest, run `http-server --cors` or `live-server --cors`

### Method 3: Serve Your Manifest with GitHub gist

1. Navigate to https://gist.github.com

1. Drag and drop your `manifest.json` file into the window and click "Create Secret Gist" (or public if you like, it doesn't matter).

    ![gist](/img/gist.png)

1. After the gist is created, click the "Raw" button to get the raw file url.
