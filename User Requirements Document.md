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
1.5.	[PROJECT OBJECTIVES](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#15-project-objectives)	5
2.	[**IDENTIFIED RISKS AND ASSUMPTIONS**](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#2-identified-risks-and-assumptions) 6\
2.1.	[Identified Risks](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#21-identified-risks)	6\
2.2.	[Assumptions](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#22-assumptions)	7
3.	[**PROPOSED SYSTEM OVERVIEW**](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#3-proposed-system-overview)	7\
3.1.	[DESCRIPTION OF PROPOSED VOLUNTEER MANAGEMENT SYSTEM](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#31-description-of-proposed-volunteer-management-system)	7\
3.2.	[SYSTEM USER PROFILE](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#32-system-user-profile)	8
4.	[**FUTURE BUSINESS PROCESS**](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#4-future-business-process) 9\
 4.1 [LIST OF FUTURE BUSINESS PROCESS](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#41-list-of-future-business-process) 9\
 4.2 [BP001-CREATION OF NEW VOLUNTEER](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#42-bp001-creation-of-new-volunteer) 9\
 4.2.1 [PROCESS DESCRIPTION FOR CREATION OF NEW VOLUNTEER RECORD](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#421-process-description-for-creation-of-new-volunteer-record) 9
5. [**FUNCTIONAL REQUIREMENTS**](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#5-functional-requirements) 10\
 5.1 [LIST OF FUNCTIONAL REQUIREMENTS](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#51-list-of-functional-requirements) 10\
 5.2 [REQ-CRE-000 CREATION OF NEW VOLUNTEER](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#52-req-cre-000-creation-of-new-volunteer) 10
6. [**NON-FUNCTIONAL REQUIREMENTS**](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#6-non-functional-requirements) 11\
 6.1 [LIST OF NON-FUNCTIONAL REQUIREMENTS](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#61-list-of-non-functional-requirements) 11\
 6.2 [AUDIT, CONTROL, & SECURITY REQUIREMENTS](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#62-audit-control--security-requirements) 12\
  6.2.1 [REQ-ASC1 System Audit](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#621-req-acs1-system-audit) 12\
  6.2.2 [REQ-ASC2 System Control](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#622-req-acs2-system-control) 12\
  6.2.3 [REQ-ASC3 System Security](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#623-req-acs3-system-security) 13\
  6.2.4 [REQ-ASC4 Backup and Recovery Requirements](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#624-req-acs4-system-backup-and-recovery-requirements) 13\
  6.2.5 [REQ-ASC5 Disaster Recovery Requirements](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#625-req-acs5-disaster-recovery-requirements) 14\
  6.2.6 [REQ-ASC6 Privacy Requirements](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#626-req-acs6-privacy-requirements) 14\
 6.3 [DATA REQUIREMENTS](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#63-data-requirements) 15\
 6.3.1 [REQ-DAR1 Global Data Requirements](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#631-req-dar1-global-data-requirements) 15\
 6.3.2 [REQ-DAR2 Key Data Requirements](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#632-req-dar2-key-data-requirements) 15\
 6.4 [USABILITY REQUIREMENTS](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#64-usability-requirements) 16\
 6.4.1 [REQ-USR1 General Usability Requirements](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#641-req-usr1-general-usability-requirements) 16\
 6.5 [SERVICE LEVEL TARGETS](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#65-service-level-targets) 16\
 6.5.1 [REQ-SLT1 System Availability](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#651-req-slt1-system-availablity) 16   
 6.5.2 [REQ-SLT2 System Performance](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#652-req-slt2-system-performance) 17\
 6.6 [DATA GROWTH AND RETENTION REQUIREMENTS](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#66-service-level-targets) 17\
 6.6.1 [REQ-DGR1 Data Growth and Retention Requirements](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#661-req-dgr1-data-growth-and-retention-requirements) 17
 7. [**SYSTEM IMPLEMENTATION CONSIDERATION**](https://github.com/jordanvalenzuela/SENG3130_VMS-Report/edit/main/User%20Requirements%20Document.md#7-system-implementation-consideration) 18
## 1 INTRODUCTION
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
#### 4.2.1 PROCESS DESCRIPTION FOR CREATION OF NEW VOLUNTEER RECORD
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
## 6 NON-FUNCTIONAL REQUIREMENTS
### 6.1 LIST OF NON-FUNCTIONAL REQUIREMENTS
Table VII - List of Non-Functional Requirements
|Req. ID|Category|Requirement Title|Target Users|Priority|
|---|---|---|---|---|
|REQ-ACS1|Audit, Control, & Security|System Audit|||
|REQ-ACS2|Audit, Control, & Security|System Control|||
|REQ-ACS3|Audit, Control, & Security|System Security|||
|REQ-ACS4|Audit, Control, & Security|Backup and Recovery Requirements|||
|REQ-ACS5|Audit, Control, & Security|Disaster Recovery Requirements|||
|REQ-ACS6|Audit, Control, & Security|Privacy Requirements|||
|REQ-DAR1|Data Requirements|Global Data Requirements|||
|REQ-DAR2|Data Requirements|Key Data Requirements|||
|REQ-USR1|Usability Requirements|General Usability Requirements|||
|REQ-SLT1|Service Level Targets|System Availability|||
|REQ-SLT2|Service Level Targets|System Performance|||

### 6.2 AUDIT, CONTROL & SECURITY REQUIREMENTS
#### 6.2.1 REQ-ACS1 SYSTEM AUDIT
Table IX - REQ-ACS1 System Audit
|Item|Description|
|---|---|
|Requirement ID|REQ-ACS1|
|Category|Audit, Control & Security|
|Requirement Title|System Audit|
|Priority|Must (except for those specially specified)|
|Non-Functional Requirement Description|The System shall provide audit trail functionalities which include: <br/> 1. Keep record of user login/logout information, e.g. unsuccessful login attempts, login and logout times, etc.; <br/> 2. Keep record of user profile information such as creation/update/deletion of a user, post/rank, user group belonged to, etc.; <br/> 3. Keep detailed record of the audit trail, which shall include user ID, functions performed, etc.; <br/> 4. Provide facilities to authorized users to allow them to print out audit trails and log records to screen or printer|

#### 6.2.2 REQ-ACS2 System Control
Table X - REQ-ACS2 System Control
|Item|Description|
|---|---|
|Requirement ID|REQ-ACS2|
|Category|Audit, Control & Security|
|Requirement Title|System Control|
|Priority|Must (except for those specially specified)|
|Non-Functional Requirement Description|1. User must create a unique username and password to log-in to the system <br/> 2. System administration functions should be defined in a separate function menu and separated from other normal user functions <br/> 3. Users should be disallowed to click into menu items in which no access rights are granted|

#### 6.2.3 REQ-ACS3 System Security
Table XI - REQ-ACS3 System Security
|Item|Description|
|---|---|
|Requirement ID|REQ-ACS3|
|Category|Audit, Control & Security|
|Requirement Title|System Security|
|Priority|Must (except for those specially specified)|
|Non-Functional Requirement Description|1. User must create a unique username and password to log-in to the system <br/> 2. System administration functions should be defined in a separate function menu and separated from other normal user functions <br/> 3. Users should be disallowed to click into menu items in which no access rights are granted|

#### 6.2.4 REQ-ACS4 System Backup and Recovery Requirements
Table XII - REQ-ACS4 System Backup and Recovery Requirements
|Item|Description|
|---|---|
|Requirement ID|REQ-ACS4|
|Category|Audit, Control & Security|
|Requirement Title|System Backup and Recovery Requirements|
|Priority|Must (except for those specially specified)|
|Non-Functional Requirement Description|1. The System shall provide daily and monthly system and data backup. <br/> 2. The backup shall be performed and completed at midnight <br/> 3. The total lead time for system recovery (in case of system failure) shall not exceed 6 hours with no loss of completed transactional data.|

#### 6.2.5 REQ-ACS5 Disaster Recovery Requirements
Table XIII - REQ-ACS5 Disaster Recovery Requirements
|Item|Description|
|---|---|
|Requirement ID|REQ-ACS5|
|Category|Audit, Control & Security|
|Requirement Title|Disaster Recovery Requirements|
|Priority|Must|
|Non-Functional Requirement Description|1. The system should have an effective solution for resilience and disaster recovery. <br/> 2. In case of total system loss, the system shall be recovered by restoring the latest system backup within 6 hours.|

#### 6.2.6 REQ-ACS6 Privacy Requirements
Table XIV - REQ-ACS6 Privacy Requirements
|Item|Description|
|---|---|
|Requirement ID|REQ-ACS6|
|Category|Audit, Control & Security|
|Requirement Title|Privacy Requirements|
|Priority|Must|
|Non-Functional Requirement Description||

### 6.3 DATA REQUIREMENTS
#### 6.3.1 REQ-DAR1 GLOBAL DATA REQUIREMENTS
Table XV - REQ-DAR1 Global Data Requirements
|Item|Description|
|---|---|
|Requirement ID|REQ-DAR1|
|Category|Data Requirements|
|Requirement Title|Global Data Requirements|
|Priority|Must|
|Non-Functional Requirement Description|1. All passwords must allow input of symbols including *, $, #, &, … <br/> 2. All “date” data to be recorded by the system actually represents the date and time.|

#### 6.3.2 REQ-DAR2 KEY DATA REQUIREMENTS
Table XVI - REQ-DAR2 Key Data Requirements
|Item|Description|
|---|---|
|Requirement ID|REQ-DAR2|
|Category|Data Requirements|
|Requirement Title|Global Data Requirements|
|Priority|Must|

Table XVII - Non-Functional Requirement Description
|Data Group|Data Required|Source|
|---|---|---|
|Volunteer|Name <br/> Date of Birth|Input by Volunteer|
|Senior|Name <br/> Address|Input by SPCC Employee|

### 6.4 USABILITY REQUIREMENTS
#### 6.4.1 REQ-USR1 GENERAL USABILITY REQUIREMENTS
Table XVIII - REQ-USR1 General Usability Requirements
|Item|Description|
|---|---|
|Requirement ID|REQ-USR1|
|Category|Usability Requirements|
|Requirement Title|General Usability Requirements|
|Priority|Must|
|Non-Functional Requirement Description|The system should meet the following usability requirements: <br/> 1. System messages, error messages, etc. shown in the user interface should be clear, direct, consistent, meaningful, and easy to understand. <br/> 2. User actions should be consistent, e.g. for actions that cannot be undone, should always ask for user confirmation and allow users to cancel.|

### 6.5 SERVICE LEVEL TARGETS
#### 6.5.1 REQ-SLT1 SYSTEM AVAILABLITY
Table XIX - REQ-SLT1 System Availability
|Item|Description|
|---|---|
|Requirement ID|REQ-USR1|
|Category|Service Level Targets|
|Requirement Title|System Availablity|
|Priority|Must|
|Non-Functional Requirement Description|The system should meet the following usability requirements: <br/> 1. The system needs to provide service with a high availability of 99.5% during normal working hours (i.e. from 8:00 am to 6:30 pm Monday to Friday and from 9:00 am to 5:00 pm on weekends) <br/> 2. Maintenance can be done any time after normal working hours <br/> 3. Data tolerance or loss can only be allowed for the current working day.|

#### 6.5.2 REQ-SLT2 SYSTEM PERFORMANCE
Table XX - REQ-SLT2 System Performance
|Item|Description|
|---|---|
|Requirement ID|REQ-SLT2|
|Category|Service Level Targets|
|Requirement Title|System Performance|
|Priority|Must|
|Non-Functional Requirement Description|The system should meet the following usability requirements: <br/> 1. 4 seconds for 99.5% of requests for data reports and updates.|

### 6.6 SERVICE LEVEL TARGETS
#### 6.6.1 REQ-DGR1 DATA GROWTH AND RETENTION REQUIREMENTS
Table XXI - REQ-DGR1 Data Growth and Retention Requirements
|Item|Description|
|---|---|
|Requirement ID|REQ-DGR1|
|Category|Data Growth and Retention Requirements|
|Requirement Title|Data Growth and Retention Requirements|
|Priority|Must|
|Non-Functional Requirement Description|The system should meet the following usability requirements: <br/> 1. The expected annual growth rate of data is about 5%. <br/> 2. Daily audit logs shall be removed from the system after every other conducting backup|

## 7 SYSTEM IMPLEMENTATION CONSIDERATION
1. The proposed system is expected to be ready for use by APR 2023.
2. As there is no existing automatic system, no system migration is required and no data conversion is required.  But pre-loading of code tables such as user profiles are required before system release.
3. A few sessions of classroom training for staff in the SPCC and other Volunteer Administrators, School Administrators, and authorized Holders are required.
