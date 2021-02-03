---
layout: posts
title:  "This bugs me"
---
## 6.4. Exercise - Find the Oldest Bug
**Find the oldest bug that's still open in your chosen project. Write a blog entry describing the problem, with a theory about why the bug hasn't been resolved yet. (Bonus points if you can actually resolve the bug.)**

My team is working on an open-source project called Zulip. The oldest open Zulip Github issue is titled ["Replace memcached with redis"](https://github.com/zulip/zulip/issues/16). It was opened on September 25, 2015, so it's been open for more than five years. I believe what has kept this issue open for so long is that it's more of an improvement than it is a bug, so the priority has always been low. 

Some users would like to change the Django caching type from Memcached to Redis. The idea is that this would trim Zulip's runtime by removing an extra remote cache and Zulip's installation dependency. 

In June 2017, a [pull request](https://github.com/zulip/zulip/pull/5224) that aimed to resolve this issue was created. However, the leader of the Zulip community, Tim Abbott, commented on this request that "[he is] much more interested in an implementation that makes this an option (so we can offer a sane migration path) than something that just flips this over." I think the nature of this issue is such that most people who would want to work on it would be so passionate about it that they'd want it implemented fully, not added as an option. Hence, the issue was set aside when this pull request that flipped the caching type completely to Redis was rejected.


## 6.5. Exercise - Create Your Bug Tracker Account
**Figure out how to create a new account on the bug tracker of your chosen project. You'll need that account very soon.**

My chosen project, Zulip, does not seem to have a bug tracker outside of github.com, which I already have an account on, of course. Specifically, they use [Github Issues](https://github.com/zulip/zulip/issues) for bug tracking.


## 6.6.1. Exercise - Reproduce a Bug
**Go through your project's bug tracker and find a bug that you think you might be able to reproduce -- and then try to reproduce it in the latest build. Take careful notes. Report your experiences as a comment to the bug. If you can reproduce the bug, great! Give as much information as you can. If you can't reproduce the bug, great! Give as much information as you can, and ask the original reporter if there are other steps you might be able to take to reproduce the bug.**

For this exercise, I decided to try to reproduce a bug that I identified as a potential issue for my team to fix. We wrote a bit about the initial triage of this bug on our [team wiki](https://github.com/CSCI-462-02-2021/404-Name-Not-Found/wiki/Ideas-for-Contributing-to-Project). Essentially, this bug does not capture filters when the search term precedes them in the search query. See the images below in my reproduction of this bug in the development environment: 

![](https://github.com/jannekemorin/jannekemorin.github.io/blob/master/assets/images/autocomplete.png)

![](https://github.com/jannekemorin/jannekemorin.github.io/blob/master/assets/images/autocomplete.png)

The first image displays the behavior of Zulip in the handled case - when the search filter precedes the search term "research". It auto-suggests "Desdemona" as a sender. The second image displays its behavior in the unhandled exception. That is, when the search term "research" is typed in before the filter for the sender, the search does not autosuggest "Desdemona" when we begin to type it. It fails to recognize "sender:" as a filter. I tested this with several other search terms and types of filters to come to the same conclusion. Reproducing this bug was the first step to working on resolving it. This was a great exercise to get me started on my first bug fix!


## 6.7.1. Exercise - Bug Triage
**Find five bug reports in the new state, and attempt to triage them according to the rules above. Your goal is to do as much as you possibly can, in a short period of time, to make those bug reports as useful as possible to the developer to whom they are assigned. (Note: be sure to follow any triage rules that your project may have defined. If there are no set triage rules, be sure to announce your intentions on the project's mailing list, so that developers can provide you some guidelines if they choose.)**

This was the trickiest exercise of all. I wasn't able to find any project-specific triaging guide, though I'd be interested to see if any other teams working on Zulip did. The TOS chapter defines five steps to triaging:
1. Letting the user know that someone has looked at it
2. Looking for other similar bugs
3. Guaranteeing proper severity and/or priority
4. Ensuring that the bug is sensible and helpful to developers
5. Ensuring that the bug is filed against the correct component, with the correct version

I  looked through some bugs in the new state and did not feel comfortable completing these steps without being able to locate the triage rules for Zulip. It seems the main contributor and leader of the project, Tim Abbott, is typically the first to jump in on issues. He is usually quick to respond, so these few bugs in the new state are recent. Nonetheless, it was useful to learn about general triage steps as this is software engineering concept is new to me.

