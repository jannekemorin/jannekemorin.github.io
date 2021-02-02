---
layout: posts
title:  "This bugs me"
---
## 6.4. Exercise - Find the Oldest Bug
**Find the oldest bug that's still open in your chosen project. Write a blog entry describing the problem, with a theory about why the bug hasn't been resolved yet. (Bonus points if you can actually resolve the bug.)**

The oldest open Zulip Github issue is titled ["Replace memcached with redis"](https://github.com/zulip/zulip/issues/16). It was opened on September 25, 2015, so it's been open for more than five years. I believe what has kept this issue open for so long is that it's more of an improvement than it is a bug. 

Some users would like to change the Django caching type from Memcached to Redis. The idea is that this would trim Zulip's runtime by removing an extra remote cache and Zulip's installation dependency. 

In June 2017, a [pull request](https://github.com/zulip/zulip/pull/5224) that aimed to resolve this issue was created. However, the leader of the Zulip community, Tim Abbott, commented on this request that "[he is] much more interested in an implementation that makes this an option (so we can offer a sane migration path) than something that just flips this over." 


## 6.5. Exercise - Create Your Bug Tracker Account
**Figure out how to create a new account on the bug tracker of your chosen project. You'll need that account very soon.**

My chosen project, Zulip, does not seem to have a bug tracker outside of github.com, which I already have an account on, of course. Specifically, they use [Github Issues](https://github.com/zulip/zulip/issues) for bug tracking.

## 6.6.1. Exercise - Reproduce a Bug
**Go through your project's bug tracker and find a bug that you think you might be able to reproduce -- and then try to reproduce it in the latest build. Take careful notes. Report your experiences as a comment to the bug. If you can reproduce the bug, great! Give as much information as you can. If you can't reproduce the bug, great! Give as much information as you can, and ask the original reporter if there are other steps you might be able to take to reproduce the bug.**

## 6.7.1. Exercise - Bug Triage
**Find five bug reports in the new state, and attempt to triage them according to the rules above. Your goal is to do as much as you possibly can, in a short period of time, to make those bug reports as useful as possible to the developer to whom they are assigned. (Note: be sure to follow any triage rules that your project may have defined. If there are no set triage rules, be sure to announce your intentions on the project's mailing list, so that developers can provide you some guidelines if they choose.)**
