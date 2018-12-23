---
title:  Creating a Navigational Line Index
layout: page
---

Indexing *Iliad* lines to their corresponding folios is incredibly important. When this work is completed we will be able to search for *Iliad* lines and get their corresponding images. 

This work will be done in a two-columned table called 'LineRangestoFolio.csv' located in the 'collections' folder. This file contains two columns:

1. TextRangeURN: a cts URN for the range of lines
2. FolioURN: an object URN for the folio as a concept (not the image!)

## Text Range URNS ##

Line range URNs will look like this:

    urn:cts:greekLit:tlg0012.tlg001.msA:1.1-1.9
    
This is a canonical text service (CTS) URN, meaning it is a very specific way of refering to a text. The parts of the URN can be broken down as follows:

**urn** means it is a uniform reference name (all URNS start with this)

**urn:cts** means it is a canonical text service (CTS) URN, meaning we are refering to a text not an object

**urn:cts:greekLit** this URN refers to a work of Greek Literature

**urn:cts:greekLit:tlg0012** this URN refers to a work of Homer

**urn:cts:greekLit:tlg0012.tlg001** this URN refers to Homer's *Iliad*

**urn:cts:greekLit:tlg0012.tlg001.msA** this URN refers to Homer's *Iliad* as found in the Venetus A MS

**urn:cts:greekLit:tlg0012.tlg001.msA:1.1-1.9** this refers to Book 1, lines 1-9 of the *Iliad* found in the Venetus A MS

It is important to write your line ranges explicitly. 1.1-9 is not valid in URN format. You MUST write 1.1-1.9!

## Folio URNs ##

Folio URNs refer to a folio as an entity or a concept. They do not refer to a specific image of a folio. They can be broken down as follows:

**urn* means it is a uniform reference name (all URNS start with this)

**urn:cite** means it is an object URN

**urn:cite:hmt** means it is refering to an object in the HMT data set

**urn:cite:hmt.msA** means it is refering to an object in the Venetus A MS

**urn:cite:hmt:msA.12r** means it is refering to folio 12 recto in the Venetus A MS as an object

## Work Flow ##

1. count the *Iliad* lines on a folio
2. verify that the first and last lines correspond to the number that you counted
3. IF they do correspond, enter that as your line range. IF they don't correspond, figure out why. If there is a line missing or duplicated you do not need to alter your line range, but you should make a note of the folio in your project wiki. For example, if line 8 was missing on the first folio, the range would still be 1.1-1.9.
