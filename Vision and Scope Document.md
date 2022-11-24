# **---------------------------------------------------------**
# Vision and Scope Document for Volunteer Management System
### Version 1.0 Approved
### Prepared by Jordan Valenzuela, Kyle McKee, Marium Tawhid
### Thompson Rivers University
### September 23 2022

### Table of Contents

Table of Contents	ii\
Revision History	ii
1.	Business Requirements	1\
1.1.	Background	1\
1.2.	Business Opportunity	1\
1.3.	Business Objectives and Success Criteria	1\
1.4.	Customer or Market Needs	1\
1.5.	Business Risks	1
2.	Vision of the Solution	2\
2.1.	Vision Statement	2\
2.2.	Major Features	2\
2.3.	Assumptions and Dependencies	2
3.	Scope and Limitations	2\
3.1.	Scope of Initial Release	2\
3.2.	Scope of Subsequent Releases	2\
3.3.	Limitations and Exclusions	3
4.	Business Context	3\
4.1.	Stakeholder Profiles	3\
4.2.	Project Priorities	4\
4.3.	Operating Environment	4

## Revision History
|Name |Date|Reason for Changes|Version|
|-----|----|------------------|-------|
|     |    |                  |       |
|     |    |                  |       |

## 1. Business Requirements

### 1.1 Background
Since the COVID pandemic, daily care workers for seniors have significantly dropped.  It is estimated that there are 10000 to 15000 senior cases that the city needs to attend to; however, with the lack of workers, as well as the limited speed of the current system, the city is unable to meet the demands fast enough. As well, due to the limited number of teachers, there is a demand in the elementary school system for additional  coaching and teaching for the students. At the moment, a lot of time is spent screening potential volunteers, and there is a lack of incentives for volunteers to contribute their time.  While people are recovering from the pandemic, we should be able to support children and seniors alike with the help of qualified volunteers.
### 1.2 Business Opportunity
The mayor has requested a centralized system to connect volunteers to seniors and children in need of special care. Combining all of the desired users into one domain will eliminate the disassociation between systems of volunteers and those of seniors and children, ensuring faster connections and a greater likelihood of such patients receiving care. Detailed profiles of patients will allow volunteers to find a patient to whom they specialize in their needs. By engaging the community in benevolent activity, the community will benefit in terms of their comfort. Such action can be incentivised with local business promotions, which may increase the number of volunteer applicants. 
### 1.3 Business Objectives
BO-1: Reduce the application process time
* Scale: Time for background validation to be processed.
* Meter: Time comparison between volunteer application request and approval (via admin logs).
* Past: 2 weeks (10 business days for police check)
* Goal: 48 hours or less

BO-2: Develop a centralized system that accurately keeps track of seniors

BO-3: Reduce assignment time by 30% - Seniors should get volunteer services within three days
* Scale: Time to assign volunteers to seniors.
* Meter: Examination of volunteer booking logs (admin logs).
* Past: 10 days
* Goal: 3 days or less

#### **Success Criteria**
SM-1: In the first year, 60% of senior cases within the city should be tracked\
SM-2: In the first year, 85% of reported cases should receive support from the system\
SM-3: The margin of error or sudden alarm (of volunteer shortage) should be kept to less than 2 times per year
### 1.4 Customer or Market Needs
The basic users of the platform would be Management in the Seniors Care facilities, who would register seniors in need of care as well as teachers in the elementary school system who would add the students in need of additional coaching/tutoring. The managers would simply need to login in and input the profile of the senior with parameters describing their level of care, needs, and time of care (i.e. length of time), location, and other relevant information. The teachers would also login, and input in the information of the student, the courses in which they require help, location, and other information that impacts the level of service provided (for example if they’re special needs, or prefer different methods of learning). The goal is to provide the best and quickest  level of service possible through matching based on the information provided, and have the system be flexible enough to run on cross-platform settings.
### 1.5 Business Risks
One of the risks involved with the platform is that it is heavily reliant on the police background checking system being ready on time, especially if both areas (seniors AND student) of volunteering require a successful background check in order to proceed with the application. One possible method to mitigate this risk is to constantly communicate with the developers of the automated policy checking system to  ensure that the system will be developed on time.This way, the developers of the Volunteer Management System are free to continue with the system’s production.

