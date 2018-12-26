---
layout: post
title: Access to HMT Facsimiles
tags: [news, update]
---


The Homer Multitext is producing complex data. The complexity is irreducible, since it is our mission to publish digital editions mapped to their manuscript folios, with Iliadic texts associated with commentaries.

This complex data is published as [a single CEX file, a plain-text serialization of the current state of the HMT](https://github.com/homermultitext/hmt-archive/tree/master/releases-cex). That data is also exposed via a [web service](http://beta.hpcc.uh.edu/hmt/hmt-microservice/), and an integrated web-application. For more straightforward access, we have published [a facsimile view of the data](http://www.homermultitext.org/facsimiles/).

This post is to announce [the Homer Multitext Facsimile Index application](http://www.homermultitext.org/facsimile/index.html), allowing users to access HMT data based on Iliadic citations, e.g. 2.100 (individual passages), or 2.1-2.10 (ranges of passages).

Because traditional citations assumed an audience of (clever, intuitive) human readers, some traditional practices do not translate to a computational environment. For example "1.1-10" is not a valid, that is, unambiguous citation. Does it mean "from 1.1 to 1.10" or "from Book 1, Line 1, through all of Book 10"? The unimaginative machine will assume the latter. So with this app, and with CITE data generally, users must be verbose and specific: 1.1-1.10, with [book].[line] on both sides of the hyphen.


-  [Homer Multitext Facsimile Index](http://www.homermultitext.org/facsimile/index.html)


As with all expressions of HMT data, this application was build with [the CITE Architecture code libraries in Scala and Scala-JS](http://cite-architecture.org/).

- Christopher Blackwell
