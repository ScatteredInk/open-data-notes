---

title: "Government as a Platform Playbook - some implications for Beneficial Ownership Transparency"
date: 2019-08-15T12:39:52+01:00
draft: false
math: false
series: ["Beneficial ownership data"]
hideReadTime: true 
meta: true
toc: false
author: "Jack Lord"

---

Richard Pope's [Government as a Platform Playbook](https://platformland.github.io/playbook/index.html) (GaaPP) is a clear and insightful summary of the move from simply digitising government services to (re)building them on "platforms" that are modular and can be reused by multiple service designers. In theory, this allows services to be designed around the needs of citizens, rather than replicating the structures of a government. The GaaPP helped clarify some of my thinking around the local context of implementing beneficial ownership transparency (BOT). That context involves not just legal frameworks and technical capacity (to which we have paid a lot of attention) but service availability (which we have probably underplayed). BOT has a lot of *dependencies* on other government services and, if implemented well, could potentially *add value* by providing services to other parts of government.

This post contains a series of, largely unordered and disconnected, implications for BOT implementation that occurred to me as I was reading through the Playbook, as well as some brief notes on the GaaPP itself. I recommend reading the whole thing, and there are some interesting essays listed in a related Twitter [thread](https://twitter.com/richardjpope/status/1158746606155571206) too.       

<!--more-->

# Platforms and Beneficial Ownership Transparency

{{% newthought %}}Platforms demand stability{{% /newthought %}} but, as a greenfield space,{{% sidenote %}}In most cases, either BO data doesn't exist yet or it exists but we aren't sure if it exists in its best/final form.{{% /sidenote %}} BOT is likely to be unstable, so identification as a building block for other critical services should be avoided until something approaching BOT 1.0 exists. This doesn't have to stop pilot use of data in other services but these should be on a limited basis and with the **expectation of instability**.

{{% newthought %}}Platform availability will shape BOT implementation.{{% /newthought %}} The presence or absence of reusable platforms for addresses, company registers, identity, proofs etc will impact (1) how BOT is implemented (what regulations/laws need to be look like, how systems are built) and (2) the quality and interoperability of data that results. We can roughly tell what BO will look like from legislation alone, but an early mapping of platforms would make prediction, planning and early intervention to improve BOT much easier. 

{{% newthought %}}Ledgers not lists.{{% /newthought %}} The idea of a canonical list of "agreed facts" is simple and powerful. But for domains where change-over-time is essential the concept of a 'list' is a potential over-simplification that will result in bad policy or design decisions. This isn't because there is something inherently wrong with lists but because it is very easy for a list to be negotiated down to "the agreed facts *at this moment in time*".

The ledger metaphor, by contrast, embeds the idea of reconstructing the state of the agreed facts *at any particular moment* ("who did we think owned Company A on 31st Dec 2018?"). A ledger is a harder sell than a list but this upfront cost is worthwhile. Governments need archival/memory functions - so, then, do their platforms.

Both of these are lists of company owners. The first list shows us who owns a company *now*. 

| Company Name | Company ID | Owner | From |
| ------------ | ----------- | ---- | ----: |
| Shell Corp  | XE-001 | Mr Nominee | 2018-12-01 |
| Real Company | XE-002 | Raleigh Real | 2001-06-06 | 

The second list is a ledger. It shows us who owns a company now (so we could create the first list from this list if we wanted a simplified version). And it lets us see who was described as owning a company on any particular date. It also shows that any list of company ownership that can't be used as a ledger is open to abuse.  

| Company Name | Company ID | Owner | From | To | Notified |
| ------------ | ----------- | ---- | ----: | --: | --: |
| Shell Corp   | XE-001 | Jack Lord | 2018-01-01 | - | 2018-01-31 |
| Shell Corp   | XE-001 | Jack Lord | 2018-01-01 | 2018-12-01 | 2019-01-01 |
| Shell Corp   | XE-001 | Mr Nominee | 2018-12-01 | - | 2019-01-01 |
| Real Company | XE-002 | Raleigh Real | 2001-06-06 | - | 2018-01-01 |

{{% newthought %}}Co-ordinating and contributing to a shared data infrastructure{{% /newthought %}}. Much of the value of beneficial ownership transparency will come from the network effects of interconnected data. This will require agreeing standards for publishing data. But, at a more fundamental level, it will require a coordinated effort to create and maintain a shared infrastructure that enables publication of easily interoperable data. Corporate ownership is transnational in nature so, for example, a state that wants to publish data on legal entities that own domestic companies needs reliable company identifiers for both domestic and international companies. It may also want other lists of agreed facts, like types of legal forms or metadata on personal identifiers.

Generally, these are *governance* rather than *technical* questions. Solving this issue is likely to involve some combination of: (1) Creating new lists where they don't exist. (2) Raising awareness that international partners are important users and stakeholders for data relating to companies and personal identity. (3) Winning the argument that contributing to and updating a shared data infrastructure are an integral part of implementing BOT.

{{% newthought %}}Event-driven beneficial ownership disclosures{{% /newthought %}} (e.g. a natural person goes over a 25% ownership or control threshold and is automatically declared a beneficial owner in a public register) are one counter-balance to a potential explosion in automated formation of short-lived companies and complex company networks - with all the harmful impacts on transparency and accountability that implies.{{% sidenote "sn-2" %}}See [Fireflies and algorithms — the coming explosion of companies](https://medium.com/@opencorporates/fireflies-and-algorithms-the-coming-explosion-of-companies-9d53cdb8738f). I think this article is too techno-fatalistic about the path we are on. Beneficial ownership transparency, for example, clearly introduces a new friction to company formation but has managed to win relatively wide support over the last few years - the race to the bottom is not a sure thing.{{% /sidenote %}} But this is a very long-term project, both politically and technically, and will require a rethinking of where company register data is held and who has access to it.{{% sidenote  "sn-4" %}}See [this post]({{< ref "beneficial-ownership-registers-who-knows-what-when.md" >}}) for some early thoughts on this. I think the legislative models adopted in several Anglophone African countries, which link beneficial ownership and members' registers, potentially offer a useful legal basis to work with.{{% /sidenote %}}

{{% newthought %}}Segmentation of service-users simplifies implementation.{{% /newthought %}} This is most obvious when thinking about using canonical lists (e.g. only check addresses for domestic beneficial owners, as in Ukraine, or only verify that the next legal entity in the ownership chain is real if it comes from the domestic company register). But it could also work for incremental compatibility with an ecosystem of digital identities: domestic identities first, then regional identities like eIDAS, then investigate other possibilites for users who fall outside these categories.

{{% newthought %}}The questions people want to ask about company ownership are relatively simple{{% /newthought %}} even if bitemporal data and modelling company ownership are complex. The service/API should be able to answer simple questions ("Who owns company A?", "Who owned company A on this date?", "Was the ownership of company A by person B on this date public knowledge?") and make the complexity optional.       


# Notes

{{% newthought %}} Digital vs platform government{{% /newthought %}}. Simply 'digitizing' governments creates problems:

1. Duplication of data.
+ Duplication of effort.
+ Service design replicates the design of government, not the way that users expect/want/need to interact with government services (Conway's Law).
+ Monopoly provision and subsequent lack of complementary design.

Government as a platform is an alternative approach that can "break down organizational silos, save money and change the types of services that can be delivered to the public". E.g, Estonia is using newly developed digital infrastructure to design services around 'life events' rather than structuring interactions around "the boundaries of government agencies".

The infrastructure layer of GaaP is "shared components, APIs, standards and canonical datasets".{{% sidenote "sn-1" %}}Richard Pope. ‘Government as a Platform Playbook’. Accessed 15 August 2019. https://platformland.github.io/playbook/book/text/introduction.html.{{% /sidenote %}}

{{% newthought %}}Users{{% /newthought %}}. Because platforms are "building blocks" their primary users are "the people and organizations who use them to create services for the public", rather than end users (who may interact indirectly with a platform through many different services without knowing). The status as a building block creates a responsibiliy around the impact of changing/withdrawing a particular platform.

{{% newthought %}}Identifying platforms{{% /newthought %}} can be done via mapping, interviews, legislative reviews etc. This may reveal common needs that could become platforms. Products can also be turned into platforms if a route is available.

{{% newthought %}}Shared data infrastructure{{% /newthought %}} is crucial. Components: (1) canonical registers or "agreed lists of facts" that serve multiple services. (2) open standards: prefer "progress, working implementations, public evolution and concrete use cases over perfection and completeness". (3) APIs, both creating new ones and building on existing ones. (4) Bulk downloads of data (but think about non-developers too).

{{% newthought %}}Adoption.{{% /newthought %}} Mandates should be used carefully and only considered once "you have proved it is useful".

{{% newthought %}}Designing services.{{% /newthought %}} Some principles: (1) Build services to solve (whole) problems, rather than replicate government structures. (2) Services can be built modularly (and experimentally) from platform components. (3) Platforms should expect/encourage "multiple, overlapping services" built on them, perhaps serving slightly different audiences (or audiences with slightly different preferences). (4) Real-time services are useful but can introduce extra risks and the need to decided "where there should be a human in the loop". (5) Event-driven services (i.e., a service driven by updates to a canonical register rather than a user-submission) reduce user-error ("I didn't know I needed to file *that* form") (and the cost of keeping users informed of policy updates?).

{{% newthought %}}Identity, trust and consent.{{% /newthought %}} Some principles: (1) Design for an identity ecosystem (may include private providers or regional systems like [eIDAS](https://ec.europa.eu/digital-single-market/en/trust-services-and-eid)). (2) Design for trust escalation and build in offline alternatives. (3) Context is important, and can bring enormous risks. (4) Limit the amount of data that is collected. (5) Be transparent about how open the data will be and what it will be used for. (6) Create APIs that answer questions. (7) Digital proofs remove some of the risks of paper, while allowing verifiability. Standards are being developed in this area.     

























