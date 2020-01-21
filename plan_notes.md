# Project plan notes
## Relevance of the system
- Is there a need / potential market?
- Has anyone done anything similar?

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
