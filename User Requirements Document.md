# USER REQUIREMENTS DOCUMENT FOR VOLUNTEER MANAGEMENT SYSTEM OF THE CITY
##### Version 0.1 
##### OCT 2022
## Project Identification
Project Name: Implementation of Volunteer Management System for the City\
Date: 17/10/2022
||Project Owner: |Business Analyst: |
|---|---|---|
|Post/Rank|| |

## Revision History
|Revision No. |Date|Pages/Section Revised|Remarks|
|-----|----|------------------|-------|
|1    |17/10/2022|                  |       |
|     |    |                  |       |

## Distribution List
|Name|Post/Rank|B/D|Date|
|-----|----|------------------|-------|
|    ||                  |       |
|     |    |                  |       |
|    ||                  |       |
|     |    |                  |       |

### Table of Contents
**Project Identification**\
Revision History	2\
Distribution List	2

1.	[**INTRODUCTION**](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#1-introduction)	5\
1.1.	[PURPOSE](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#11-purpose)	5\
1.2.	[PROJECT BACKGROUND](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#12-project-background)	5\
1.3.	[BUSINESS OBJECTIVES](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#13-business-objectives)	5\
1.4.	[PROJECT SCOPE](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#14-project-scope)	5\
1.5.	PROJECT OBJECTIVES	5
2.	**IDENTIFIED RISKS AND ASSUMPTIONS** 6\
2.1.	Identified Risks	6\
2.2.	Assumptions	7
3.	**PROPOSED SYSTEM OVERVIEW**	7\
3.1.	DESCRIPTION OF PROPOSED VOLUNTEER MANAGEMENT SYSTEM	7\
3.2.	SYSTEM USER PROFILE	8
4.	**FUTURE BUSINESS PROCESS** 9\
 4.1 LIST OF FUTURE BUSINESS PROCESS 9\
 4.2 BP001-CREATION OF NEW VOLUNTEER 9\
 4.2.1 PROCESS DESCRIPTION FOR CREATION OF NEW VOLUNTEER RECORD 9
5. **FUNCTIONAL REQUIREMENTS** 10\
 5.1 LIST OF FUNCTIONAL REQUIREMENTS 10\
 5.2 REQ-CRE-000 CREATION OF NEW VOLUNTEER 10
6. **NON-FUNCTIONAL REQUIREMENTS** 11\
 6.1 LIST OF NON-FUNCTIONAL REQUIREMENTS 11\
 6.2 AUDIT, CONTROL, & SECURITY REQUIREMENTS 12\
  6.2.1 REQ-ASC1 System Audit 12\
  6.2.2 REQ-ASC2 System Control 12\
  6.2.3 REQ-ASC3 System Security 13\
  6.2.4 REQ-ASC4 Backup and Recovery Requirements 13\
  6.2.5 REQ-ASC5 Disaster Recovery Requirements 14\
  6.2.6 REQ-ASC6 Privacy Requirements 14\
 6.3 DATA REQUIREMENTS 15\
 6.3.1 REQ-DAR1 Global Data Requirements 15\
 6.3.2 REQ-DAR2 Key Data Requirements 15\
 6.4 USABILITY REQUIREMENTS 16\
 6.4.1 REQ-USR1 General Usability Requirements 16\
 6.5 SERVICE LEVEL TARGETS 16\
 6.5.1 REQ-SLT1 System Availability 16   
 6.5.2 REQ-SLT2 System Performance 17\
 6.6 DATA GROWTH AND RETENTION REQUIREMENTS 17\
 6.6.1 REQ-DGR1 Data Growth and Retention Requirements 17
 7. **SYSTEM IMPLEMENTATION CONSIDERATION** 18\
## 1 Introduction
### 1.1 PURPOSE
This document defines the user requirements for the new Volunteer Management System for the city.  The information stated in this document will be used as the basis for subsequent development activities including design, implementation, testing, and post-implementation review.
### 1.2 PROJECT BACKGROUND
Since the COVID pandemic, daily care workers for seniors have significantly dropped.  It is estimated that there are 10000 to 15000 senior cases that the city needs to attend to; however, with the lack of workers, as well as the limited speed of the current system, the city is unable to meet the demands fast enough. As well, due to the limited number of teachers, there is a demand in the elementary school system for additional coaching and teaching for the students. At the moment, a lot of time is spent screening potential volunteers, and there is a lack of incentives for volunteers to contribute their time.  While people are recovering from the pandemic, we should be able to support children and seniors alike with the help of qualified volunteers.
### 1.3 BUSINESS OBJECTIVES
The high-level business objectives for the project are the following:
1. Reduce the application process time
2. Develop a centralized system that accurately keeps track of seniors
3. reduce volunteer assignment time by 30% (Seniors should get volunteer services within three days)
### 1.4 PROJECT SCOPE
The new VMS aims to provide volunteer support to seniors in need of assistance and elementary school children further tutoring.  

The major functions to be provided by the system are listed below:\
a) Creation, updating, and deletion of volunteer and senior profiles\
b) Approve volunteer applications for service\
c) Generate daily reports of a forecasted number of senior cases for the next week
### 1.5 PROJECT OBJECTIVES
The project objectives are to\
a) Decrease the number of senior cases in the city\
b) Decrease volunteer assignment time by 30%
## 2 IDENTIFIED RISKS AND ASSUMPTIONS
The following are the identified risks, assumptions, and constraints related to requirements collected at this stage from the business users and/or the stakeholders involved.\
### 2.1 IDENTIFIED RISKS
The list of identified risks for the project is shown below:\

