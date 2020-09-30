---
layout: posts
title:  "HW9: Chapter 8 and reflections on testing"
---
#### 8.7: Write a scenario that could be used to help design tests for the wilderness weather station system.
Context: According to Chapter 7, Design and Implementation, the wilderness weather station system is a station deployed in a remote area. It records local weather information and periodically transfers this to a weather information system using a satellite link.

Scenario: Alex is a local weatherman in small-town North Dakota. Although his home town is small, it's surrounded by even more remote communities which use the wilderness weather system to transmit weather data to aggregators and reporters. Alex is putting together a weekly report in which he includes the forecast for not only his town but also the surrounding areas. His home town's data automatically syncs to a weather information system. However, in order to manage all of the up-to-date weather data he needs in this report in one place, he puts in a request to the satellite (SatComms) of the wilderness weather system for data from Area1. The weather is then reported to the weather station and once a summary is retrieved, it's summarized into the requested report and returned to the weather information system/database. With the data from the remote areas now synced to the general weather information system, Alex can effectively plan for his presentation by creating graphics and charts and analyzing the data. He repeats this process for Area2 and Area3 through separate requests to the satellite.

#### 8.10: A common approach to the system testing is to test the system until the testing budget is exhausted and then deliver the system to the customers. Discuss the ethics of this approach for systems that are delivered to external customers.

I do not think that this is an ethical system. The scenario implies a lack of planning by the testing team to create a comprehensive test-suite within the budget. Particularly because this is a system that will be delivered to an external customer, it's crucial that testing within the budget is maximized. I think it's important here to distinguish between the case that the system was tested until the budget ran out according to plan and the case that the system was tested until the budget ran out wihout covering all of the planned (comprehensive test cases). If this testing strategy resulted in major holes in testing, it would certainly not be an ethical use of the client's money. For example, say features were tested separately and sequentially so that testing the last few was cut out with the budget loss. It would be more ethical to test each feature to a lesser degree. If it isn't possible to test every feature sufficiently within the budget, this should be communicated to the customer as early as possible.

#### Reflections on readings:

