---
title: "Reflections: 2.17-2.21"
date: 2024-02-21
---
# Summary 
Research was pretty unremarkable this week. Otherwise, I was pointed towards a job opening by a mentor's colleague, and spent more time practicing Hebrew, reading, and looking into blogging stuff. I also started journaling again and listened to an interesting [podcast](https://www.npr.org/2025/01/24/1226561694/ted-radio-hour-future-of-memory-technology) about "synthetic memories".  

## HivE Research
This week Dr. Hyman and I met a number of times to discuss something like symbolic regression for model discovery. In so doing, he recommended I put away DSR. I also started mentoring an RA for the reproductions project I've been working on. 

### Projects
**Reproductions.** I officially on-boarded an RA - the same who had mentioned that my earlier presentation on reproducing some of the 2017 Hyman et al.[^1] paper made him realize coding "could be fun" - for the reproductions project I've been working on since around November. We have ~1.5 months until submission to [OURS](https://www.unlv.edu/our/research-symposia); until then, he'll spend time learning about MATLAB fundamentals and my approach to reproducing Fig. 2A. (Hopefully, he'll also come up with a working approach of his own.) He seems excited to do this work, and I'm excited to mentor an RA through their introduction to computing in neuroscience.  

**DSR.** I can't lie, I was (am?) pretty bummed about the suggestion to leave DSR to the wayside for now. It's not that I don't agree -- I *did* feel way in over my head, what with my limited background in the formalism required to *really* understand engineering neural networks for the purposes of DSR. I guess I feel sad because it's something I've spent a long time (*read:* months, since November) thinking about, and I've grown attached to the promises of data-driven model discovery; and also because it feels like I have to "give up" on DSR because I'm not capable enough to make meaningful progress on it in the time I have left at the lab. I still intend to learn about ANNs/ML and dynamical systems fundamentals, because I think it's interesting and useful for the future work I intend to do. 

**???.** I'm not sure what to call this project just yet. It emerged as an off-shoot of a DSR-style take on some preliminary data analysis Dr. Hyman did last week, but it feels quite different in approach. The biggest difference, in my opinion, is ???'s top-down approach to model creation: whereas NN-based DSR seems to (rather) successfully infer a dynamic system's "signatures" (such as its overall geometry) through "translating"[^2] the configuration of a trained NN into the "language" of DSs, ???'s approach requires *first* defining a family of models from which to compare actual data against data *then* generated under particular models of choice. In this way, ??? is reminiscent of the class of "symbolic regressors" (like SINDy[^3]) approach to DSR. An immediate criticism of this approach, while yielding highly interpretable descritpions of the data-generating system being studied, is its "bias" induced by the researcher-defined choice of models upon which regression is done - not to mention the possibility that the system being studied might not be expressible in terms of such models[^4]. As the authors of the cited literature put it, the "bias" is like trying to fit an exponential with a polynomial: in a certain sense, it can be done - but, troublingly, we'd be grasping at the wrong straws. Despite these shortcomings, I'd like to look into this project some more. 

### Textbook Learning
None this week, again. Oof. 

## Job Search
A colleague of my mentor's 

## *Sipurei Savta*
## Languages
### Hebrew
### Spanish
## Blogging

[^1]:
[^2]: Monfared, Z. & Durstewitz, D.. (2020). Transformation of ReLU-based recurrent neural networks from discrete-time to continuous-time. *Proceedings of the 37th International Conference on Machine Learning*, in *Proceedings of Machine Learning Research* 119:6999-7009. Available from https://proceedings.mlr.press/v119/monfared20a.html
[^3]: Brunton, S. L., Proctor, J. L., & Kutz, J. N. (2016). Discovering governing equations from data by sparse identification of nonlinear dynamical systems. Proceedings of the National Academy of Sciences, 113(15), 3932–3937. https://doi.org/10.1073/pnas.1517384113 
[^4]: Durstewitz, D., Koppe, G. & Thurm, M.I. Reconstructing computational system dynamics from neural data with recurrent neural networks. Nat. Rev. Neurosci. 24, 693–710 (2023). https://doi.org/10.1038/s41583-023-00740-7
