---
layout: posts
title:  "HW9: Chapter 8 and reflections on testing"
---
#### 8.7: Write a scenario that could be used to help design tests for the wilderness weather station system.
Context: According to Chapter 7, Design and Implementation, the wilderness weather station system is a station deployed in a remote area. It records local weather information and periodically transfers this to a weather information system using a satellite link.

Scenario: Alex is a local weatherman in small-town North Dakota. Although his home town is small, it's surrounded by even more remote communities which use the wilderness weather system to transmit weather data to aggregators and reporters. 

Alex is putting together a weekly report in which he includes the forecast for not only his town but also the surrounding areas. His home town's data automatically syncs to a weather information system. In order to manage all of the weather data he needs in this report in one place, he puts in a request to the satellite (SatComms) of the wilderness weather system for data from Area1. The weather is then reported to the weather station and once a summary is retrieved, it's summarized into the requested report and returned to the weather information system/database. With the data from the remote areas now synced to the general weather information system, Alex can effectively plan for his presentation by creating graphics and charts and analyzing the data.

#### 8.10: A common approach to the system testing is to test the system until the testing budget is exhausted and then deliver the system to the customers. Discuss the ethics of this approach for systems that are delivered to external customers.

#### Reflections on readings:

