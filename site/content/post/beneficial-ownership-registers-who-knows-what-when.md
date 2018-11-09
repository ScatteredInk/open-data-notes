---

title: "Beneficial Ownership Registers: who knows what?"
date: 2018-11-08T13:35:08Z
draft: false
math: false
hideReadTime: true 
meta: true
series: ["Beneficial ownership data"]
toc: false
author: "Jack Lord"

---



<!--more-->

This is an condensed, expanded *and* tidied up version of a talk I gave at EITI's Opening Up Ownership: Africa conference, Dakar, Senegal in November 2018. It covers which actors know what in the beneficial ownership disclosure process, and some of the implications for data quality, business processes and register design.   

{{% unboxedsummary title=""%}}Lord, Jack. “Beneficial Ownership Registers: Who Knows What?” presented at the EITI, Opening Up Ownership: Africa, Dakar, Senegal, November 1, 2018.{{% /unboxedsummary %}}


## Moving from information to data

Today's panel is about the accuracy of beneficial ownership information. I want to talk about moving from information to data and why maintaining accuracy is such a hard problem when describing beneficial ownership. Part of my work involves writing a [data standard](http://standard.openownership.org/en/schema-beta-2/) - a template - for benefical ownership information. In general, therefore, my stance is that data is good: data has structure; data is exchangeable; data is interoperable. If it is standardised data costs less to use and analyse.

But I also come at this topic from the point-of-view of a data sceptic. I work with data but I often have a hard time believing it. As a result, I'm very interested in understanding the underlying factors that determine data quality - and how we can intervene to improve data quality.

For beneficial ownership data, this is not just an intellectual exercise. Poor quality beneficial ownership data will sit unused on a register. High quality beneficial ownership data has the potential to become the kind of actionable intelligence or evidence in a court of law that the other panellists have talked about.

## Knowledge about beneficial ownership

There are two primary problems relating to knowledge about beneficial ownership:

1. No one source gets to the truth of who the real beneficial owner is.
2. No single actor has a complete view of the beneficial ownership of a legal entity.

That means two things.

1. Beneficial ownership registers are necessary - but they are not sufficient.
2. Data collection is a co-ordination process. The challenge is to find the most knowledgeable parties, collate the information that they hold and then publish it.

So, if we want to decide how to do the work of collecting and verifying information about a company, we should ask: who knows most about the ownership of that company?

## Verification

I won't talk much about the first problem - that no one source gets to the truth of who the real beneficial owner is - today. But, briefly, the "truth verification problem" points us towards the need for inter-operable data and to platforms that aggregate claims about the state of the world, which can then be interrogated and compared by experts.

In practical terms, to understand if someone is lying about beneficial ownership about a block of shares, we need two pieces of information:

1. A statement of who the *beneficial owner* is supposed to be.
2. A trail of who the *beneficiaries* from that block of shares actually are.

Those are two different kinds of information: one is about the ownership of legal entities, the other is about the ownership of accounts. But to become actionable intelligence, both pieces of information must be interoperable - and this is where data standards come in. When the other panellists talk about platforms and centres of excellence, the direction of travel will need to be towards data standards, precisely because those platforms will deal with input from such a diverse array of sources and systems.

## Three stakeholders

I want to mainly discuss the second problem: identifying the parties who are most knowledgeable about beneficial ownership, and co-ordinating the collection and publication of what they know. I'll discuss three main stakeholders in this process: natural persons as legal or beneficial owners of companies; companies as reporting entities; and central beneficial ownership registers.{{% sidenote "mn-5"%}}There are a couple more stakeholders that could usefully be considered here: financial intelligence units plus other competent authorities and third-party verifiers of data.{{% /sidenote %}} And, in each case, I want to ask:

- What do they *know*? 
- And, given what they know know, what do they *need* in order to create *accurate* beneficial ownership information.

### Natural persons, as legal and beneficial owners. 

