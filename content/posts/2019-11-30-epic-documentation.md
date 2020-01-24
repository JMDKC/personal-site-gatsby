---
title: Epic documentation
date: "2019-11-30"
template: "post"
draft: false
slug: "/writing/epic-documentation" 
category: "Product Management"
tags:
  - "Product Management"
  - "Strategy"
  - "Business"
description: "Agile documentation needs to do the minimum viable job. Docs shouldn’t be comprehensive, but they should still exist. Here's an example."
---

It’s right there in the [Agile Manifesto](https://agilemanifesto.org/): today’s product teams should prioritise “working software over comprehensive documentation”.

A nice thought. But having notched up several years of working with Agile teams, I feel like these five words have led to an unfortunate belief taking hold among certain zealots: that we don’t need documentation at all!

Which is nonsense. We need the leanest, briefest, most maintainable documentation possible. But we need documentation all the same.

This is what the Agile Manifesto states in the first place. Here’s a [useful summary from Jonathan Berger](https://content.pivotal.io/blog/minimum-viable-deliverable):

> Agile seeks to minimize waste, so taken to its logical extreme, *all documentation is waste*. That doesn’t mean documentation can (or should) be done away with entirely. But it does suggest that minimizing documentation is a Good Thing.  

So documents in themselves aren’t bad, they just need to do the minimum viable job. They shouldn’t be “comprehensive”, but they should still exist.

Here’s an example of a useful document I’ve started using: the **Epic document**. The thinking behind this doc is very much a work in progress. The doc’s sections are a mishmash of convention and convenience. The process comes loaded with caveats. But I’m pretty pleased with this doc approach, pleased enough to post this mini-case study about it!

### Background

First of all, here’s why the docs are based around the team’s Epics. The Agile teams I work with both use JIRA as our issue-tracking tool, though the learnings are relevant to other tools.

![](/media/epic-documentation-1.jpg)

I’m defining Epics as large units of work for the team, accompanying “more than several” individual stories, which are themselves captured as individual tickets in the tracker.

To use an illustrative example, the work for building the CRUD for a particular tool in the CMS would likely be one or two stories; but building the tool as a whole - including additional stories for the data model, front end and so on - would be an Epic.

The main problem that led me to start these docs is that the members of the team working further down the funnel - mainly developers - often felt that we were not getting enough into the “why” of the things they were building. Our Product Manager would often come with lists of requirements that I worked with him to produce stories for, which were then reviewed and refined by the devs, designer and QA.

The question of where the requirements came from, why we were doing it, and what results we were targeting, often got left by the wayside. 

The problem had easy-to-define causes. Firstly, we encounter the extremely common problem of the business making strategic decisions without involving the product team, and giving lists of fully-formed requirements accompanied by a tight deadline which we have to “just deliver”. This meant that just getting everything into JIRA and into a workable state for the devs was a challenge, and that there was often simply no time to consider the “why”.

The second cause, I’m afraid to say, is that we’d swallowed a bit too much of the Agile snake oil - and regarded any and all process documentation as unnecessary to efficient working.

The third - I was inspired by this article about Amazon’s business practices - which involves a surprising amount of documentation. They start the process with writing an [imaginary press release](https://medium.com/@IndianaStyle/amazon-press-release-how-to-55d61188ecdd) for the final product: a short document that’s focused on the “why”, in other words.

Lightly adapted, our Epic docs provide a touchstone for the team, explaining the “why” as well as the “what” behind each of the Epics we take on.

### Execution

As Atlassian, the maker of JIRA, [states in its own documentation](https://www.atlassian.com/agile/project-management/epics), part of the role of Epics is to connect the nitty-gritty of fully-estimated user stories with the broader business strategy: 

> Breaking initiatives into **epics** helps keep the team’s daily work — expressed in smaller stories — connected to overall business goals. As a team learns more about an epic through development and customer feedback, user stories will be added and removed as necessary. That’s the key with agile epics: Scope is flexible, based on customer feedback and team cadence.    

All of which I agree with. But just keeping work items as Stories, themselves tied within Epics, without a higher-level document to explain the thinking behind the Epic, was leaving people feeling a bit stranded as to why they were doing the work in the first place.

So, over the course of a few sprints, I worked on putting together just such a summary document. Through trial and error, the documents coalesced around the following sections:

* **Metadata:** a section at the top of the document with basic information about the Epic - its name, JIRA issue key (with a link to that JIRA issue), who wrote the document (always me, sometimes with the Product Manager in a supporting role), and with links to any initial prototypes and wireframes the designers have completed
* **Introduction:** a summary of what the product or product increment is covered by the Epic. Using the example below, this could be a CMS tool. An integration with our CRM system. A new section of a website. Anything, so long as it’s bigger than a few Stories!
* **The important bit… the why behind the Epic:** This is the bit that I most need our Product Manager’s help with. I’m looking for actionable information in the following sections:
	* **The business case**: Exactly why are we doing this? Who has asked for what we are delivering? What problem for our users will it solve - and who are these users?
	* **The business cost**: Which parts of the product team need to work on this? Roughly how long for? If it’s been asked for by the business, or if we need to work with an external agency or partner, who owns that relationship?
	* **Expected results**: I’m pretty liberal with this one, but we need one or more signposts on whether we are looking for uplift on one of our quant metrics, faster load times, or even better a measurable financial impact!

Finally, at the bottom of the document, an optional extra: I draft a list of Stories that I imagine we will need to complete the Epic. We keep them in the “[Given/When/Then](https://www.agilealliance.org/glossary/gwt/)” format 

Note the “imagine” and “draft” in that last sentence. At this point, nothing of the Epic is in JIRA yet. The document, built by the Product Manager and me, needs to be tech reviewed by devs and QA, and any designer who didn’t work on the prototypes, in a story estimation meeting. From there, the initial list of Stories are plugged into the issue tracker. The draft list in the Epic document can be revised or even deleted if you like. It’s served its purpose, to drive conversation in the story estimation meeting.

The important part of the document - the “why” - is the only part that will be revisited as the work gets done. Every time we wonder what the user need is, we revisit and update the document. And if requirements change significantly, we revisit the document to check the original purpose behind the Epic.

### Results

You’ll probably have guessed by now that I was the driving force within the team for producing these documents. So I’m going to be as honest with myself as possible when putting together the list of Pros and Cons of our experience with Epic documents so far.

**Pros**
* These documents have been effective in the Product Manager’s validating of background assumptions as to why we *need* a particular new tool or feature.
* They’ve become very useful reference documents for me, who works on delivery further down the funnel, in providing an effective one-page summary of a particular product or feature.
* They fit in well with our current workflow: of course, they are keyed to individual JIRA epics. The documents themselves are in Google Doc format, and are stored in a particular folder in our team Wiki, which is on the corporate G-Suite. While you could put them in Confluence or Sharepoint, they must be living and editable documents, subject to changes and accessible to the team at any moment, *not* forgettable and losable attachments on an email.

**Cons**
* To be truly Agile, these documents would be a resource written by and maintained by the team. At the moment, the devs aren’t really involved. On one hand, this is to be expected - as the developers might naturally work more on the Stories, which are tech reviewed and estimated by them. And, quite naturally, the devs are more inclined to be opposed to over-comprehensive documentation. But on the other hand, everyone in the team should have a degree of ownership on the “why” behind the products, and nobody should be solely focused on the delivery.
* While pretty minimal, I can see these documents getting bloated over time. Because that’s always the way with IT documentation, which is itself the reason the Agile Manifesto was written in the first place!
* The documents are a long way from [true OKRs](https://weekdone.com/resources/objectives-key-results) - the success metrics mentioned in them are only suggested, rather than enforced. Similarly, the documents are closely coupled to JIRA epics rather than the broader business strategy, making them of limited use outside of the product team. 

### The future

For me, it is going to be a process of addressing these cons, one by one. 

Something to try in 2020 is to make them shorter and more visual, merging sections, and maybe doing away with that suggested story list altogether.

Watch this space for how I get on.
