# Project plan notes
## Relevance of the system
- Is there a need / potential market?
- Has anyone done anything similar?

### Research showing a need
Our key argument:
- High nurse:patient ratios mean nurses have a lot of work to do in a short time.
- Nurses spend a lot of time on admin and want to spend more time on caring.
- Automation of manual tasks will free up more time for caring. 

**Ratios not rationing: UNISON safe staffing report 2017** https://www.unison.org.uk/content/uploads/2017/04/Rationotrationing.pdf
63.2% of nurses say that comforting or talking to patients was rushed, unfinished, not done to an acceptable standard, or missed entirely. 
54% said medication administration errors happened often or sometimes; 54% said that administering medication on time was done to acceptable standards

**Staffing levels: advice guides (Royal College of Nursing)**
https://www.rcn.org.uk/get-help/rcn-advice/staffing-levels
There is no national guidance on staffing levels and nurse:patient ratios in care homes.

**Guidance on safe nurse staffing levels in the UK (Royal College of Nursing)**
http://www.weds.wales.nhs.uk/sitesplus/documents/1076/rcn%20safe%20staffing%20levels.pdf
In care homes there is an average ratio of 18 patients per registered nurse during the day, and 26 patients per RN at night. 

**Survey of district and community nurses in 2013** https://www.rcn.org.uk/about-us/policy-briefings/pol-1414
19% of the day is spent on administration: only 20% of district and community nurses are satisfied with the distribution of their time across activites, preferring to spend less time on admin and more on direct care and leadership

**Managing medicines in care homes**
https://www.nice.org.uk/guidance/sc1/evidence/full-guideline-pdf-2301173677
NICE healthcare guidelines advice care home providers to consider the following in a medicines administration process:
- 6 R's of administration: right (resident, medicine, route, dose, time), resident's right to refuse
- Make record of administration as soon as possible

R&D work relating to existing assistive technology
https://assets.publishing.service.gov.uk/government/uploads/system/uploads/attachment_data/file/706841/Assistive_Technology_Report_2016-17.pdf - CHIRON?

How will the population grow?
https://www.thelancet.com/journals/lanpub/article/PIIS2468-2667(18)30118-X/fulltext
 190,000 more people aged 65 years or older will require care by 2035 - a rise of 86%. 
 
### Similar existing solutions
- Number of existing solutions for logistical assistance 

https://www.ipa.fraunhofer.de/content/dam/ipa/en/documents/Expertises/Roboter--und-Assistenzsysteme/Servicerobots_residential_care.pdf
- WiMi-Care project: Care-O-bot 3 tracks per-patient hydration and brings them water if they have not drunk enough (in German: https://www.uni-due.de/wimi-care/)
- "inhabitants  understood  the  idea  of  a  robot  supporting  the  staff  without replacing them and showed no fear to interact with the machine" (https://link.springer.com/chapter/10.1007/978-3-642-37346-6_9)
- speech input - addressing them by name (https://ieeexplore.ieee.org/abstract/document/6213397)
- moving on a pre-determined path - but avoiding obstacles (ibid)

What do we add?
- 

## High-level description
- Describe the robot in terms of user stories
### Waking patient
- Nurse specifies wake-up time for each patient in an app
- At the specified time, the robot goes to the specified patient's room
- Once in the room, the robot speaks to wake the patient up
  - We may want to have a 'yes, I've woken up' button or something similar
	- If the patient does not press it, alert the nurse through the app who can then go check on the person
- The robot returns to its spot to await its next command. 
### Checking patient medication
- Nurse specifies the time that a patient needs to take medication through the app
- At the specified time, the robot goes to the specified patient's room
- Once in the room, the robot goes to the patient and:
  - Stretches out arm to receive the medication
  - Moves arm to itself to take a picture of the medication
  - The picture is sent to the nurse for verification through the app
  - Once the nurse approves the medication, the robot uses its arm to return it to the patient
  - (Optional extension) the robot gives a cup to the patient for water
- The robot returns to its spot to await its next command. 
### Checking on patient
- Nurse specifies that the robot should go check on a patient
- The robot moves to the specified patient's room
- The robot approaches the patient and:
  - Indicates with its voice that the nurse would like to check on the patient
  - The patient can indicate if they are ok:
	- If they press the ok button, the robot informs the nurse through the app
    - If they press the not ok button OR do not respond at all, the robot informs the nurse through the app
- The robot returns to its spot to await its next command. 

## Milestones and task decomposition
- What are the main technical subgoals?
  - Do based on user stories
  - For each subgoal: what you should have achieved, what date, what evidence you will show
  - Keep in mind demo dates:
	1. Feb 5th
	2. Feb 26th
	3. March 11th 
	4. March 30th
  - For each milestone - decompose into atomic tasks: name, one-sentence description, estimated time for completion 
	- As a table
    - Mention dependencies - which tasks need to be done beforehand?
    - Gantt chart

## Resource distribution
- How will we deploy 200 hours per group member?
  - Take into account scheduled sessions, and time used in planning / presenting
- What resources do we have available?

## Risk assessment
- What risks do we anticipate? What contingency planning will we do against them?

## Group organization
- What roles are group members taking?
  - Intention is to split the team into two sub-teams: hardware, software
  - Strongly functional organizational structure
  - Each team will have a dedicated POC for co-ordinating with the other team
  - Who will be in each team?
	- Hardware: Rebecca, Jakub, Wojtek, Luukas, Errikos 
    - Software: Ben, Theo, Errikos, Yuchen, Ching Ling
- How will we communicate with each other?
  - Meetings:
	- First two weeks are daily meetings
    - Afterwards - sub-teams will have meetings as needed (min. weekly) and POC from each team will meet weekly on progress
  - Communication:
	- Primarly using Slack channel (detroit15.slack.com)
  - Code sharing:
	- Collaboration using GitHub (github.com/detroit-sdp)
  - Task allocation:
	- GitHub project boards per section (example: github.com/detroit-sdp/reports/projects/1)
    - Kanban-style (to do, in progress, done)
    - Also covers progress tracking
      - Update on progress in meetings