Let's first consider natural persons, in their role as legal or beneficial owners of companies. Natural persons level of knowledge is generally very high. Individual shareholders or beneficial owners know (or can find out) how many shares they own, how many votes they control and what other influence they might wield over a company. Individual shareholders also know, unsurprisingly, the most about themselves: their names, addresses, identity numbers, nationalities and tax residencies. Crucially, they have access to the *canonical* representation of those details: a name as it appears on a national identity card, for example (and not an approximation thereof). They also know whether, when they make a disclosure about these details, they are telling the truth - and when, and how far, they are diverging from their canonical representations.{{% sidenote "mn-1"%}}On the UK's companies House, for example, there is someone called “Ali Moulaye”, whose name is on the paperwork for dozens of different companies, using [seven different spellings](https://www.linkedin.com/pulse/finding-ali-moulaye-detective-story-graham-barrow). His true relationship to those companies is not clear. This is where things connect with [authorisation](https://openownership.org/news/what-we-really-mean-when-we-talk-about-verification-authentication-and-authorization-part-2-of-4/): the *right* to make a statement. Without some mechanism to ensure that an authorised person is making a statement, it is much easier for a company or beneficial owner to disclaim responsibility for a statement on a beneficial ownership register.{{% /sidenote %}}


But, while natural persons know a lot, they lack the capacity to report that information in a consistent way, and in a format that is consistent enough to work for scalable analysis techniques. That is, the lack of capacity will manifest in two ways: misunderstanding the rules (and so making incorrect declarations) and using whatever leeway is available to subvert data entry expectations (and so making declarations that are inconsistent).{{% sidenote "mn-2"%}}This is a particular challenge with paper forms. Here the need is to make the forms as clear as possible, publish guidance alongside the forms, and have validation processes in place when the forms are transferred to electronic format.{{% /sidenote %}} These are crucial problems for beneficial ownership registers to address for three reasons:

1. Bad actors will take advantage of a low information environment. Honest mistakes create room for dishonesty to hide.
2. Any enforcement is likely to be ineffective while false statements can be attributed to mistakes.
3. Risk-based approaches to verification and investigation are likely to be compromised by the ubiquity of bad data. 

To help shareholders and beneficial owners minimise mistakes, companies and registers need to provide access to their tools and expertise. This means well-designed forms, guidance and data validation. We want that grounded knowledge - but we also want it to be correct.

### Reporting companies 

As for companies reporting on their beneficial owners, they also know quite a lot - but their knowledge is about different things.

For an authorised person inside a company, ownership - meaning legal ownership - looks like a list of shareholders: a register of members. That list is kept up-to-date - but perhaps not always up-to-date when it comes to personal details. A company therefore has a more holistic view of the overall ownership position than any individual shareholder.

But there are definite limits to what a reporting company knows. One of those limits is set in stone: a company is never going to know, for certain, anything more than the identity of its legal owners. But, given the right tools and capacity, a reporting company can collect information from its legal owners and report on this basis. 

For this to happen, companies need two things:

1. On the technical side: good forms from the registry, guidance documents so that they can inform shareholders what they expect in terms of information and perhaps also access to the same validation tools so that they can check if the data that they receive from shareholders conforms to the data that they are expected to submit to the register.
2. On the legal side: the power to chase non-responding shareholders, query incorrect data and freeze rights attached to shares if disclosure rules are not followed.

Note that, in a complex ownership chain, the further one gets from a company's legal owners, the more uncertain the information collected becomes. And, more importantly, the toolset that registries can provide *also becomes ineffective* if any link in that chain is outside the original jurisdiction. This has very important implications for how much data is collected, and by who.{{% sidenote "mn-2"%}}In particular, it implies that the stance that "collecting the whole ownership chain is better" is wrong because the practicalities of doing so are so difficult and the quality of resulting data is likely to be low. Instead, minimal but high-quality beneficial ownership information based on the first layer of legal owners is likely to be optimal.{{% /sidenote %}}  

### Registers

Registers of beneficial ownership want to know a lot - but, as things stand, they actually know very little. The limits of what registers know is what information is submitted to them by more knowledgeable parties.

But registers have four important roles in creating knowledge about beneficial ownership. 

1. Registers act as as co-ordinators of the submission process, setting the rules on time, place and format. They also hold the stick when it comes to enforcement - if the right regulation is in place.
2. Registers are stewards of data quality. Here, again, registers play an enabling role. They can provide the tools and guidance that allow the partners with the knowledge to pass on that information accurately. While registers want to leverage the knowledge held by shareholders and companies, shareholders can use the capacity of registers and/or the knowledge of companies to simplify declarations and companies can use the capacity of registers to ensure the accuracy of the information they collect, reduce the reporting burden and make sure that shareholders comply with the rules. 
3. Registers are aggregators (and hopefully publishers) of information provided by others. If this aggregation is done well then users will be able to tell where a given piece of information came from and make their own judgement on its truthfulness.{{% sidenote "mn-6"%}}From conversations with colleagues at OpenOwnership, it has become clear that aggregation is the key feature of beneficial ownership registers - something I'll address in a future post.{{% /sidenote %}} 
4. They are knowledge producers. Although registers know very little directly, in aggregate registers can know a lot. If registers have the tools and capacity to combine and analyse beneficial ownership data, this can create new kinds of knowledge about company ownership. Registers should be the bodies most able to see patterns and identify red flags.{{% sidenote "mn-6"%}}For an example, see “The Companies We Keep.” Global Witness. https://www.globalwitness.org/en/campaigns/corruption-and-money-laundering/anonymous-company-owners/companies-we-keep/.{{% /sidenote %}}  Additionaly, registers have the advantage of being able to pull in external sources of data to cross-check and verify what is submitted.     

## What this means

What does this mean for beneficial ownership data collection? In terms of 'who collects' and 'who declares' there is unlikely to be a single perfect model. But there are two guiding principles that we can keep in mind when designing such processes.

1. We want to optimise collection and declaration practices for the information available to stakeholders and their capacity to collect it accurately and in a timely manner.
2. Capacity is more flexible than information availability.

This suggests that we may want to focus our efforts on decentralising the *capacity* to collect accurate beneficial ownership data. That does not mean that every shareholder or reporting company needs to become an expert. Instead, it may mean widening access to validation and submission tooling so that knowledgable stakeholders can create accurate information and exchange it *among themselves* before submission to a central register.

To make that happen, all of those stakeholders must be able to describe and exchange information about beneficial ownership using a common template and language - and that means adoption of a common beneficial ownership data standard, and a set of shared tools and methods. And though the idea of decentralised use of data collection and validation tools may seem more complex than current register designs, it lays the groundwork for both high-quality data and the widespread use and re-use of beneficial ownership data elsewhere. 


