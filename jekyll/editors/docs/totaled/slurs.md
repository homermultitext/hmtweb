---
title: "How to document 'slurs'"
layout: page
---


## ὑφ᾽ ἕν

You may see arced lines, which resemble musical slur marks, written beneath  compound words in some manuscripts.  This mark indicates that the two parts should be read as one unit.  This form of reading, and the mark that aids you to recognize it, was called ὑφ᾽ ἕν (hence the English word *hyphen*).  This example, from *Iliad* 21.15 in the Venetus A manuscript, illiustrates the practice:



[![](http://www.homermultitext.org/iipsrv?OBJ=IIP,1.0&FIF=/project/homer/pyramidal/deepzoom/hmt/vaimg/2017a/VA270RN_0440.tif&RGN=0.408,0.4632,0.158,0.0225&wID=5000&CVT=JPEG)](http://www.homermultitext.org/ict2/?urn=urn:cite2:hmt:vaimg.2017a:VA270RN_0440@0.408,0.4632,0.158,0.0225)



## Recording "slurs"

As with every other mark on the page of a manuscript, we record these as part of our editorial process.

Your repository may include a directory names `hyphens` where you can put files with tables recording three columns of data:  a URN for the hyphen mark, a URN for the text it marks, and a URN with an illustrative image.


### URN for hyphen

To create a URN for the mark, you will be adding to one of the following collections:

- Venetus A manuscript:  `urn:cite2:hmt:msAslur.v1:`
- Venetus B manuscript:  `urn:cite2:hmt:msBslur.v1:`
- Upsilon 1.1 manuscript:  `urn:cite2:hmt:e3slur.v1:`

The identifier for the individual slur should be formed from the page ID and a running count of "slurs" on that page, separated by a comma.  The example above is the first slur on folio 270r of the Venetus A, so its full URN is `urn:cite2:hmt:venAslur.v1:270r_1`.


### URN for text

The CTS URN for the text where the slur appears should include a subreference for the word the slur marks.   The full URN for the text passage illustrated above would therefore look like this:


    urn:cts:greekLit:tlg0012.tlg001.msA.hmt:21.15@βαθυδινήεντος

### URN for image

The record should be completed by citing visual evidence. As in the example above, your image citation should illustrate the entire word as well as the slur mark beneath it.

### Complete record

The complete record for the example illustrated above would look like this:


    Slur#Reading#Image
    urn:cite2:hmt:venAslur.v1:270r_1#urn:cts:greekLit:tlg0012.tlg001.msA.hmt:21.15@βαθυδινήεντος#urn:cite2:hmt:vaimg.2017a:VA270RN_0440@0.408,0.4632,0.158,0.0225
