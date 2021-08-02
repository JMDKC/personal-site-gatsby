---
title: Waterfall or straw man?
date: "2021-08-02"
template: "post"
draft: false
slug: "/writing/waterfall-strawman"
category: "Technology"
tags:
  - "Technology"
  - "Product management"
description: "The whole Waterfall vs Agile comparison is a sham. Here's why."
---

The whole Waterfall vs Agile comparison is a sham - because nobody’s really put forward Waterfall as a good way of doing things, not even the inventor of the concept.

So many blogs, tweets and Medium posts about Agile have drawn the contrast. On one side, the old bad Waterfall way of doing things - bloated planning phases, long lead times, no user feedback, big release with no improvements afterwards. On the other, the shiny new Agile way: learning from doing, iterative improvements, listening to users.

This contrast is implicitly drawn in the Agile Manifesto [and its associated principles](https://agilemanifesto.org/principles.html), which posits the bad old way of doing things as over-emphasising “following a plan”, “comprehensive documentation” and ignoring “customer collaboration”.

These days, the comparison is often illustrated in a graph. You’ve probably seen it before, drawing the contrast between the sad linearity of Waterfall, crashing down a staircase of stress, and the sinuous, virtuous Agile loops. Here’s an example.

![waterfall vs agile graph](/media/waterfall-strawman-1.png)
Source: Planview

There are two problems with this very popular contrast.

First problem: far from being an upstart, Agile is nothing new. In fact, it’s ubiquitous: even the most traditional project management behemoths, like McKinsey, are [running their own “agile business units”](https://medium.com/@scotty.middleton/agile-is-dead-mckinsey-just-killed-it-547df8c6c9df?source=email-6374e4b61ef7-1627521385081-digest.reader-f6b05f5c9120-547df8c6c9df----1-71------------------1f20ae93_117e_44a0_bc4b_8641210d99ec-27-1a86e2b3_3b7a_45c3_9ba3_d414a62d9f15). While I’d love to think that we’re still in 2001, the year the Agile Manifesto was drawn up and I was still a teenager, it was 20 years ago. Not to mention that concepts in the Manifesto [have been established business practices for decades before it was written up](https://www.red-gate.com/blog/database-devops/real-origins-agile-manifesto).

The second problem is more surprising. The contrast between Waterfall and Agile pre-supposes a conflict between two different ways of doing things. It follows that each ‘side’ has a set of advocates or fans. If that’s the case, though, where are the people who speak up for Waterfall? Has anybody, ever?

## What if Waterfall was a strawman all along?
The penny dropped for me when I first read [this great blog post from Dorian Taylor](https://doriantaylor.com/agile-as-trauma): not only does nobody speak up for Waterfall these days, he points out, it’s likely that nobody ever has, *including the person who popularised the concept of Waterfall in the first place*!

So, what was the source of the Waterfall? The classic graph - but not, interestingly, the term - was popularised in a 1970 paper by US computer scientist Winston W Royce, [which is freely available online](http://www-scf.usc.edu/~csci201/lectures/Lecture11/royce1970.pdf). I guess it was originally delivered at a conference, as it’s more of a polemic than a research paper.

(Sidebar: it’s unclear how, in the intervening decades, how ‘waterfall’ became the phrase to describe the process. The earliest citation is in [a 1976 paper](https://static.aminer.org/pdf/PDF/000/361/405/software_requirements_are_they_really_a_problem.pdf), which explicitly connects Royce and the word as if it was in common parlance.)

Royce is up front about the opinionated nature of the paper in his introduction: “I have become prejudiced by my experiences, and I am going to relate some of these prejudices in this presentation,” he states. First up, here’s the *original* waterfall graph, from requirements-setting (top left) to delivery (bottom right).

![royce waterfall chart](/media/waterfall-strawman-2.png)

You’d expect the inventor of Waterfall to hold this up as the right way of doing things, wouldn’t you? You’d be wrong. “The implementation described above is risky and invites failure,” Royce states, baldly. “The … method has never worked on large software development efforts and the costs to recover far exceeded those required”.

That’s right. The inventor of Waterfall invented it - *as the wrong way of doing things*. More than that, the 1976 paper that introduces the *word* Waterfall to describe the process explicitly disavows it as a “top down” way of doing things.

Nobody liked Waterfall from the start!

So what’s the alternative? Royce, writing in 1970 - the era of humming room-size IBM computers, COBOL and FORTRAN - advocates *something that sounds very much like Agile*.

Specifically, he praises iterative development, going to market early with a Minimum Viable Product (MVP) and incorporating user feedback in the final build.  He doesn’t call it an ‘MVP’ of course. And the projects Royce was thinking of would involve physical software or hardware, tied to a single delivery date. His version, enabled by the technology of this time, is a “simulation”, a mock-up of the final thing:

> If the computer program in question is being developed for the first time, arrange matters so that the version finally delivered to the customer for operational deployment is actually the second version insofar as critical design/operations areas are concerned… by means of a simulation.   

This “simulation” is a prototype of the final delivered product. Royce says we should aim to get it to market roughly one quarter to one third the way through the project, Royce writes, in order to get “sufficient leverage” on what you finally deliver. And if you don’t?

> Without this simulation the project manager is at the mercy of human judgment. With the simulation he can at least perform experimental tests of some key hypotheses and scope down what remains for human judgment, which in the area of computer program design (as in the estimation of takeoff gross weight, costs to complete, or the daily double) is invariably and seriously optimistic.   

So, in other words, getting something out early to see what works allows the project team to validate assumptions, cut back on feature bloat and get a more realistic handle on delivery time - all impossible with Waterfall development. All important parts of Agile development.

Another ‘Agile’ benefit of prototyping early? Getting user feedback, early:

> What a software design is going to do is subject to wide interpretation even after previous agreement. It is important to involve the customer in a formal way so that he has committed himself at earlier points before final delivery. To give the contractor free rein between requirement definition and operation is inviting trouble… the insight, judgment, and commitment of the customer can bolster the development effort.   

As well as the original Waterfall graph, Royce gives us an alternative one for his preferred way of doing things. These sinuous Agile loops are just about discernible at various stages in the process, building in ‘review’ stages along the way.

![royce agile chart](/media/waterfall-strawman-3.png)

We’re not quite Agile yet, but that’s more due to the technology available to Royce, 50 years ago. He is still tied to a single ‘OPERATIONS’ (or final release or delivery) and iterative improvements *after* release just isn’t a thing.

So it’s still a downwards slope, from top left to bottom right. But it is significantly more complicated, and describes a significantly more iterative process, than that simple iconic first chart.


## If nobody likes Waterfall, why are we still doing it?
So if Waterfall as a concept is so bad, *and was introduced by the very founder of the term as something that should not be done*, why is it still so popular?

I’m firmly convinced that everyone working in product development feels a chilling sense of recognition when they see what’s involved in Waterfall, because they see it again and again in their working lives.

Similarly, Agile as a better way of doing things assumes immense power *by contrast* to this Waterfall reality. These simple bad way vs good way graphs have an avid audience of people working in digital development, who live the reality of business stakeholders bringing solutions to them rather than problems, working on fixed requirements ahead of development, being HIPPO’d (that’d be ‘highest paid person’s opinion’) rather than building according to user needs, and being tied to stressful and error prone huge releases.

Taylor is scathing on this point:

> I want you to consider instead the possibility that Waterfall came to exist, and continues to exist, for the convenience of managers… who, more than anything else, need you to promise them something specific, and then deliver exactly what you promised them, when you promised you’d deliver it. There exists many a corner office whose occupant, if forced to choose, will take an absence of surprises over a substantive outcome.  

And he doesn’t have much hope that Agile can save us from this reality, because it doesn’t cover “anything higher up the chain than project management”. Agile ceremonies and artefacts is, from this point of view, “all tactical stuff”, that doesn’t really change anything.

> Failures to implement Agile principles are often easily diagnosed as side effects of the constraints of antiquated procurement and contracting practices.  

It follows therefore that in order for projects to be Agile, they need to be delivered in an Agile organisation. For an organisation to be Agile, it means that each unit follows these principles. Each unit includes very un-Agile functions like procurement and drawing up contracts. And some of these units are not Agile for excellent reasons - who on earth wants to release an MVP legal contract which we all iterate on, after all? (Though the retro on that would at least be very interesting…)

I think that Taylor’s placing the blame mainly on managers is valid, but also lets people lower down the chain off the hook. I find in my job as an agile delivery manager (let’s face it, another term for project manager) I constantly find myself coming up against our own ‘waterfall thinking’, whether it’s insisting on documenting processes that may or may not be necessary, advocating larger but later releases, or, afraid of a looming deadline, supporting the cutting back on user research and analysis.

While our managers cast us down the waterfall, sometimes we don’t need much persuasion to jump. Sometimes we jump ourselves. While Agile rationally makes sense as a better way of doing things, it’s much easier to talk about in the abstract rather than just *do*.

## A few conclusions
So, now I know that:
a) Agile is an attractive idea that’s reached maturity in the business world
b) nobody ever liked Waterfall, including the person who popularised the concept 50 years ago
c) Despite these intervening years, Waterfall is still instantly recognisable to people working on digital projects
d) Many businesses have adopted Agile practices - the popular new thing - in a facile way, leaving the old way of doing stuff broadly unchallenged
e) There are obviously loads of factors behind this being the case! But one major one is - our managers
f) And, if we’re honest, we in digital teams also reinforce Waterfall ourselves. Because it’s superficially safer, and playing safe is hard wired into human nature.

That’s a tough set of truths to accept, as it means that being truly
Agile, and working in a truly Agile environment will be a hard uphill battle for everyone. And that doing so will involve overriding some natural instincts, and persuading better-paid people to override theirs. Very often, it will be doomed to failure. Agile benefits may only be, as Taylor says, “tactical” - and maybe we should be happy with that.

A more achievable conclusion for me is - the next time I see one of those graphs with the bad old Waterfall staircase on the left, and the nice new Agile loops on the right - I’ll give it an eye roll. The easy dichotomy is not so easy. It’s not a comparison of competing ideologies. It’s a battle between our instincts and our rational brain!