Table I - Identified Risks Related to Requirements
|No.|Risk Description|Likelihood (High/Medium/Low/Rare)|Impact Description (Cost, Schedule,Scope, Quality, or Others)|Risk Rating|Possible Resolutions & Mitigations|Risk Owner|
|---|---|---|---|---|---|---|
|1.|The senior may not give consent to collecting their information|Medium||High|||
|2.|The number of senior cases may be less than what we expected|Low||Low|||
|3.|Even with the new system, the number of volunteer applications may not be enough to meet the needs of the city|Medium||High|||
|4.|The server may crash, losing all clientele information and causing a shortage of volunteers|Very Low||High|The system can retrieve data from the last backup|All direct users|
### 2.2 ASSUMPTIONS
The identified assumptions are listed below:\
1. The automated Police Background Checking System will be available in a few months.  
2. The system will result in a lower crime rate as a result of ethical job opportunities.  
3. There will be business sponsors that will offer promotions, especially for volunteers.
## 3 PROPOSED SYSTEM OVERVIEW
### 3.1 DESCRIPTION OF PROPOSED VOLUNTEER MANAGEMENT SYSTEM
A sample of Context Diagram for the project is shown below:\
![User_Req_ContextDiagram](https://user-images.githubusercontent.com/113567393/203883828-326d43ec-b93d-4dd2-8442-1dd2bdd5aa42.png)\
**Figure 1 - Context Diagram of Volunteer Management System**
### 3.2 SYSTEM USER PROFILE
A sample of System User Profile for the project is shown below:\
Table II - System User Profile
|No.|User Role|Responsibilities|Branch/Division/Section/Unit|Staff Post/Rank|Stakeholder Group|
|---|---|---|---|---|---|
|1.||Responsible for reporting senior’s health and social status|||Volunteers|
|2.||Responsible for approving volunteers; Responsible for overseeing the progress of senior cases |||Volunteer Administrator|
|3.||Responsible for submitting senior cases into the system|Ministry of Health||SPCC Employees|
|4.||Responsible for submitting requests for further education assistance|School District||School Administrator|
## 4 FUTURE BUSINESS PROCESS
### 4.1 LIST OF FUTURE BUSINESS PROCESS
Table III - List of Future Business Processes for the Volunteer Management System
|Process ID|Business Process Title|
|---|---|
|BP-001|Creation of New Volunteer|
|BP-002|Update of Volunteer Record|
|BP-003||
|BP-004||
|BP-005||
|BP-006||
|BP-007||
### 4.2 BP001-CREATION OF NEW VOLUNTEER
## 4.2.1 PROCESS DESCRIPTION FOR CREATION OF NEW VOLUNTEER RECORD
Table IV - Process Description for Creation of New Volunteer
|Task No.|Actor|Task Name and Description|Input|Output|
|---|---|---|---|---|
|1|Volunteer||||
|2|||||
|3|||||
|4|||||

Table V - More Information for Creation of New Volunteer
|Other Information||
|---|---|
|References||
|Assumptions||
|Business Rules||
## 5 FUNCTIONAL REQUIREMENTS
### 5.1 LIST OF FUNCTIONAL REQUIREMENTS
Table VI - List of Functional Requirements
|Req. ID|Requirement Title|Target Users|Priority (M=must; S=should; C=could; W=won’t)|
|---|---|---|---|
|REQ-CRE-000: Creation of New Volunteer Record||||
|REQ-CRE-001||||
|REQ-UPD-000: Update of Volunteer Record||||
|||||
### 5.2 REQ-CRE-000 CREATION OF NEW VOLUNTEER
Table VI - Requirement Description (REQ-CRE-001)
|Item|Description|
|---|---|
|Requirement ID|REQ-CRE-001|
|Requirement Title|Create a new volunteer|
|Priority|Must|
|Functional Requirement Description|1. Volunteer gets approved to perform service <br/> 2. Volunteer creates an account with username, password, and basic information (full name, address, date of birth, etc.) <br/> 3. Volunteer agrees to Terms and Conditions <br/> 4. Volunteer puts in profile picture <br/> 5. Volunteer enters in favorable activities <br/> 6. List of available cases are displayed for volunteer to choose from|
|Frequency of Use||
|Acceptance of Criteria||
|Related Business Process|Refer to [BP-001](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#42-bp001-creation-of-new-volunteer).|
