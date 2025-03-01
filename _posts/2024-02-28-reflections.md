---
title: "Reflections: 2.24-2.28"
date: 2024-02-28
---
# Summary 
Research was again pretty unremarkable, though I did have a nice conversation with one of the doc students in our lab. I spent more time practicing Hebrew than last week, and much more time journaling. I also listened to another interesting podcast about ["Quantum Birds"](https://radiolab.org/podcast/quantum-birds) (gotta love Radiolab). 

## HivE Research
I met once with Dr. Hyman to clarify next steps in our model discovery project. As a lab, we spoke about a very dense (but methodologically and interpretively interesting) paper characterizing (putatively) bidirectional hippocampal-cortical interactions thought to support mechanisms of memory consolidation (specifically, the "short wave ripple", or SWR)[^1]. After that meeting, I had a chance to chat with one of the lab's doc candidates about my research and possible collaboration; see below.  

### Projects
**Reproductions.** I met briefly with the RA working on the reproductions work. He said he enjoyed working through the MATLAB tutorials I pointed him towards. He is continuing to work on said tutorials this week, and I will draft a more ganular schedule of our goals until we get to OURS in May. 

**Model Discovery.** I've named this next project, yay! I like the term "model discovery" because it suggests a continuation of the DSR efforts. Indeed, as NN-based DSR seeks to discover underlying dynamic system structure "agnostically", so too does this new project seek to characterize the hypothetical (dynamic?) features guiding how the neural data we recorded was generated. 

What do I mean by "agnostic"? Unlike the approach I'm working on with Dr. Hyman, the DSR I read about (i.e., approaches developed at the [Durstewitz Lab](https://durstewitzlab.github.io/)) doesn't seek to regress dynamic system activity onto a pre-defined library of candidate features/functions. In this sense, said DSR approaches are less "agnostic" about what underlying system dynamics are; they just "discover" them. (I put *discover* in quotation marks because I still understand very little about how such NN-based "agnostic" approaches actually work.) The regression approach, reminiscent of SINDy[^2], is what Dr. Hyman and I are working towards. (My qualm is that such an approach seems fundamentally biased towards how we pre-define such a library of relevant features/functions characterizing a system, but - you gotta start somewhere.)

Specifically, my goal is to stitch together some sort of methodology for regression-based feature selection. These features, in turn, would be used to characterize a model (in our case, a model describing *how* the neural data we collected was generated), which, in turn, could hopefully provide a pathway to elucidating testable hypotheses about the significance of said features to the underlying data-generating process. Let me clarify things with an example: 

> Rats completing a hierarchical task in a maze may have to track information about where they are in the maze, what phase of the task they're on, and whether they're doing the right thing (i.e., whether they've been rewarded for past actions). Accordingly, the neural activity recorded from a brain structure thought to track such task-relevant featues (e.g., the ACC[^3]) ought to have some correspondence to fluctuations in those features: the overall neural signal should bear traces (*systematic* ones, hopefully) of changes in, say, heading direction.
>
> A model characterizing the neural representations of such features (location, task phase, reward history) should then be able to "mix and match" said representations until it "fits" onto a representation of the *actual* neural data collected. If we chose to represent recorded data in, say, a 3-D plot, we could "mix and match" feature plots until we get something that "looks like" the plot of our recorded data. Then, increasing (or decreasing) the contribution of individual features, or interactions therein, to the overall model provides a framework for testing what happens to actual neural activity as said features get manipulated in experimental settings.

This sketch is rife with shortcomings: regression (the "mix and match") is prone to overfitting, especially with more features added to the model. Perhaps even more damningly, there is little to guide which form of regression one might prefer - much less whether the features we are regressing over are even relevant in the first place. But, as I wrote above - you gotta start somewhere.  

### Textbook Learning
This week I started self-studing UC Berkeley's Fall '24 offering of CS 189, which is an (intense) introductory course on machine learning principles and popular algorithms. I'm pursuing this path because I'm interested in ML and I think it lays valuable groundwork for pursuing deeper, more formal studies in the theory and application of neural networks. (As you can tell, I still haven't given up on a NN-based DSR approach to model discovery.) This week, all I really did was course setup stuff (like setting up a virtual environment to complete assignments), but next week I hope to start digging into material - and continue learning about nonlinear dynamics, as mentioned in my [first reflection](2024-02-14-reflections.md). 

## Job Search
Last week, I [mentioned](2024-02-21-reflections.md) interest in a technical incidence response internship. This week, I messaged one of the recruiters for that role on LinkedIn, though I have yet to hear back from him. It's possible that internship's applications have already closed, though the job posting makes no mention of start or application close date. Nevertheless, I plan on writing my cover letter, asking for my mentor's colleague's feedback, and submitting my application for the internship this week. 

In general, I need to devote more time to the job search. I truly enjoy the research that I do, but it is not sustainable in the long run without a path to employment. That being said, the same doc candidate that I mentioned above also told me that she was impressed by my work ethic, the questions I'm pursuing, and my analysis skills. She works at the Cleveland Clinic and offered to put me in contact with some of her team leads; "maybe a job opens up over there." Whatever the case, it could be another great experience to develop my research skills. 

## *Sipurei Savta*
Though I didn't record any conversations this week, Savta and I just had a wonderful breakfast together where she told me that one of the things she truly misses about Jerusalem is her time working at the *gan yeladim*, or children's daycare. I think she misses taking care of young children and singing to them. In the past, she would sometimes randomly start singing daycare songs while cooking or cleaning; she doesn't really do that anymore. This week she told me, in a hushed and secretive tone, that she's afraid she's begun to forget things. 

The aging of a loved one is a difficult thing to witness. Nevertheless, I am grateful that I get to do so. 

## Languages
### Hebrew
I finished reading through Yankele Rotblit's ״דברים שרציתי לומר״ ("dvarim sh'ratziti lomar", sung by Yehuda Poliker). I may make another post where I publish my translation of the song - but it's a clunky translation that doesn't do the song justice, so I may not. Unsure. Otherwise, I also began reading through actual news articles in Hebrew. The process is slow, but rewarding.   

### Spanish
No updates this week, again. Oof. 

## Blogging
I started watching a [video essay/Obsidian tutorial](https://youtu.be/hSTy_BInQs8?si=5UQ9ElhsR5ScrQeH) by Odysseas called "Obsidian: The King of Learning Tools (FULL GUIDE + SETUP)" on YouTube. Odysseas makes a compelling case for using Obsidian, even if his delivery style is a bit heavy on the tortured-artist-scholar for my liking. Otherwise, I didn't do anything else to further my technical understanding of how to blog (e.g., learning about Jekyll or HTML).

However, I *did* diligently take some notes throughout the week with the express purpose of devoting my weekend to refleciton activities (like blogging and writing otherwise). I used my notes from this past week to write this reflection post. It seems like a good system to devote my weekends to blogging/writing, since it feels more relaxing and true-to-spirit than trying to get "it" (working out, reading, translating, research, reflections) all in, everyday. 

---
[^1]: Swanson, R. A., Chinigò, E., Levenstein, D., Vöröslakos, M., Mousavi, N., Wang, X.-J., Basu, J., & Buzsáki, G. (2025). Topography of putative bi-directional interaction between hippocampal sharp-wave ripples and neocortical slow oscillations. Neuron. https://doi.org/10.1016/j.neuron.2024.12.019 
[^2]: 
[^3]: 
