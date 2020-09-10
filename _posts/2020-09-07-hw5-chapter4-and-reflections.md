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
1. *Withdrawal:* a customer feeds his/her card to the ATM, then indicates the amount of money to withdraw from the account on the user-interface. The ATM checks that it has that amount of money. If it does, it dispenses the money and processes the withdrawal. Otherwise, it calls an administrator. Lastly, it returns the card.
2. *Deposit:* a customer feeds his/her card to the ATM, then selects the option to deposit on the UI. He/she inputs the money into the machine. The machine tallies it up, rejecting any fraudulent or unreadable bills. Then, it processes the deposit in the electronic system.
3. *Multiple transactions:* a customer makes a deposit or withdrawal, then opts to complete another transaction. The machine keeps the card and restarts the transaction selection process. After a certain number of depsoits/withdrawals determined by the bank, the ATM rejects any further transactions and investigates potential fraud.
4. *Cancellations:* a customer is in the middle of completing a transaction, then decides to cancel it. The ATM returns the card and resets to its new customer mode. If the user fails to retrieve the card, the machine swallows it back up so the administrator can call the customer to retrieve it.
5. *Suspicious activity*: a customer would like to withdraw an unusual amount of money (or all of the money in his/her account). The ATM detects this as suspicious and sends a note that the customer should visit the nearest bank to complete this transaction. 



#### Reading Reflections:
This class’s readings dove into the world of requirements engineering. Chapter 4 of the textbook details this topic, outlining a few approaches to engineering requirements for software. According to the Chapter, “the requirements for a system are the descriptions of the services that a system should provide and the constraints on its operation.” Writing requirements is usually one of the first steps in the software engineering process, sometimes occurring before the system has even been approved for development. 

Of course, different teams take different (and often, multiple) approaches to requirements engineering such as ethnography, interviewing, or collecting stories and scenarios. I found the idea of Test Driven Development (TDD) from the article **Test-Driven Development** particularly interesting. The author, Scott, Wambler, explains that the adoption of the technique is not very high, which is probably why I hadn’t heard of it. Nonetheless, this technique is a strong way to think through your requirements prior to writing production code. TDD involves, as the name suggests, writing tests prior to running the functional code that those tests test (wow, that’s a mouthful!). In terms of requirements, TDD seems like an excellent way to identify constraints on your system that may transfer to the requirements. You can also validate your requirements through early testing, checking their consistency (that they don’t conflict) and completeness (that they conform to the constraints of the system/user), then making adjustments accordingly. Incorporating testing into every stage of the software engineering process like TDD promotes prevents potential holes in requirements from falling through the cracks due to our human ability to hold only an average of 7 +/- 2 objects in our short-term memory at a time (**Magical Number 7**). 

Lack of thorough requirements engineering through techniques like TDD naturally creates opportunities for issues when parts of the software do not fit within the constraints of the system. The article **Tire Pressure Monitoring System** provides a few related examples. In **Tire Pressure Monitoring System**, the TPMS system raises privacy concerns due to a lack of cryptographic mechanisms to prevent vehicle tracking. The system was lacking several other security features that should have been included in the requirements such as shielding from eavesdropping, authentication of messages, and simple input validation. The potential for malicious activity due to these missing requirements is so severe that a Senate Bill was passed to protect consumers from security and privacy threats to their motor vehicles (** The research completed in the paper was able to identify these holes through experimentation (**Spy Car Act of 2015**). It seems TDD could have prevented these issues as it would have involved some testing to examine any existing security requirements and engineer new ones. Essentially, this would be similar to that experimentation, but occur earlier in the process so that any insight into missing security features could be incorporated right off the bat. This would greatly reduce the risk of security compromises.
