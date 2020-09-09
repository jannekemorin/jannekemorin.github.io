---
layout: posts
title:  "HW5: Chapter 4 and reflections"
---
#### 4.5: Using the technique suggested here, where natural language descriptions are presented in a standard format, write plausible user requirements for the following functions:
#### An unattended petrol (gas) pump system that includes a credit card reader. The customer swipes the card through the reader, then specifies the amount of fuel required. The fuel is delivered and customer's account debited.
1. The petrol pump system shall charge the customer's account the correct amount of money based on the amount of fuel specified.
2. The petrol pump system shall provide secure credit card processing.
3. The petrol pump system shall provide the customer with a record of their transaction (through a receipt).
4. The petrol pump system shall implement mechanisms to ensure safe fuel delivery.
5. The petrol pump system shall deliver the smaller of the amount of fuel specified and the amount of fuel to fill the tank.

#### The cash-dispensing function in a bank ATM.
1. The cash-dispensing function shall keep track of the amount of cash available.
2. The cash-dispensing function shall ensure the ATM stays stocked with cash by notifying the administrator when cash is low.
3. The cash-dispensing function shall keep bills neat and organized for quick delivery.
4. The cash-dispensing function shall integrate with existing bank software to verify the user's accounts.
5. The cash-dispensing function shall detect and report suspected fraudulent activity.

#### In an Internet banking system, a facility that allows customers to transfer funds from one account held with the bank to another account with the same bank.
1. The Internet banking system shall prevent transfers that would result in negative account balances.
2. The Internet banking system shall limit the number of transfers allowed per customer per month.
3. The Internet banking system shall allow customers to schedule transfers.
4. The Internet banking system shall allow customers to set up recurring transfers.
5. The Internet banking system shall allow customers to document their transfers through notes.


#### 4.6 Suggest how an engineer responsible for drawing up a system requirements specification might keep track of the relationships between functional and non-functional requirements.
According to Chapter 4, Requirements Engineering, functional requirements describe what the system should do while non-functional requirements specify or constrain characteristics of the system. After thinking about this a bit, it seems like each non-functional requirement should be mapped to at least one functional requirement that it specifies. Many non-functional requirements will support multiple functional requirements. Hence, I would suggest that an engineer uses software like AirTable or Notion that can create complex tables for keeping track of relationships between items. For example, if a row in the table is taken as a non-functional requirement, a multi-select column could allow the user to input all of the functional requirements it supports. This way, using the sorting and filtering functions of the software (AirTable or Notion), the engineer could easily display all non-functional requirements that support a certain requirement or all functional requirements supported by a non-functional requirement. This would also provide several other "views" such as a Kanban board that the engineer could use to visualize the requirements as a whole.


#### 4.7 Using your knowledge of how an ATM is used, develop a set of use cases that could serve as a basis for understanding the requirements for an ATM system.


#### Reading Reflections:
