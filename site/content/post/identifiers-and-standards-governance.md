---

title: "Identifiers and Standards Governance"
date: 2019-03-04T11:33:51Z
draft: true
math: false
hideReadTime: true 
meta: true
toc: false
author: "Jack Lord"

---

{{% newthought %}}In open data{{% /newthought %}}, and in open data standards, everybody loves identifiers. But maybe we love identifiers so much that we are accelerating use and production of identifiers, at the expense of:

- governance and documentation for identifiers use and publication (particularly when identifying a 'thing' gets tricky);
- resourcing the common good infrastructure for co-ordinated publication patterns; and
- research and development that will help us avoid a lot of legacy issues in 3-5 years time.

This post is about the current dynamics between open data standards and identifiers, as I see them, and the implications for what might need to happen next.      

<!--more-->

 {{% newthought %}}Stable and permanent{{% /newthought %}} identifiers mean that you always know who or what you are talking about.{{% sidenote "sn-1" %}}A good summary report on the advantages of open identifiers, and best practice, is Open Data Institute and Thompson Reuters, [“Creating Value with Identifiers in an Open Data World](http://innovation.thomsonreuters.com/content/innovation/en/labs/data-identifiers.html).,” 2014.{{% /sidenote %}}
 While a company name can get written down in a dozen different ways (Open Data Services, Open Data Services Co-operative Limited, ODSC, Open Data Services Coop, ...), a well-defined identifier for a company will be unique and unambiguous, and follow the company throughout its life.
 Thus, using the [org-id.guide](http://org-id.guide/list/GB-COH) scheme, Open Data Services Co-operative Limited would be identified as `GB-COH-09506232`, even if we changed our name to Closed Data Uncooperative Limited - which we might have to, if people don’t start using better identifiers.

## Standards and identifiers: emerging stresses

My sense from working on org-id.guide and from watching discussions emerging in various data standards, is that the current demand for organisational identifiers is outstripping our collective ability to deliver a sustainable ecosystem of useful, usable and interoperable identifiers.
I don't think this bad, per se.
Rather, it looks like the inevitable growing pains of a set of data standards that are reaching maturity, discovering new use cases or simply hitting the complexities of the domains they cover.
The existing identifier infrastructure is inevitably stretched by those situations. The solution to this is only partly technical.
A much larger effort will be required to think about governance and user needs within and between data standards for identifers - and, from there, to work out what infrastructure is required to support existing standards to grow and, increasingly, for the data produced to be put to use.

Some of the most important dynamics that emerge from data standards loving identifiers, include:
      

1. Technical demands are placed on institutions and systems that lack capacity, particularly in the global South.
2. Publishers are tempted to choose a “good” identifier over adherence to the meaning of data standard mappings
3. Publishers are tempted to choose a “good, but not open” identifier.
4. A desire to push the boundaries of *what* can be identified to *who* can be identified, without the legal or metadata scaffolding that would allow such data to reused with confidence.
5. Organisations are encountered over their whole lifecycle, with different official identifiers. This is particularly relevant to 360 Giving or the Social Economy Data Lab Specification, where a grant-giving body might give funds to an organisation that is, at various times, an unincorporated association, a charity or a community benefit society. With a simple implemenation of identifiers, this will look like a grant being given to three *different* organisations. A data user, though, might reasonably expect the organisation ("the thing itself") to be the same in these instances.{{% sidenote "sn-2" %}} GLEIF's discussion paper on [predecessor entities](https://www.leiroc.org/publications/gls/roc_20170726-1.pdf) has some useful material that could inform to how standards might incorporate the temporal aspects of organisations into their own guidance on {{% /sidenote %}} 
6. Good identifier systems are, on closer inspection, weirder and less good than we thought.

What this means for data standards:

1. Resourcing stop-gap solutions in environments that lack capacity.
2. A monitoring process to ensure that stop-gap solutions don’t become needlessly permanent, i.e., when jurisdiction X implements a proper company register.
3. Having governance processes and documentation in place so that uncertainty and compromise in some data doesn’t undermine the usefulness of the data as a whole and the perceived meaning of the publication standard.
4. Compromise in the present over identifiers - and given the catalyst for poor systems to change in future any improvements in the future - will require governance, monitoring and technical efforts to integrate new and legacy data and systems into coherent workflows for data users and publishers.



