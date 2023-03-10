# hw2-Kieran-Amir-Wenwen-Nesa

## Epic 1

This epic is focused on the development of a portable, wearable, 24/7 health and safety monitoring system for the elderly. Stakeholders include the elderly who will wear the device, emergency contacts, doctors and EMS. Features included in this epic include 

- Detecting falls
- Monitor heart rate / pulse
- Gps location tracking
- alert when taken off
- vibrating alarm for deaf users
- text to speech
- speech to text
- monitor diabetes
- alert EMS in emergency
- S.O.S. Button
- changeble, rechargeable battery 
- alert emergency contact in emergency
- alert when time to take meds

## Epic 2

This epic is focused on the safety of the elderly while they are at home. It includes the installation of cameras, anti theft sensors, automated locks, smoke detectors, and carbon monoxide monitors. There will be a hub that all of these devices are connected to accessed with a centralized  control panel.

- The footage from the cameras will need to be acccessed securely onyl by verified users. 
- Alerts can be managed from the control panel
- all devices can be managed from the control panel
- automated locks can be controlled from control panel
- control panel can be used to call EMS in emergency



## Part 4: User Stories in Gherkin Syntax

### User Presses SOS Button
Feature: User presses SOS button<br/>

Scenario: User needs to manually contact emergency services<br/>
Given: The device is connected to the internet and configured with the country's EMS contact info<br/>
When: The use presses the SOS button<br/>
Then: A call is initiated with EMS
### Alert EMS When User Falls
Given that I’m wearing the device and not exercising, when my heart rate is out of normal range for more than 1 minute, then the device will call 911.

### Alert To take meds
Given that I’m wearing the device and it's time to take my med, when I confirm that the med is taken then I expect the amount of remaining med updates accordingly.

 Feature : Reminder for taking meds <br />
 - Scenario     Elderly takes all the meds on time 
 - Given        Elderly takes two different meds per day 
 - And          All the meds are enough 
 - And          An alarm is already set for these two meds on specific time 
 - When         The time for taking a med comes 
 - Then         The alarm goes on 
 - And          The elderly can see on the screen which med to take 
 - And          The elderly confirms that they took the med 
 - And          The quantity of that med will be updated  
 - And          The alarm goes off 

### Send GPS location to a caretaker

Feature: Sending GPS Location to Caretaker

-Scenario: GPS location will be sent to the caretaker<br/>
-Given the elderly person has agreed to wear the GPS enabled device<br/>
-And the caretaker has agreed to receive the GPS location information<br/>
-And the GPS enabled device is fully charged and activated<br/>
-When the elderly person wears the GPS enabled device<br/>
-And the device continuously tracks the location of the elderly person<br/>
-And the device sends the location data to a remote server<br/>
-And the remote server processes the data and sends it to the caretaker's device<br/>
-Then the caretaker receives the GPS location information<br/>
-And can view it on their device<br/>



## Part 5: System Requirements in EARS Syntax

### Take their meds
Where the alarm doesn't go off after an hour, the wearable shall send a message to the elderly's children and doctor.\
If the amount of meds are running low, then the wearable shall send a reminder message to elderly’s children.

<!---2.Where the sugar level drops, the wearable shall send a notification.
3.Where the elderly is unable to read the wearable shall read notifications.
2.If the wearable is taken off, then the wearable shall alert.
3.If the battery goes low, then the wearable shall send a notification of changing the batteries. -->



### SOS Button
While I’m wearing the device, when I press the “SOS” button, the device will call 911. If the call is unsuccessful, it will call again. It will continue the loop until battery is out.

### Fall detection (event driven EARS Statement)
When the device detects a fall, the device shall start a 60 second countown to let the user know EMS will be contacted.


### Smoke and break-in detection sensors
The system shall have sensors installed in the senior's house to detect smoke and break-ins. The sensors shall provide real-time alerts to authorized users when smoke or a break-in is detected.

### Secure access to footage from senior monitoring cameras
The system shall provide secure access to footage from cameras installed around the senior's house. Authorized users shall be able to view the footage in real-time or recorded format. The system shall use secure and encrypted communication channels to protect the privacy and security of the elderly's living situation.
