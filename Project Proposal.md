# CS-353-Project-Reports
# 

![](https://github.com/Seftali/CS-353-Project-Reports/blob/master/Bilkent.jpg)

**CS 353 Project Proposal**

**Maintenance Data Management System - FixItUp**

**Berk Ataç 	-		21200623 - Section 1**

**Eren Ayture	-		21200559 - Section 1**

**Umut Balkan	-		21401911 - Section 1**

**Derviş Mehmed Barutcu -	21302589 - Section 1**



# 1.Project Description

In this project, we are going to design a database for maintenance department of a company. We have customers, employees, technical staff, products, categories, complaints, repairments, and so on. Customers should be able to file a request for repairments of their products. Whole process should be kept track of to monitor progress in each step. Customers can also file a complaint about products. Such complaints should be handled by customer services. Conversation between customers and employees should also be recorded.


# 2.Funtional and Non-Funtional Requirements

2.1Functional Requirements

In this section, the functional requirements will be mentioned. They are filing a request for the repairment of their product, filing a complaint about product, suggestions, monitoring the processes and chatting mechanism. All these functions can happen after they login to the system.

**File a Request for Repairment** After they log in to the website, they can request a repairment of their products. When they request a repairment, the system skips the related page of the website. Their information such as name and the product or products that they have, will be automatically pasted to relative parts but they also should fill some parts. They must select the product that they will request a repairment then the system shows the related information about that product like the name of the product, brand, model, specifications and the date of purchase. According to the date of purchase, if that product has a guarantee or not will be shown. After they select the product, they must enter the problem with the product. This information will help the relevant departments and the process will be faster. After they fill the problem section, they can send a request for that device.


**File a Complaint** When they want to complain about the product, they need to click the relative button. The system will load the required page. As happen in file a request for repairment system, some of the information will be automatically loaded. Then they should select the product that they will complain about and fill the extra information on why they have complaints about the product. After they finish filling the information, they can send complaints.


**Suggestion** After they file a complaint about the product, the system shows some of the frequently asked questions and their answers are given by the company. If it will help them to solve their problems, they can withdraw their complaints but if they do not find a solution, they do not need to do anything.


**Monitoring the processes** They can monitor the processes that they have requested. The system will show the ongoing processes in the main page. However, it will be just a summary of the process or processes. If they want to see more detailed information about their request for repairment or complaints, they can click the processes button to pass the process page to see all their processes in detailed.


**Chatting mechanism** After they complain about their product, if it is necessary, the customer services will send a message to the user to start a conversation. This chatting will be recorded at the database and will be secure. The customer can talk through the system and complain more about the product. At the same time, the customer services will ask questions more about their problem to understand and give better service and make suggests about to get rid of their problems if it is possible. This will be live and when they finish talking, customer services click to the finish button to commit the conversation to the database.

2.2 Non-Functional Requirements

**Security**
	There will be personal information and conversations between the users and the customer service, therefore the system must secure. No personal information will be shared with a third party.

**Platforms**
	The users of the FixItUp can reach the system from various devices like IOS, Android devices, and desktop, etc. Since the users of the system can reach from different platforms to their profiles and information, we keep their data in a database. 
  
**Usability**
	The age spectrum of the users can be wide so the interface of the system should be easy to understand and use. The instructions must be clear so that the users can understand. Therefore, FixItUp will be user-friendly and appealing.
  The database will be an essential part of storage and also search and retrieve operations of FixItUp. The database will have certain levels and views for each type of user. For example, customers cannot alter the information about products, repairs, categories, etc. However, they can view those information.

**Performance**
	Logging in to our system will not take more than 5 seconds. Our database design will be efficient and well designed. It needs to provide users with the best experience possible without any performance issues. Redundancy and any type of inconsistency will be avoided.  Furthermore, the database is also needed to create a multi-user application that has online features like requesting a service or file a complaint.


** **

#  3. E/R Diagram


![](https://github.com/Seftali/CS-353-Project-Reports/blob/master/ERdiagram.jpg)


complaints(complaintID, content, date)

CustomerServices(ServiceID)

Employees(EmployeeID, name, email, phone)

Conversation(convID, content, date)

TechStaff(StaffID)

Customer(customerID, name, email, address)

Category(categoryName)

Products(productID, name)

Repairments(repID, Status)

has(complaintID, convID)

handle(complaintID, ServiceID)

about(complaintID,productID)

file(complaintID, customerID)

belong(categoryName, productsID)

have(productID, customerID)

Request(customerID, repID)

manage(StaffID, repID)

repair(productID, repID)

# 4.Resources

[https://www.draw.io/](https://www.draw.io/)

