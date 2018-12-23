---
title: "How to document 'slurs'"
layout: page
---

Semi-circular symbols, which resemble musical slur marks, are written beneath some compound words in the Venetus A manuscript. These marks are recorded in comma separated value tables (files should be .csv and can be edited on github or in simple text editor). The tables for compound word slurs should contain three headings: 

`Slur,Reading,Image` 

Under **Slur** goes the urn reference for the slur itself. This urn reference is composed of the Book Number, a hyphen, and unique identifying sequence.


`urn:cite:hmt:venAslur.Book#_Identifier`

Under **Reading** goes the urn reference for the line of text in the *Iliad* in the Venetus A and the word under which the slur appears.


`urn:cts:greekLit:tlg0012.tlg001.msA:11.[line#]@[word],`

Finally, under **Image**, goes the the urn reference for the image citation of the word and its slur. This is contained within quotation marks(""). This urn reference is obtained via the image citation tool.

Each of these columns is separated by a comma.

An entry typically looks like this:

`Slur,Reading,Image`
`urn:cite:hmt:venAslur.10_1,urn:cts:greekLit:tlg0012.tlg001.msA:10.1@Παναχαιῶν,"urn:cite:hmt:vaimg.VA126RN-0298@0.4825,0.2141,0.1131,0.0173"`
