---
title: "Identifying Aristarchean Commentary in the Venetus A Scholia"
layout: post
tags: ["va"]

---


A guest post by Thomas Arralde, Class of 2013, College of the Holy Cross

The overarching philosophy behind our work in the Homer Multitext is to be as exact and as comprehensive as possible. Last summer we digitally inventoried every scholion in the entirety of Book 1 of the Venetus A manuscript, and created a diplomatic edition of all the scholia dating to the 10th century. We also make our findings accessible and searchable to facilitate our own research as well as that of others. All people and places referenced in the scholia were tagged with a unique identifier that corresponded to person and place inventories.

In our work on editing the scholia of Book 1 of the Venetus A, we noticed that the word “ὅτι” (because) often began a scholion, and that these scholia often continued “Ζηνόδοτος γράφει” (Zenodotus writes). Our consistent documentation of when Zenodotus, the first publisher an Alexandrian edition of Homer, appeared in the scholia allowed us to observe how frequently his name appeared in the context of these ὅτι scholia. Our comprehensive work on the scholia gave us results that were authoritative for the whole of Book 1, notable for being the book of the Iliad with the greatest number of scholia in the Venetus A, as well as Books 3, 4, and 5. From the statistics we compiled, we were able to form hypotheses about the significance of these scholia, and why they appear so formulaically, which leads us now to the great Homeric scholar Aristarchus.

Aristarchus of Samothrace took over the directorship of the Library of Alexandria in the middle of the 2nd century BC, after the death of his predecessor Aristophanes of Byzantium. The work of Aristarchus is seen as an important turning point in the history of the Homeric tradition, in which the works of Homer become relatively rigid and texts were studied outside the context of performance (Nagy 1996: 110). Because of his pivotal role in the textual history of the Homeric epics, identifying the comments of Aristarchus from what does survive is an important task for Homeric scholars. But doing so is not always a straightforward task, since the scholiast does not always write the name of the scholar whose work he is referring to (Nagy 1997: 117).

One way of identifying scholia attributable to Aristarchus in the Venetus A, we discovered, could be the use of the word ὅτι at the beginning of scholia. As our team was editing the scholia of Book 1, every time a name appeared we placed it in TEI markup, and provided a unique identifier for each name. In our markup, Zenodotus was given the identifier “pers15,” so that his every appearance looked as follows:

    <persName n=“pers15”>Ζηνόδοτος</persName>


Because of this markup, only a simple search was required to find every reference to Zenodotus in our transcriptions. With this information it was an easy task to see in what scholia Zenodotus appeared, and how many of them were ὅτι scholia. We applied the same search to Aristarchus, who appeared in our marked-up scholia as `<persName n=“pers16”>Ἀρίσταρχος</persName>`, which led to an exciting discovery. Aristarchus’ name almost never appears in these scholia, but Zenodotus’ does quite frequently. This and other observations lead to the possibility that these scholia are more or less direct quotations from Aristarchus’ lost works.


Critical signs next to lines of the Iliad on 15V of the Ven. A
Our current understanding of critical signs is that Aristarchus used them both in the scroll of the Iliad text he worked from and in the scroll of his comments to the text so that the two could be easily matched (Bird 2009). With the advent of the codex, the use of critical signs next to both became superfluous and were mostly removed from the scholia but mostly retained next to the text of the Iliad. Evidence of Aristarchus’ usage is the presence of the word “ὅτι” at the beginning of scholia, on its own meaning something like “the sign is here because”. The structure of the scholia in Aristarchus’ notes is supposed to have been sign, lemma, and then the scholion itself.

A rare scholion (from 28R of the Venetus A) that follows the sign-lemma-ὅτι comment sequence that we think Aristarchus’ commentary had

Although the signs that we believe to have been written in Aristarchus’ commentary scroll do not appear in most cases in front of the Venetus A scholia, the word that started the explanation of that sign, ὅτι, often survives as the beginning of the comment. One would expect, then, that when a ὅτι appears there was a critical sign in the scholion that is no longer there, but is retained next to the text. In Book 1 of the Venetus A, however, this does not happen as often as such a rule supposes. In this Book ὅτι begins a scholion which does not have a corresponding critical sign in the main text ~43% of the time. If the critical sign has disappeared in both locations, ought the ὅτι really be translated as “the sign is here because” when no sign exists?

Iliad 1.216, on 16R in the Venetus A, has no Critical sign placed next to it.

Yet the scholion on this line begins with ὅτι
 The absence of critical signs does not continue throughout the Venetus A, however. In Book 3 more than 95% of the scholia that begin with ὅτι are accompanied by a critical sign. What is it about the scholia in Book 1 that causes the scribe to include critical signs with ὅτι scholia 50% less of the time than in Book 3? Is it the great density of scholia that continues through the first book but subsides somewhat in later books that causes the disparity? All of these questions require further investigation, and as we continue to edit more scholia we expect to find further evidence to assist us in our inquiries.

Furthermore, Aristarchus is rarely cited in scholia which begin with ὅτι; his name appears in such scholia only twice in Book 1. This is astounding considering in Book 1 there are 136 ὅτι scholia and 61 occurrences of Aristarchus’ name and little overlap between the two. More frequently citations of Aristarchus appear “thus Aristarchus” or simply “Aristarchus” followed by the comment. What we find instead is that Zenodotus’ name more often follows after ὅτι (30% of the time in Book 1, 28% in Book 3). When Zenodotus appears in the scholia of Book 1, ~85% of the time it is in a ὅτι scholion. If the ὅτι follows Aristarchus’ method of writing his commentary, why is Zenodotus so often cited in these scholia? It could be that the scribe of the Venetus A is quoting directly from Aristarchus (or someone else quoting directly from Aristarchus) in the ὅτι scholia since Aristarchus would not refer to himself in the 3rd person, and would be commenting on the edition of his predecessor, Zenodotus. In fact, there is scarcely ever a mention of any scholar later in date than Aristarchus found in these scholia.

We know that the system of Critical signs used in the Venetus A comes from Aristarchus’ edition of the Iliad. The fact that the ὅτι scholia virtually never name Aristarchus or scholars later than him, and name Zenodotus with an unusual frequency, leads us to believe that they are authentic Aristarchean commentary. Work is ongoing and findings in Book 2 have already yielded tantalizing results. As further evidence comes to light we hope to come closer to answering the critical question of where the information in our scholia comes from.


- Bird G. 2009. “Critical Signs - Drawing Attention to ‘Special’ Lines of Homer’s *Iliad* in the Manuscript Venetus A,” 89–155 in *Recapturing a Homeric Legacy*, ed. C. Dué, Washington DC.
- Nagy G. 1996. *Poetry as Performance*. Cambridge.
- Nagy G. 1997. “Homeric Scholia,” 101–122 in *A New Companion to Homer*, ed. Morris and Powell. Leiden & New York.
