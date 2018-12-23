---
title: Editing the Scholia
layout: page
---


1. Useful items to have open:
  - Erbse (if you also have the print edition, this is useful because it is the only place his apparatus criticus is preserved)
  - Dindorf (available [here](http://www.homermultitext.org/resources.html) Volume 1 contains books 1-12, Volume 2 contains books 13-24 and also contains an appendix with the interlinear scholia)
  - [personal name authority list](https://github.com/homermultitext/hmt-authlists/blob/master/data/hmtnames.csv)
  - [place name authority list](https://github.com/homermultitext/hmt-authlists/blob/master/data/hmtplaces.csv)
  - an edition of the *Iliad*
  - authority lists for CTS `greekLit` namespace: 
      - [works](https://github.com/chs-tg/greekLit/blob/master/collections/greekLit-works.csv)
      - [text groups](https://github.com/chs-tg/greekLit/blob/master/collections/greekLit-groups.csv)
  - a Greek dictionary or parser
  - [Editors' Guide](http://homermultitext.github.io/hmt-editors-guide/)
  
2. Open the XML edition for your scholia document (main, interior, exterior, intermargial, interlinear). 

  Each scholion is composed of the basic element 'div' for division. Each scholion has its own 'div' within the XML document. These 'div's get attributes @n, which corresponds to the TextURN for that scholion which you generated when you indexed the scholia, and @type which is always 'scholion'.

  Each scholion is further composed of three 'div's within the main 'div'. The first 'div' is for the lemma, the short string of text that links the scholion to the main text in the Venetus A. This 'div' naturally gets the @type attribute, which is always 'lemma'. Within this 'div' is the element 'p' for paragraph. This element can contain any text. This is where you will put the text of the lemma.

  The second 'div' gets the @type attribute, which is always 'reference'. The second 'div' also contains the 'p' element and in this element you will put the full text URN for the *Iliad* passage on which the scholion comments. Remember that it is commenting on a specific manuscript, so the text URN should be version specific.

  The third 'div' gets the @type attribute, which is always 'comment'. The third 'div' contains the 'p' element and within this element, you record the contents of the scholion.

3. Locate the base text for the scholion in Erbse. It is recommended that you copy and paste this into a simple text editor (like Text Edit or Notepad++, Microsoft Word or the like is not advised) where you can do a diplomatic edition and then copy and paste into your XML editor. Some XML editors are obnoxious when you attempt to type Greek.

4. Follow the standards laid out in the [Editors' Guide](http://homermultitext.github.io/hmt-editors-guide/). You should be marking up things like:
  - personal, place, and ethnic names
  - quotations, cited quotations, and quoted strings
  - abbreviations
  - scribal corrections
  - damage resulting in missing text
 
*This list is not exhaustive. Reference your Editors' Guide!*  

## Special Characters You May Need ##

- End of scholion mark: ⁑
- cross: ‡

## Proposing New Personal and Place Names, or Additions or the Entries ##

Be sure to try all variations in spellings. If you find a variation in spelling is missing from the descriptor, use the issue tracker to propose changes. You can also use the issue tracker to propose additional personal and place names not on the list. When you do this, you must include the following:

- the name, and variant spellings
- a clear description of who the person is, especially if there is more than one person by that name
- the full text URN for where the name appears

## Other Tips ##

When doing the XML editing, you may need to go into the special characters menu for things like combining diareses, macrons, breves, etc.


