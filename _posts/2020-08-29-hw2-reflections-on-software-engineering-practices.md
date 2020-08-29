---
layout: posts
title:  "HW2: Reflections on software engineering practices"
---
#### The Complexity of Software and Its Evolution
Software is, by definition, complex. Frederick P Brooks, in his article "Essence and Accidents of Software Engineering," describes the essence of a software entity as "a construct of interlocking concepts: data sets, relationships among data items, algorithms, and invocations of functions." 

This week's readings reminded me of the sheer amount of moving pieces that drive software and how this complexity connects to its other characteristics. For instance, a constant need to change. Each "interlocking concept" evolves in its own right; the software has to keep up to keep from breaking. This comes with complications because when a change is made, all of the dependencies have to be considered. For instance, if a developer adds new columns to a database, each file referencing that database should be reworked. Naturally, it becomes dangerous to merge personal changes against code that's not up-to-date. In his article, "Cherry-Picking and the Scientific Method," George V. Neville-Neil, writes that “the real work” is periodically merging whatever code we are working against. If we keep the tip of the git, as he calls it, from straying too far without our work, we can prevent a lot of unnecessary trouble reworking it to accomodate the latest version.


#### Lessons from Google: Productivity, Reliability, and Simplicity
I first read these three words mentioned together in "Essence and Accidents of Software Engineering." The author suggests that the antitheses of these create software costs, thereby suggesting that we should strive for productivity, reliability, and simplicity as software engineers. 

While reading about Google's codebase systems in the article"Why Google Stores Billions of Lines of Code in a Single Repository" by Rachel Potvin and Josh Levenberg, I kept these attributes on my mind. What better company to analyze for lessons on successful software practices?

The first characteristic I noticed in Google's systems was simplicity. According to the article, Google stores one billion files, a history of approximately 35 million commits, and 86TBs of data in a monolithic repository. I was shocked by this! The single repository is by no means small, which prevents its own challenges, but its monolithic natures allows for simpler tooling with just one system of reference.

Google also implements a number of systems to support code reliability. Particularly, they've implemented sophisticated automated testing which covers each dependency impacted by the change at hand. They have also the automated reversal of the unlikely changes that do cause breakage. As Neville-Neil writes in "Cherry-Picking...," "no part of working on software should be based on gut feelings, because, after all, software is supposed to be a part of computer science, and science demands proof." Google's automated testing work to "prove" the safety of each change, maintaining the reliability of a codebase worked on by thousands of developers on a daily basis.

The third and final attribute, productivity, is primarily supported by Piper and CitC architectures. These tools allow the developers to work on a such a large database as the Google repository through their own synced local "workspace." By only storing modified files, workspaces consume a relatively small amount of storage while giving developers quick access to anything they need from the distributed cloud repository. Through the trunk-based development model, engineers work from the most recent version of the code, making changes through "single, serial ordering." 
