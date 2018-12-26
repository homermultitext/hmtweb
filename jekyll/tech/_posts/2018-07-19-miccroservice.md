---
layout: post
title: The Homer Multitext Microservice
tags: [news, update]
---


The Homer Multitext produces integrated data on Greek Epic poetry, its language, its evolution over time, the traditions of scholarship surrounding it, and the physical artifacts, manuscripts and papyri, that are our only evidence. For a concise explanation of what the HMT publishes, please see [http://www.homermultitext.org/digital/overview](http://www.homermultitext.org/digital/overview).

At the same time, we Project Architects of the HMT, Neel Smith and Christopher Blackwell, are interested in making this data as widely accessible as possible. The data is released in [CEX Format](https://cite-architecture.org/citedx/CEX-spec-3.0.1/), a plain-text serialization of [data organized according to defined abstract data models](http://cite-architecture.org/about/). We have developed [code libraries in Scala](https://github.com/cite-architecture) implementing these abstract data models. These libraries provide the greatest flexibility in manipulating, locating, aggregating, and transforming the data of the Homer Mulititext.

For users who may not want to write code directly, we have provided [an online application offering a graphical user interface](http://www.homermultitext.org/hmt-digital/) for interacting with HMT data using the Cite Architecture’s Scala libraries.

For those who might want to write their own applications that interact with the HMT data, we provide a collection of microservices.

The examples below demonstrate the Scala Cite Services (Akka) application, SCS-Akka, running at beta.hpcc.uh.edu/scs/, and (as of July 19, 2018) serving data from the [2018g Release of the Homer Multitext Data](https://github.com/homermultitext/hmt-archive).

The service accepts requests via HTTP, and returns JSON expressions of CITE objects. We have published [a library in Scala for de-marshalling those JSON expressions into CITE data objects](https://github.com/cite-architecture/CITE-JSON).

The [CiteApp web-based application for the Homer Multitext](http://www.homermultitext.org/hmt-digital/) gets its data from this service, and indeed the web-application and the microservice were developed jointly.

This collection of microservices is serving current data from the Homer Multitext, edited by Casey Dué and Mary Ebbott, a project of the [Center for Hellenic Studies of Harvard University](http://www.chs.harvard.edu/).

For more information on this service, please see <https://github.com/cite-architecture/scs-akka>.

For information on the CITE Architecture, please see <https://cite-architecture.org>.

Report bugs by filing issues on GitHub.

### Texts

#### About the Service’s Catalog

- <http://beta.hpcc.uh.edu/scs/libraryinfo>


#### See the Text Catalog


-  <http://beta.hpcc.uh.edu/scs/texts>
-  <http://beta.hpcc.uh.edu/scs/textcatalog>
-  <http://beta.hpcc.uh.edu/scs/textcatalog/urn:cts:greekLit:tlg0012.tlg001:>


#### Get the First Valid Reference in a text
-  <http://beta.hpcc.uh.edu/scs/texts/firsturn/urn:cts:greekLit:tlg0012.tlg001.msA:>

#### Get Valid References

All references for a version of a text:

-  <http://beta.hpcc.uh.edu/scs/texts/reff/urn:cts:greekLit:tlg0012.tlg001.msA:>


Valid references for parts of a text:

-  <http://beta.hpcc.uh.edu/scs/texts/reff/urn:cts:greekLit:tlg0012.tlg001.msA:2>
-  <http://beta.hpcc.uh.edu/scs/texts/reff/urn:cts:greekLit:tlg0012.tlg001.msA:2-3>
-  <http://beta.hpcc.uh.edu/scs/texts/reff/urn:cts:greekLit:tlg0012.tlg001:1>


#### Get Passages

Passages for a specific version of a text:

-  <http://beta.hpcc.uh.edu/scs/texts/urn:cts:greekLit:tlg0012.tlg001.msA:1.1>
-  <http://beta.hpcc.uh.edu/scs/texts/urn:cts:greekLit:tlg0012.tlg001.msA:1.1-1.25>
http://beta.hpcc.uh.edu/scs/texts/urn:cts:greekLit:tlg0012.tlg001.msA:2
-  <http://beta.hpcc.uh.edu/scs/texts/urn:cts:greekLit:tlg0012.tlg001.msA:2-3>
-  <http://beta.hpcc.uh.edu/scs/texts/urn:cts:greekLit:tlg0012.tlg001.msA:1.600-2>


Passages for all versions of a text:

-  <http://beta.hpcc.uh.edu/scs/texts/urn:cts:greekLit:tlg0012.tlg001:1.1>
-  <http://beta.hpcc.uh.edu/scs/texts/urn:cts:greekLit:tlg0012.tlg001:2.1-2.5>


####  NGrams

NGrams in works present in the library:

-  <http://beta.hpcc.uh.edu/scs/texts/ngram/urn:cts:greekLit:tlg5026.msA.va_dipl:?n=3> (3-grams in the Venetus A Main Scholia)
-  <http://beta.hpcc.uh.edu/scs/texts/ngram/urn:cts:greekLit:tlg5026.msA.va_dipl:?n=3&t=20> ( occuring more than t times)
-  <http://beta.hpcc.uh.edu/scs/texts/ngram/urn:cts:greekLit:tlg5026.msA.va_dipl:?n=3&s=Ζηνόδοτος> (Filter for string, s=Ζηνόδοτος.)

Find citations to NGrams:

-  <http://beta.hpcc.uh.edu/scs/texts/ngram/urns?ng=ὅτι+Ζηνόδοτος+γράφει> (find URNs for a given N-gram in the entire library)
-  <http://beta.hpcc.uh.edu/scs/texts/ngram/urns/urn:cts:greekLit:tlg0012.tlg001.msA:?ng=προσέφη+πόδας+ὠκὺς> (find URNs for a given N-gram in one text)

Returning a Corpus of Passages containing an NGram:

-  <http://beta.hpcc.uh.edu/scs/texts/ngram/urns/tocorpus?ng=ὅτι+Ζηνόδοτος+γράφει> (find URNs for a given N-gram in the entire library)
-  <http://beta.hpcc.uh.edu/scs/texts/ngram/urns/tocorpus/urn:cts:greekLit:tlg0012.tlg001.msA:?ng=προσέφη+πόδας+ὠκὺς> (find URNs for a given N-gram in one text)

#### String Searches

-  <http://beta.hpcc.uh.edu/scs/texts/find?s=ἄναξ+ἀνδρῶν+Ἀγαμέμνωνl>
-  <http://beta.hpcc.uh.edu/scs/texts/find?s=γράφει>
-  <http://beta.hpcc.uh.edu/scs/texts/find?s=ὅτι&s=γράφει>
-  <http://beta.hpcc.uh.edu/scs/texts/find/urn:cts:greekLit:tlg0012.tlg001.msA:?s=Ἀγα>

#### Token Searches
-  <http://beta.hpcc.uh.edu/scs/texts/token?t=Ἀγαμέμνων>
-  <http://beta.hpcc.uh.edu/scs/texts/token/urn:cts:greekLit:tlg0012.tlg001.msA:?t=Ἀγαμέμνων>
-  <http://beta.hpcc.uh.edu/scs/texts/tokens?t=πόδας&t=ὠκὺς>
-  <http://beta.hpcc.uh.edu/scs/texts/tokens/urn:cts:greekLit:tlg0012.tlg001.msA:?t=πόδας&t=ὠκὺς>
-  <http://beta.hpcc.uh.edu/scs/texts/tokens?dist=3&t=ὅτι&t=γράφει> (Two tokens within dist=3 of each other)
-  <http://beta.hpcc.uh.edu/scs/texts/tokens?dist=3&t=ὅτι&t=γράφει> (Two tokens within dist=2 of each other, should return no passages)


### Collections of Objects


####  Catalog

-  <http://beta.hpcc.uh.edu/scs/collections/> (all collections)
-  <http://beta.hpcc.uh.edu/scs/collections/urn:cite2:hmt:msA.v1:> (filter by URN)
-  <http://beta.hpcc.uh.edu/scs/collections/reff/urn:cite2:hmt:msA.v1:> (filter by URN, just URNs)
-  <http://beta.hpcc.uh.edu/scs/collections/hasobject/urn:cite2:hmt:msA.v1:1r> (check for an object; should return true)
-  <http://beta.hpcc.uh.edu/scs/collections/hasobject/urn:cite2:hmt:msA.v1:NOTOBJECT> (check for an object; should return false)
-  <http://beta.hpcc.uh.edu/collections/labelmap> (returns a map of Cite2Urn -> String, the label of each citable object)


#### Objects

-  <http://beta.hpcc.uh.edu/scs/objects/urn:cite2:hmt:msA.v1:> (all objects for version v1 of collection urn:cite2:hmt:msA:)
-  <http://beta.hpcc.uh.edu/scs/objects/prevurn/urn:cite2:hmt:msA.v1:2v> (get the URN of the previous object in an ordered collection)
-  <http://beta.hpcc.uh.edu/scs/objects/nexturn/urn:cite2:hmt:msA.v1:1r> (get the URN of the next object in an ordered collection)
-  <http://beta.hpcc.uh.edu/scs/objects/urn:cite2:hmt:msA.v1:12r-13v> (a range of objects in an ordered versioned collection)
-  <http://beta.hpcc.uh.edu/scs/objects/urn:cite2:hmt:msA.v1:12r-13v?dse=true> (a range of objects in an ordered versioned collection, with all DSE records associated with those objects and properties of those objects [see below])
-  <http://beta.hpcc.uh.edu/scs/objects/paged/urn:cite2:hmt:msA.v1:?offset=1&limit=10> (paged viewing of objects in an ordered collection)
-  <http://beta.hpcc.uh.edu/scs/objects/paged/urn:cite2:hmt:msA.v1:?offset=11&limit=10> (paged viewing of objects in an ordered collection)
-  <http://beta.hpcc.uh.edu/scs/objects/paged/urn:cite2:hmt:msA.v1:> (paged viewing, with default values, offset=1, limit=10, of objects in an ordered collection)

Get objects from multiple collections:

-  <http://beta.hpcc.uh.edu/scs/collections/objects?urn:cite2:cite:datamodels.v1:&urn=urn:cite2:hmt:msA.v1:&urn=urn:cite2:hmt:compimg.v1:>


####  Finding Objects

urn-match

-  <http://beta.hpcc.uh.edu/scs/objects/find/urnmatch?find=urn:cite2:hmt:msA.v1:12r> (search all property-values for a URN)
-  <http://beta.hpcc.uh.edu/scs/objects/find/urnmatch?find=urn:cite2:hmt:msA.v1:12r&dse=true> (search all property-values for a URN, with DSE records for the returned objecs.)
-  <http://beta.hpcc.uh.edu/scs/objects/find/urnmatch?find=urn:cite2:hmt:msA.v1:12r&offset=0&limit=3> (search all property-values for a URN; offset=0 start at the first result; limit=3 return only three results; these optional parameters apply to all searching requests and allow paged access to results)
-  <http://beta.hpcc.uh.edu/scs/objects/find/urnmatch/urn:cite2:hmt:va_dse.v1:?find=urn:cite2:hmt:msA.v1:12r> (limit to a specified collection)
-  <http://beta.hpcc.uh.edu/scs/objects/find/urnmatch/urn:cite2:hmt:va_dse.v1:?find=urn:cite2:hmt:msA.v1:12r&parameterurn=urn:cite2:hmt:va_dse.v1.surface:> (limit to a specified collection and a specified property)

regexmatch

-  <http://beta.hpcc.uh.edu/scs/objects/find/regexmatch?find=[0-9]{2}> (use regular expressions to search property values)
-  <http://beta.hpcc.uh.edu/scs/objects/find/regexmatch/urn:cite2:hmt:compimg.v1:?find=[0-9]{2}> (use regular expressions to search property values)

stringcontains

-  <http://beta.hpcc.uh.edu/scs/objects/find/stringcontains?find=folio+320>
-  <http://beta.hpcc.uh.edu/scs/objects/find/stringcontains/urn:cite2:hmt:vaimg.2017a:?find=folio+321>

valueequals

-  <http://beta.hpcc.uh.edu/scs/objects/find/valueequals?propertyurn=urn:cite2:hmt:msA.v1.rv:&value=recto>
-  <http://beta.hpcc.uh.edu/scs/objects/find/valueequals?propertyurn=urn:cite2:hmt:msA.v1.rv:&value=verso>

-  <http://beta.hpcc.uh.edu/scs/objects/find/valueequals?propertyurn=urn:cite2:hmt:msA.v1.sequence:&value=3>
-  <http://beta.hpcc.uh.edu/scs/objects/find/valueequals?propertyurn=urn:cite2:hmt:msA.v1.image:&value=urn:cite2:hmt:vaimg.2017a:VA002RN_0003>

numeric less-than

-  <http://beta.hpcc.uh.edu/scs/objects/find/numeric?n1=5&op=lt>
-  <http://beta.hpcc.uh.edu/scs/objects/find/numeric?n1=5&op=lt&propertyurn=urn:cite2:hmt:msA.v1.sequence:>
-  <http://beta.hpcc.uh.edu/scs/objects/find/numeric/urn:cite2:hmt:msA.v1:?n1=5&op=lt>

numeric less-than-or-equal

-  <http://beta.hpcc.uh.edu/scs/objects/find/numeric?n1=5&op=lteq>
-  <http://beta.hpcc.uh.edu/scs/objects/find/numeric?n1=5&op=lteq&propertyurn=urn:cite2:hmt:msA.v1.sequence:>
-  <http://beta.hpcc.uh.edu/scs/objects/find/numeric/urn:cite2:hmt:msA.v1:?n1=5&op=lteq>


numeric equals

-  <http://beta.hpcc.uh.edu/scs/objects/find/numeric?n1=5&op=eq>
-  <http://beta.hpcc.uh.edu/scs/objects/find/numeric?n1=5&op=eq&propertyurn=urn:cite2:hmt:msA.v1.sequence:>
-  <http://beta.hpcc.uh.edu/scs/objects/find/numeric/urn:cite2:hmt:msA.v1:?n1=5&op=eq>

numeric greater-than

-  <http://beta.hpcc.uh.edu/scs/objects/find/numeric?n1=5&op=gt>
-  <http://beta.hpcc.uh.edu/scs/objects/find/numeric?n1=5&op=gt&propertyurn=urn:cite2:hmt:msA.v1.sequence:>
-  <http://beta.hpcc.uh.edu/scs/objects/find/numeric/urn:cite2:hmt:msA.v1:?n1=5&op=gt>

numeric greater-than-or-equal

-  <http://beta.hpcc.uh.edu/scs/objects/find/numeric?n1=5&op=gteq>
-  <http://beta.hpcc.uh.edu/scs/objects/find/numeric?n1=5&op=gteq&propertyurn=urn:cite2:hmt:msA.v1.sequence:>
-  <http://beta.hpcc.uh.edu/scs/objects/find/numeric/urn:cite2:hmt:msA.v1:?n1=5&op=gteq>

numeric within

-  <http://beta.hpcc.uh.edu/scs/objects/find/numeric?n1=4&op=within&n2=6>
-  <http://beta.hpcc.uh.edu/scs/objects/find/numeric?n1=4&op=within&n2=6&propertyurn=urn:cite2:hmt:msA.v1.sequence::>
-  <http://beta.hpcc.uh.edu/scs/objects/find/numeric/urn:cite2:hmt:msA.v1:?n1=4&op=within&n2=6>


### Data Models
-  <http://beta.hpcc.uh.edu/scs/datamodels>
-  <http://beta.hpcc.uh.edu/scs/collectionsformodel/urn:cite2:cite:datamodels.v1:imagemodel>
-  <http://beta.hpcc.uh.edu/scs/modelsforcollection/urn:cite2:hmt:vaimg.2017a:>
-  <http://beta.hpcc.uh.edu/scs/modelapplies?modelurn=urn:cite2:cite:datamodels.v1:binaryimg&collurn=urn:cite2:hmt:binaryimg.v1:>


### Images

Basic Image Retrieval

-  <http://beta.hpcc.uh.edu/scs/image/urn:cite2:hmt:vaimg.2017a:VA012RN_0013> (resolve to image)
-  <http://beta.hpcc.uh.edu/scs/image/urn:cite2:hmt:vaimg.2017a:VA012RN_0013@0.04506,0.2196,0.1344,0.10093> (resolve to image)
-  <http://beta.hpcc.uh.edu/scs/image/urn:cite2:hmt:vaimg.2017a:VA012RN_0013?resolveImage=false> (return URL to image)
-  <http://beta.hpcc.uh.edu/scs/image/urn:cite2:hmt:vaimg.2017a:VA012RN_0013@0.04506,0.2196,0.1344,0.10093?resolveImage=false> (return URL to image)


Defining a width

-  <http://beta.hpcc.uh.edu/scs/image/200/urn:cite2:hmt:vaimg.2017a:VA012RN_0013>
-  <http://beta.hpcc.uh.edu/scs/image/200/urn:cite2:hmt:vaimg.2017a:VA012RN_0013@0.04506,0.2196,0.1344,0.10093>

Defining MaxWidth and MaxHeight

-  <http://beta.hpcc.uh.edu/scs/image/500/500/urn:cite2:hmt:vaimg.2017a:VA012RN_0013>
-  <http://beta.hpcc.uh.edu/scs/image/500/500/urn:cite2:hmt:vaimg.2017a:VA012RN_0013@0.04506,0.2196,0.1344,0.10093>


Embedding

![12-recto](https://beta.hpcc.uh.edu/scs/image/500/500/urn:cite2:hmt:vaimg.2017a:VA012RN_0013)

`https://beta.hpcc.uh.edu/scs/image/500/500/urn:cite2:hmt:vaimg.2017a:VA012RN_0013`
{:.figure}

![12-recto-detail](https://beta.hpcc.uh.edu/scs/image/500/500/urn:cite2:hmt:vaimg.2017a:VA012RN_0013@0.04506,0.2196,0.1344,0.10093)

`https://beta.hpcc.uh.edu/scs/image/500/500/urn:cite2:hmt:vaimg.2017a:VA012RN_0013@0.04506,0.2196,0.1344,0.10093`
{:.figure}

###  Relations

CITE Relations are associations of URN to URN, with the relationship specified by a Cite2 URN.

-  <http://beta.hpcc.uh.edu/scs/relations/urn:cts:greekLit:tlg0012.tlg001:1.1> Get all relations for a URN.
-  <http://beta.hpcc.uh.edu/scs/relations/urn:cts:greekLit:tlg0012.tlg001:1.1?filter=urn:cite2:cite:verbs.v1:commentsOn> Get all relations, filtered by a relation-URN.

### Commentary Data Model

If a library includes CiteRelations and implements the Commentary datamodel, comments associated with passages of text can (optionally) be attached to replies for a corpus of texts.

-  <http://beta.hpcc.uh.edu/scs/texts/urn:cts:greekLit:tlg0012.tlg001:1.1?commentary=true>


### Documented Scholarly Editions (DSE) Data Model

The DSE Data model consists of a CITE Collection of objects, each documenting a three-way relationship between (a) a text-bearing artifact, (b) a documentary image (ideally with a region-of-interest defined), and © a citable passage of text.

-  <http://beta.hpcc.uh.edu/scs/dse/recordsforsurface/urn:cite2:hmt:msA.v1:12r> Get all DSE Records associated with a Text Bearing Artifact.
-  <http://beta.hpcc.uh.edu/scs/dse/recordsforimage/urn:cite2:hmt:vaimg.2017a:VA012RN_0013>  Get all DSE Records associated with a Citable Image.
-  <http://beta.hpcc.uh.edu/scs/dse/recordsfortext/urn:cts:greekLit:tlg0012.tlg001.msA:1.1> Get all DSE Records associated with a passage of text.
-  <http://beta.hpcc.uh.edu/scs/dse/recordsfortext/urn:cts:greekLit:tlg0012.tlg001.msA:1.1-1.3> Get all DSE Records associated with a passage of text expressed by a range-URN.
-  <http://beta.hpcc.uh.edu/scs/objects/urn:cite2:hmt:msA.v1:12r-13v?dse=true> (a range of objects in an ordered versioned collection, with all DSE records associated with those objects and properties of those objects -- see below)
-  <http://beta.hpcc.uh.edu/scs/objects/find/urnmatch?find=urn:cite2:hmt:msA.v1:12r&dse=true&offset=0&limit=3> Search all property-values for a URN, with DSE records for the returned objecs. If offset and limit are not used to constrain the returned results, the list of DSEs might be huge, and cause the request to timeout.
-  <http://beta.hpcc.uh.edu/scs/texts/urn:cts:greekLit:tlg0012.tlg001.msA:1.1-1.5?dse=true> Load a corpus of text, with DSE records, if any, for each citable node.

(The dse=true parameter is valid for all object-searching, as well as for retrieval of individual objects or ranges of objects.)

- Christopher Blackwell
