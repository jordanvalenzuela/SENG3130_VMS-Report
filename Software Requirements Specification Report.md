# Software Requirements Specification for Volunteer Management System
### Version 1.0 Approved
### Prepared by Jordan Valenzuela, Kyle McKee, Marium Tawhid
### Thompson Rivers University
### November 28 2022

### Table of Contents
**Revision History** xiii

1.	[**INTRODUCTION**](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/Software%20Requirements%20Specification%20Report.md#1-introduction)	1\
1.1	[Purpose](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/Software%20Requirements%20Specification%20Report.md#11-purpose)	1\
1.2	[Document Conventions](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/Software%20Requirements%20Specification%20Report.md#12-document-conventions)	1\
1.3	[Intended Audience and Reading Suggestions]()	1\
1.4	[Product Scope]()	1\
1.5	[References]()	1
2.	[**OVERALL DESCRIPTION**]() 1\
2.1	[Product Perspective]()	1\
2.2	[Product Functions]()	2\
2.3 [User Classes and Characteristics]() 2\
2.4 [Operating Environment]() 3  
2.5 [Design and Implementation Constraints]() 3\
2.6 [User Documentation]() 3\
2.7 [Assumptions and Dependencies]() 3
3.	[**EXTERNAL INTERFACE REQUIREMENTS**]()	3\
3.1	[User Interfaces]()	3\
3.2	[Hardware Interfaces]()	3\
3.3  [Software Interfaces]() 3\
3.4  [Communication Interfaces]() 4\
  3.4.1 [Communications with the end-users]() 4\
  3.4.2 [Communications with the backend servers]() 4
4.	[**SYSTEM FEATURES**]() 4\
 4.1 [Create New Volunteers]() 4\
 4.1.1 [Description and Priority]() 4\
 4.1.2 [Stimulus/Response Sequences]() 4\
 4.1.3 [Functional Requirements]() 4\
 4.2 [Assign Volunteer]() 5\
 4.2.1 [Description and Priority]() 5\
 4.2.2 [Stimulus/Response Sequences]() 5\
 4.2.3 [Functional Requirements]() 5\
 4.3 [Generate a Daily Report]() 5\
 4.3.1 [Description and Priority]() 5\
 4.3.2 [Stimulus/Response Sequences]() 5\
 4.3.3 [Functional Requirements]() 6\
5. [**OTHER NONFUNCTIONAL REQUIREMENTS**]() 6\
 5.1 [Performance Requirements]() 6\
 5.2 [Safety Requirements]() 6\
 5.3 [Security Requirements]() 6\
 5.4 [Software Quality Attributes]() 6\
 5.5 [Business Rules]() 6
6. [**OTHER REQUIREMENTS**]() 7\
Appendix A: [Glossary]() 7\
Appendix B: [Analysis Models]() 7

## Revision History
|Name|Date|Reason for Changes|Version|
|---|---|---|---|
|||||
|||||

## 1 INTRODUCTION
### 1.1 Purpose
The purpose of this SRS is to describe the software requirements specifications for the first version of the Volunteer Management Web application. This application provides a personal management system for personal uses and a service for the general public. This version contains the basic functionalities for users.

This document describes the purpose of the system, the scope of the system, and the system’s features.
### 1.2 Document Conventions
<Any comments inside single brackets such as this are not part of this SRS, but it is to help reader to understand the point being made.>
### 1.3 Intended Audience and Reading Suggestions
This document is written for developers and testers. 
### 1.4 Product Scope
This application provides a personal productivity manager for personal uses. 
It provides the following benefits:
* It has a day-to-day case report for the volunteer administrator
* It scores each day's performance
* It puts each user in a hierarchy of competence with clients
* It defines some benefits to keep user engaged in his/her activities
### 1.5 References
N/A
## 2 OVERALL DESCRIPTION
### 2.1 Product Perspective
A volunteer management system stores the following information:
* Volunteer's basic information (such as full name, date of birth, email, phone number, address, etc.)
* Senior's basic information (full name, age, date of birth, phone number, address, etc.)
* Senior health and social status
* Volunteer login history
* Volunteer activity history
### 2.2 Product Functions
The major features of the volunteer management system as shown in below entity-relationship diagram (ERD)\
<img width="590" alt="Entity_Relationship_Diagram" src="https://user-images.githubusercontent.com/113567393/204615784-f0b61687-0654-41aa-bc97-418525c85adf.PNG">
### 2.3 User Classes and Characteristics
The customer should be able to do the following functions:\
* Create a customer profile
* Update a customer profile
* Delete a customer profile
The employee should have the following management functionalities:\
* CUSTOMER FUNCTIONS
  * Send a request for assistance
* ADMINISTRATIVE
  * View Status Report
  * Send volunteer infor to the BCS
  * Evaluate a volunteer's engagement
### 2.4 Operating Environment
Operating environment for the volunteer management system is as listed below.

* Relational
* Client/Server
* Windows
* Oracle DB
* Dev-C++
### 2.5 Design and Implementation Constraints
1. The volunteer management system must be implemented alongside the police department's background check system
### 2.6 User Documentation
The VMS website provides an insight of its purpose and function for users.\
Help links, FAQs, and a search bar are provided for the user in case of further inquiries.
### 2.7 Assumptions and Dependencies
Refer to the Vision and Scope Document

## 3 External Interface Requirements
### 3.1 User Interfaces
* Front-end software: HTML
* Back-end software: C++
### 3.2 Hardware Interfaces
* Since the application must run over the internet, all the hardware shall require an internet connection
### 3.3 Software Interfaces
|**Software Used**|**Description**|
|---|---|
|Operating System: Windows|Windows was chosen for its broad support and user-friendliness|
|Database: Oracle|Oracle DB was chosen to store user data|
|Platform: Dev-C++|Dev-C++ was chosen for our knowledge of the language|
### 3.4 Communications Interfaces
The system supports all types of web browsers.
#### 3.4.1 Communications with the end-users
Users interact with the system by using any web browser to access the system's URL.
#### 3.4.2 Communications with the backend servers
The system will retrieve a file upon its request from C++ using the HTTP protocol.
## 4 System Features
### 4.1 Create new Volunteers
#### 4.1.1 Description and Priority
The volunteer management system shall allow an approved volunteer to create their profile;
this feature is of High priority. 
#### 4.1.2 Stimulus/Response Sequences
* Once a volunteer has been approved by the volunteer administrator, the system will notify the volunteer using their contact information such as email
* The volunteer shall create an account using their basic information (such as name, date of birth, address, etc.), contact information (i.e. phone number, email address), their chosen account password, and their preferred volunteer work type into the system. The system will store this information and create their profile.
#### 4.1.3 Funcitonal Requirements
    REQ-1: The Volunteer Administrator shall be able to submit an applicant’s information into the system
    REQ-2:	The system shall be able to send the applicant’s information to the Police Background Check System for screening
    REQ-3:	The system shall receive the results of the volunteer background check from the Background Check System
    REQ-4:	The system shall send the results of the volunteer background check to the Volunteer Administrator
    REQ-5:	The volunteer should be able to create an account by entering in their basic information (first name, last name, age, email, etc.) and a unique password once they have been approved by the Volunteer Administrator
    REQ-6:	The volunteer shall be able to log in to their account using their email and password
### 4.2 Assign Volunteer
#### 4.2.1 Description and Priority
The volunteer management system shall allow an approved volunteer to view and select a
senior case or a student case job; this feature is of High priority. 

#### 4.2.2 Stimulus/Response Sequences
* Once a volunteer has created an account, they may view the system’s postings of request for senior assistance or student assistance which may be based on their preferred volunteer work
* Once a volunteer has chosen the job they want to do, the system shall make sure that job cannot be chosen by another volunteer.  In the case of a senior, the system shall notify the SPCC that a volunteer will assist the senior in question.  The system shall allow the volunteer to edit the senior’s health and social status. 
#### 4.2.3 Funcitonal Requirements
    REQ-1:	The SPCC shall be able to make a request for senior assistance in the system
    REQ-2:	The volunteer shall be able to view the list of ongoing requests for assistance
    REQ-3:	The volunteer shall be able to choose from the list of ongoing requests for assistance
    REQ-4:	The system shall be able to send the volunteer’s past volunteering history to the Volunteer Administrator
    REQ-5:	The system shall be able to score the volunteer’s engagement based on their past volunteering history
    REQ-6:	The volunteer administrator shall be able to view the volunteer’s “potential” or “interested” volunteer cases
    REQ-7:	The system shall be able to take an accepted job off the ongoing list of requests for assistance
### 4.3 Generate a Daily Report
#### 4.3.1 Description and Priority
The volunteer management system shall create a report which includes the forecasted number of senior cases for the next week to the volunteer administrator and the Mayor; this feature is of High priority.\

#### 4.3.2 Stimulus/Response Sequences
* Once a volunteer has been approved by the volunteer administrator, the system will notify the volunteer using their contact information such as email
* The volunteer shall create an account using their basic information (such as name, date of birth, address, etc.), contact information (i.e. phone number, email address), their chosen account password, and their preferred volunteer work type into the system. The system will store this information and create their profile. 
#### 4.3.3 Funcitonal Requirements
    REQ-1:	The system shall be able to calculate the number of senior cases for the next week by midnight each day
    REQ-2:	The system shall be able to send a daily case report to the volunteer administrator and the Mayor everyday
## 5 Other Nonfunctional Requirements
### 5.1 Performance Requirements
_NFR-1: The VMS should send requests for assistance in less than 2 seconds._  
_NFR-2: Volunteer approval process should take no more than 3 work days._
### 5.2 Safety Requirements
N/A
### 5.3 Security Requirements
_NFR-1: The system shall not disclose any personal information to unauthorized parties\
NFR-2: The system shall provide a backup of the most recently updated data in the event of unexpected data loss\
NFR-3: Volunteer data shall be updated after the end of each assignment\
NFR-4: The system shall keep volunteer activities for the last two years_
### 5.4 Software Quality Attributes
_NFR-1: 75% of first-time users shall be able to process their account in under 5 minutes\
NFR-2: The VMS shall ask a user to resubmit a form if their entry is invalid\
NFR-3: The VMS should be up and running for 99.5% of work hours\
NFR-4: The VMS should experience no more than 2 failures every year\
NFR-5: The background check system shall process background checks at a rate of 1000 per hour_
### 5.5 Business Rules
Refer to System Features
## 6 Other Requirements
N/A
## Appendix A: Glossary
|**Word/Acronym**|**Description**|
|---|---|
|SPCC|Senior People Care Center|
|BCS|Background Check System|
|System|Refers to the Volunteer Management System|

## Appendix B: Analysis Models
<img width="574" alt="Appendix-Entity_Relationship_Diagram" src="https://user-images.githubusercontent.com/113567393/204623831-198f9468-594b-4997-96af-94957bc6ef41.PNG">

### Table I: Data Dictionary
|**Data Element**|**Description**|**Composition or Data Type**|**Length**|**Values**|
|---|---|---|---|---|
|Request for Assistance|Request for assistance|Request Information <br/> + Requester|-||
|Volunteer Profile||+ Name <br/> + Phone Number <br/> + Age|-||
|Volunteer Name||String alphabet|50||
|Volunteer Password|||20|Numbers and characters (case sensitive)|
|Client Information|Information about the senior and senior case in question|Client Profile <br/> + Name <br/> + Address <br/> + Health/Social Status <br/> + Age|-||
|Client Name||String alphabet <br/> + First Name(s) <br/> + Middle Name <br/> + Last Name|50||
|Client Age||Positive Integer|3|The minimum value is 0, and the maximum value is 200|
|Client Address||+ City <br/> + Street Name <br/> + Street Number <br/> + Unit Number <br/> + Province/Territory <br/> + Country|-||
|Status Report|Daily report sent to the volunteer administrator|Positive integer <br/> Database <br/> + Number of current senior cases <br/> + Number of forecasted cases for the next week|-|The minimum value is 0|
