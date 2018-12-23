---
title:  Creating images of bifolio spreads with the GIMP
layout: page
---

## The problem ##


In the generic Digital Scholarly Editions model,  citable passages of texts are indexed to citable regions of an image.  Manuscripts are generally photographed one page at a time.  For manuscripts where the layout is designed to be right across an open pair of pages (a bifolio spread) rather than one page at time, we need to index texts to an image showing the entire bifolio spread, however.  In this case, we will create a composite image juxtaposing the verso of one folio with the recto of the following folio.   These notes will show you how to do that using the GIMP, a freely available image processing program.

## Prerequisites ##

- install [GIMP](http://www.gimp.org/)
- a pair of images you want to paste together

## Process ##

3. Open GIMP
4. Select "File" then "New"
5. Set generous dimensions.  For HMT composites, we generally can use a width of 10000 pixels and a height of 7000 pixels.  Ignore the warning about the size being too big.
6. Open the verso image, either in GIMP or another image viewer, and copy the entire image.
7. In the new GIMP you created, select "Edit", "Paste As", and then "New Layer".
8. Repeat these steps for the recto image.
9. Using the rectangle drawing tool, select portions of the image you want to remove and cut them out (Command + X). You'll want to take from the center to match up the gutters as closely as you can. If both verso and recto images have color scales, save at least one of them, ideally both. Avoid cutting from the top and bottom until you have the two images aligned.
10. Using the move tool, align the images along the gutter of the bifolio. 
11. When you have the aligned the two layers, merge them into one: Under the 'Image' menu select 'Merge Visible Layers.' The default settings are acceptable. 
12. When you have merged the visible layers, using the rectangle tool again select the portion of the image that you want to keep. Now is the time to cut off any excess on the outside edges, but remember to keep at least one color scale. 
13. Copy this selection (Command + C).
14. Go the 'File' menu. Select 'Create' and then 'From Clipboard'.

## Saving ##

1. Select “File” and “Save As”, and choose a place to save it where you will have easy access (desktop, a folder, etc.)
Name the file using the pattern: manuscript - verso number v- recto number r (e.g., `gen49-10v-11r.xcf`). This should create an `.xcf`  file (GIMP's native format).
1. In that same file, go to "File", "Export" then select the location where the .xcf was saved, click "Export" in the saving window, and then click "Export" a final time in the new window which pops up. This should create a `.png` file with the same name.
