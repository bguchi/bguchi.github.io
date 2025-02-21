---
title: "Reflections: 2.10-2.14"
date: 2024-02-14
---
# Summary
This week saw a lot of great progress at the lab and the beginning of working on song translations with Savta. It is also the second full week of walking Louie and Bernie (🐶) with my parents everyday, the second week of cooking Shabbat dinner with Savta, and my first real day of blogging. 🤭 

## HivE Research
On Monday, I gave a presentation on my work relating to reproducing some figures in Dr. Hyman's 2017 paper[^1]. I was very pleased; whereas the first such presentation was a paper overview, this presentation was all about my approach to actually scripting a reproduction of Fig. 2A - and an RA even told me I had made "coding look fun" for him, 🫂. Otherwise, I began long-awaited work on MATLAB related to my dynamic systems reconstruction (DSR) project.  
  
### Projects
**Reproductions.** I sent an email to two RAs with the hopes of beginning working together towards postering at UNLV's [OURS research fair](https://www.unlv.edu/our/research-symposia) in May. There are a number of [student resources](https://www.unlv.edu/our/rsa) available for becoming acquainted with research and research communication; it might be a good idea to go to some events, like the OURS information session and poster making workshop, together. (I know the latter would certainly be useful for me, as someone with no postering experience - thus far.) Our actual work together would be relatively straightforward. More on that in a different post, perhaps. 

**DSR.** After months of lightly working through papers and textbooks on reconstructing dynamic systems from neural data, I finally got my hands on using neural networks in MATLAB. The tutorial, in my opinion, was kinda lame; it provided little in terms of learning about neural networks. But it was a good first exposure to how MATLAB encourages using their Deep Learning objects, something I imagine I will do much more of as I get deeper (no pun intended) in my DSR project with Dr. Hyman. 

On that note, Dr. Hyman shared an exciting update on some preliminary data analyses he was running on the `3portdata` used for both his 2017 paper and the lab's 2024 paper[^2]. After running PCA on all-session, all-site neural data, the resulting 3D plot rendered an almost ribcage-like progression of averaged, time-stamped neural activity. Interestingly, gross neural activity corresponding to the start of each trial appeared to hug some invisible axis that the visualized data wound itself around, like the vertebra supporting the outward extension of one's ribs. And from these trial starts, data regularly traveled to some region ostensibly representing "right" spatial contexts, and then traveled onward to another region ostensibly representing "left" spatial contexts. Remarkably, though trials are evenly spaced in real time, their start-time representations in the PCA space appear "chunked" - perhaps corresponding to the experimental design setup of right-left trials making up one "super" trial. The current visualization is noisy, but Dr. Hyman hopes that smoothing the data might accentuate these features some more. 

<figure>
    <img src="/assets/week1-ribs.png"
         alt="Albuquerque, New Mexico">
    <figcaption>What I imagine a smoothed plot of the PCA visualization would look like</figcaption>
</figure>

Why is this all relevant to me, exactly? Perhaps a DSR-based approach might provide an alternative proof-of-concept for feature selection (or, in the parlance of DSR, "parameter discovery" - i.e., learning those {physiological} parameters which drive {neural} dynamic activity), in much the same way PCA does. Perhaps, as Dr. Hyman and others[^3] hope, it also provides a way to generate simulated data based off those extracted parameters. In that case, we might be able to simulate neural data where selective features - such as those corresponding to, say, the progression of time in a behavioral task - get "turned off". Such simulated "perturbations" - generalizable to different types of neural data, collected from different behavioral paradigms - would be of immense utility to neuroscience, and science writ large. That's part of why I feel really excited to work on a project about DSR; there's still so much to learn. 
 
### Textbook Learning 
None this week. However, I found another textbook - [Brunton & Kutz's *Data-Driven Science and Engineering: Machine Learning, Dynamical Systems, and Control*](https://www.databookuw.com/) - which looks approachable, well-written, and recent. I may start reading from it soon. Then again, I may not. I'm already reading through [Strogatz's *Nonlinear Dynamics and Chaos*](https://www.stevenstrogatz.com/books/nonlinear-dynamics-and-chaos-with-applications-to-physics-biology-chemistry-and-engineering), and have the best intentions of self-studying UC Berkeley's [Sp'21 offering of CS 182](https://cs182sp21.github.io/), for which I am perusing [Bishop & Bishop's *Deep Learning: Foundations and Concepts*](https://www.bishopbook.com/). I probably shouldn't bother with another textbook - or, if I do, I should re-evaluate which textbooks/courses feel relevant to "keep".

## Job Search 
No active searching on my end this week. 

## Languages
### Hebrew 
This week I finally got to reading through song lyrics (״דברים שרציתי לומר״, *"dvarim sh'ratziti lomar"*, sung by Yehuda Poliker) with Savta. Translating songs together has been a goal of mine for forever. I chose to translate this song in particular because I hope to build towards reading a [*Haaretz* article about its lyricist](https://www.haaretz.co.il/gallery/music/2025-02-12/ty-article-magazine/.premium/00000194-f920-d3a7-a1fc-f96e3a770000), Yankele Rotblit, together. She seemed genuinely interested, too.

### Spanish
No updates this week. However, I'd like to get back into reading my copy of Penguin's parallel text [*Cuentos en español*](https://citylights.com/story-anthologies/new-penguin-parallel-text-ss-in-spanish/). I started it while traveling in Mexico City with Sarah, but I've since put it down. Hopefully I'll have more substantive updates next week. 

## Sipurei Savta 
No updates this week, though I do hope to get back into transcribing and translating soon.  

[^1]: Hyman, J. M., Holroyd, C. B., & Seamans, J. K. (2017). A novel neural prediction error found in anterior cingulate cortex ensembles. Neuron, 95(2). https://doi.org/10.1016/j.neuron.2017.06.021 
[^2]: Wirt, R. A., Soluoku, T. K., Ricci, R. M., Seamans, J. K., & Hyman, J. M. (2024). Temporal information in the anterior cingulate cortex relates to accumulated experiences. Current Biology, 34(13). https://doi.org/10.1016/j.cub.2024.05.045
[^3]: Durstewitz, D., Koppe, G., & Thurm, M. I. (2023). Reconstructing computational system dynamics from neural data with recurrent neural networks. Nature Reviews Neuroscience, 24(11), 693–710. https://doi.org/10.1038/s41583-023-00740-7 
