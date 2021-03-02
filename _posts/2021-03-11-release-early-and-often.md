---
layout: posts
title:  "Release early and often"
---
Proper documentation for both internal and external users of a software application is crucial to its sustained success after deployment. This week, we read Chapter 8 of our assigned textbook ("Client-centered Software Development") and Chapters 8 and 9 of the "Teaching Open Source" book. These covered how good documentation complements the practice of frequent, early deployment in software development.

One important distinction that these readings make is between user documentation and developer documentation. I actually hadn't really made this distinction in my mind before reading! Documentation is documentation, right? These readings devote equal importance to both types but focus more on best practices for user documentation.

In terms of developer documentation, it's crucial to ensure that developers can understand the most recent changes to the code with each deployment. This will allow them to successfully work with the code, making progress on the project via future changes. Another important impact of good developer documentation is that it allows new developers who join later in the software's lifecycle to gain a working understanding of the existing systems they will alter. Developer documentation can take the form of code comments or other documents. 

Likewise, the user must know how to complete the basic functions of the application as their steps (may) change with each deployment. As users of applications, we expect access to a "help" section with good documentation when we run into issues. Creating this user documentation is no small undertaking, especially because it's dynamic. As the application changes frequently, the user documentation will need to keep up the pace.

The chapter "Preparing to Deploy" from our textbook outlined the importance of writing for the audience of your application. Sometimes this audience will be specific enough that you can cater to them in your writing. However, I learned through reading that it's important to assume a broader, more diverse audience when creating user documentation. You should assume that people with English as a second language will read it. Taking this into account could range from sticking to simplified English (1,000 words, each with just one meaning) to having your writing translated to numerous languages.

The audience of a software application is diverse in more ways than nationality. Some users will prefer text while others will prefer pictures - include both. Some users won't understand metaphors or humor - be literal. Some users can't consume large amounts of text at once - keep it to a minimum. The reading outlines a list of additional tips that improve readability for everyone including being concise, precise, and direct. 

Dr. Bowring mentioned the possibility of writing or improving documentation as one of our contributions for the semester project (Zulip). An opportunity recently arose for me to do this. I submitted a pull request that failed due to a test conflicting with my new code. The head of the project suggested that I rewrite the test case to accommodate my code. Of course, this change would need to be well documented. Having learned about how to write documentation that will best serve the internal and external users of an application, I feel well-equipped to work on this!
