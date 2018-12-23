---
title: Systematic paleographic observations
layout: page
---


## Background

We take a sample of paleographic observations whenever we  begin editing a new manuscript page.   To sample the paleography of the main hand in the *Iliad* text, you will record observations for the first line of *Iliad* text.   To sample the paleography of the scholia in the Venetus A, we take the first 40 *glyphs* in the main scholia.  If there are more than forty glyphs in the first scholion you should stop at forty. If there are fewer, you should move on to a second scholion until you reach forty. 

Your goal is to identify every glyph in the sample:  individual character, or multi-character abbreviation or ligature.
You should ignore punctuation. Ligatures such as epsilon-iota should be treated as a single glyph. If your glyph has any diacritical marks (accents or breathings), include those in your citation of both the image and the text  (see below). 


## Process ##

Record your observations in the file `paleography.csv`, located in the `collections` folder of your team's editing repository.   You will record each observation on a separate line, in four columns labelled Observation, TextUrn, Image, and Comments.



**Observation**: This column contains a URN we will use to identify this record of this observation. It will look something like this:

    urn:cite:op:YOURTEAMID.X

  The two variables are `YOURTEAMID` and `X`.  The HMT project will assign your team a unique identifier that could be something like `2015office3`.  `X` is a value you will choose to identify this observation uniquely among all the observations your team makes.  It will probably be easiest to start with 1 and go up sequentially, but remember that they are not numbers, they are names.

**TextUrn**: This column contains a CTS URN citing the passage of text you are recording.   In addition to giving the canonically citable line of the *Iliad*, you want to include a *subreference* (following the `@` symbol) identifying substring you observed, most often a single character.  For example if you are citing the first alpha in the Venetus A *Iliad* 18.1, the URN could look like this:

    urn:cts:greekLit:tlg0012.tlg001.msA:18.1@α
  
Repeated sequences of characters must include a further index in square brackets showing the number of times the letter has appeared in that particular text passage.   While the first occurence needs no brackets and number, the second alpha in the Venetus A *Iliad* 18.1 would be cited as followed:

    urn:cts:greekLit:tlg0012.tlg001.msA:18.1@α[2] 
  

Remember that you are indexing the entire character sequence you record.  For example, a two-character sequence of an alpha with a rough breathing would be different from an alpha with a smooth breathing, or an alpha with no accent.

  Remember that the text URN will change for the scholia. It might look something like this:

    urn:cts:greekLit:tlg5026.msA.hmt:18.1@α 


  
**Image**: This column cites a rectangular region on an image.  From the HMT [manuscript browser](http://www.homermultitext.org/hmt-digital/home), you can use the Image Citation Tool to find this citation. If your glyph has any diacritical marks (accents or breathings), include those in the image. Remember that a ligature counts as one glyph. A good rule of thumb is that if you can't get two characters distinctly in a single image, you should index them together.

**Notes**: This column is for any extra notes you may want to make, such as there being a ligature. You do not have to include notes if there is nothing to report. 



