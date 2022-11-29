# Software Requirements Specification for Volunteer Management System
### Version 1.0 Approved
### Prepared by Jordan Valenzuela, Kyle McKee, Marium Tawhid
### Thompson Rivers University
### November 28 2022

### Table of Contents
**Revision History** xiii

1.	[**INTRODUCTION**]()	1\
1.1	[Purpose]()	1\
1.2	[Document Conventions]()	1\
1.3	[Intended Audience and Reading Suggestions]()	1\
1.4	[Product Scope]()	1\
1.5	[References]()	1
2.	[**Overall Description**]() 1\
2.1	[Product Perspective]()	1\
2.2	[Product Functions]()	2\
2.3 [User Classes and Characteristics]() 2\
2.4 [Operating Environment]() 3  
2.5 [Design and Implementation Constraints]() 3\
2.6 [User Documentation]() 3\
2.7 [Assumptions and Dependencies]() 3
3.	[**External Interface Requirements**]()	3\
3.1	[User Interfaces]()	3\
3.2	[Hardware Interfaces]()	3\
3.3  [Software Interfaces]() 3\
3.4  [Communication Interfaces]() 4\
  3.4.1 [Communications with the end-users]() 4\
  3.4.2 [Communications with the backend servers]() 4
4.	[**SYSTEM FEATURES**]() 4\
 4.1 [Create New Volunteers]() 4\
 4.2 [Assign Volunteer]() 5\
 4.3 [Generate a Daily Report]() 5
5. [**FUNCTIONAL REQUIREMENTS**]() 6\
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
## 2 Overall Description
### 2.1 Product Perspective
A volunteer management system stores the following information:
* Volunteer's basic information (such as full name, date of birth, email, phone number, address, etc.)
* Senior's basic information (full name, age, date of birth, phone number, address, etc.)
* Senior health and social status
* Volunteer login history
* Volunteer activity history
### 2.2 Product Functions
The major features of the volunteer management system as shown in below entity-relationship diagram (ERD)