Other risks include:\
a. The senior may not consent to having their information collected (Probability = 0.4; Impact = 7)\
b. The amount of senior cases might be less than what we expect (Probability = 0.2; Impact = 2)\
c. Even with the new system, the number of volunteer applications may not be enough to meet the needs of the city (Probability = 0.5; Impact = 9)\
d. Base server crashes, losing all clientele information and causing a shortage of volunteers (Probability = 0.01, Impact = 10)\
## 2. Vision of the Solution
### 2.1 Vision Statement
For the Mayor who wants to provide swift and secure care for his seniors and children, the Volunteer Management System (VMS) is an internet-based, smartphone and tablet-enabled application that will allow interested members of society to submit their applications. Seniors can get the support they need, and parents and guardians can request additional aid for their children. Unlike the current method of manually inputting and sending the data of applicants, users who use the Volunteer Management System will not have to wait two weeks to sign up or receive care. This system will help reduce crime rates, improve the quality of life for seniors, and help children perform better in school.
### 2.2 Major Features
1. The system will send volunteer assistance to seniors in need and children that require more tutoring and/or coaching within three days.
2. Within the first day of notice, the system will check for volunteer availability and credibility (send data of the selected volunteer(s) to the police department for background check).  Once credibility is achieved, volunteer(s) will help the client(s) the next day.
3. The system should continue to monitor seniors even after support is given
4. The system should notify the city of a forecasted entry of needed cases for the next week (based on current data).  
### 2.3 Assumptions and Dependencies
AS-1: The automated Police Background Checking System will be available in a few months.   
AS-2: The system will result in a lower crime rate as a result of job opportunity\
AS-3: There will be business sponsors that will offer promotions especially for volunteers\
DE-1: If the police department has an automated background check system, the Volunteer Management System must be able to communicate with it bidirectionally.
## 3. Scope and Limitations
### 3.1 Scope of Initial Release
By initial release, the system will keep track of many senior cases and give support to most of them. The system will also provide volunteers for elementary school children that need the extra tutoring and/or coaching.  Any new volunteers and seniors will be able to register themselves into our system. 
### 3.2 Scope of Subsequent Releases
Over time, the system should be able to keep track of more and more of these senior cases. Subsequent implementations will allow for volunteer reviews, and requests to become a recurring client of a volunteer. As volunteers complete jobs (alongside their background information), the system should recommend patients to whom their skills are suited for.
### 3.3 Limitations and Exclusions
The system will not provide a direct solution to each senior case but rather, assign a qualified volunteer who has gone through a background check by the police to come to the client’s residence or place of stay to support them. The system will only be used in this city.
## 4. Business Context
### 4.1 Stakeholder Profiles
|**Stakeholder** |**Major Value**|**Attitudes**|**Major Interests**|**Constraints**|
|-----|----|------------------|-------|--------------------------------------------|
|**Project Sponsor**|Improved Seniors Care <br /> -Lower Crime Rates <br /> -Increased Business|Extremely enthusiastic and optimistic about making sure that the seniors and children in the city are receiving the care they need.|Meet the demand for senior’s help and accurately account for and predict (week in advance) the help required, thus preventing emergencies.|Consent of Seniors to have their information uploaded online. <br /> -Have actively involved guardians for the children.|
|**Police**|Provide the background check required for the application process|Enthusiastic about lowering the crime rates in the city|Have a faster screening process, lower crime rates|Training for staff to use the new system|
|**Sponsors; Business Owners**|Provide incentive for volunteers; higher number of volunteers|Supportive and willing to aide by offering special promotions to volunteers|Increased business due to lower crime rates||
|**Volunteers**|Key in providing the care and coaching required. <br /> -Job opportunities||Job opportunity, give back to the community.|To be cleared on the background check; Have a minimum education level in order to tutor/coach students.|
### 4.2 Project Priorities
|**Dimension** |**Driver**|**Constraints**|**Degree of Freedom**|
|-----|----|------------------|-------|
|Schedule|release 1.0 to be available by 12/1, release 1.1 by 3/1|||
|Features|||70-80% of high priority features must be included in release 1.0|
|Quality|||90-95% of user acceptance tests must pass for release 1.0, 95-98% for release 1.1|
|Staff||maximum team size is 6 developers + 4 testers||
|Cost|||budget overrun up to 15% acceptable without executive review|
### 4.3 Operating Environment
Users of this system will be confined to the city.  Users will need access to the system when a massive shortage of support occurs after the system is implemented, when the system requires updates or any other changes. The system should only be accessed when it is necessary to access it, such as updating client data and system maintenance.  People that do not need to see client data should not be allowed to access client data.  Clients will only be able to view and edit their own information.
