---
layout: posts
title:  "HW17: Team Progress I"
---
This is my first reflection on our team's testing project. I think this will be a helpful exercise as we move into the final stages of building our testing framework.

So far, I think our team has worked very well together! After deliverable 2, we loosely assigned parts of the framework (the parser, the driver, and the reporting mechanism) to each person. Between deliverable 2 and deliverable 3, we met several times to discuss what still needed to done and any issues that arose.  Justin did an *excellent* job creating a parser that converts test cases from .json files to test case objects that we execute. I am still so in awe of how it works! Matt is our selenium expert who has been creating the test cases and their driver. 

My role was to determine how we could print the results of our tests to a .html file that automatically opens. I struggled with this a bit because implementing and testing the reporting mechanism depended so much on the parser and driver. I was able to research packages and decide on one early on (HTML Test Runner), but it wasn't until this week that I could actually add it to the program and play around with it. This was a good learning experience - in the future I will definitely get more involved in the requirements for my piece if I need them ready earlier.

That said, one of the major points of improvement for our current framework is the test report. I need to spend time making it more verbose, displaying the inputs, outputs, requirements, run time, success, etc. of each test. Currently, it just displays the name of the test and a pass/fail measure. I'll have to look further into the docs of HTML Test Runner and probably create a template for the report to work from.

Additional areas of improvement and research include:
* The structure of TestAutomation - making sure it follows the specification document.
* The memory requirements if we were to ramp up the number of tests.
* Documentation! This month, I am going to make sure we have solid documentation that covers all of the bases and concurs in every outlet (the Wiki, the final report, readmes, etc.).

I'm looking forward to putting together the final pieces of this project through deliverables 4 and 5, the final reports, and the presentation which showcases our work. Overall, I'm proud of how our team has worked together!



