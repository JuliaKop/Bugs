# Bugs
ID:  1
Summary:  [Configuration] button overlaps [Add] button on price package page.
Severity: Minor
Description: On information price package page [Configuration] button overlaps  [Add] button.
Test environment: Windows, Opera
Reproducibility: always
Workaround: the overlay of buttons does not interfere with their action
Steps to reproduce:
1.     Click [Price package] button
2.     Click [Configuration] button
Actual result: [Configuration] button overlaps [Add] button.
Expected result: [Configuration] button does not overlap [Add] button.

ID:  2
Summary: No matter what type of zone is editing it is of a blue color on the map
Severity: minor
Description: After clicking on [Edit] on the https://admin.scootapi.com/geofence page opens a page with form and map whereby the edited zone is drawn. All zones are blue, no matter what color was assigned.
Reproducibility: always
Symptom: enhancement
Steps to reproduce:
1. Open https://admin.scootapi.com/ Credentials: 
login: group3@it-academy.by
password: 2BwntG4gM5MtmVYKnk9WJy2XSGcxVb7K3
2. Click on Geofence/zones in the menu
3. Click on [Edit] of any zone
Actual result: the zone is drawn by blue color on the editing page no matter what color was assigned to that zone type
Expected result: zones of different types have different colors on the editing page as well as on the geofence page and color of zone changes when user chooses another zone type in the dropdown menu in the editing form

ID: 3
Summary: Mini delete icon doesn’t delete created note.
Severity: Medium
Description: Created note doesn’t delete via clicking on mini delete icon in the action bar.
Test environment: Android 6.0.1
Reproducibility: Always
Workaround: Click on the created note field on the main page and hold until the command list appears, click on [Delete] button.
Attachment: https://drive.google.com/file/d/18W7LQ0FA8HWUyoaNXPXRPdogeKcf1Hku/view?usp=sharing ‌
Steps to reproduce:
1) Click on created note on the main page
2) Click on mini delete icon in the action bar
Actual result: The note is not deleted and is shown on the main page.
Expected result: The note is deleted from the list of notes on the main page.

ID: 4
Summary: [Paste] button id disabled in the action bar.
Severity: Medium
Description: [Paste] button appears via clicking on settings button in the right corner of the action bar on the main page. It is not clickable.
Test environment: Android 6.0.1
Reproducibility: Always
Attachment: https://drive.google.com/file/d/18b9-2lwXeOQgjuemdXsck4FQX-km2pq2/view?usp=sharing
Steps to reproduce:
1) Click on [⋮ ] button in the action bar.
2) Click on [Paste] button.
Actual result: [Paste] button is disabled in the action bar on the main page.
Expected result: [Paste] button is clickable. 

ID: 5
Summary: When searching for caregivers through the zipcode or name, the search result gives an incomplete number of people.
Severity: Medium
Description: When entering an zipcode or name in the search field for caregivers or families and after clicking on the search button, the search result shows an incomplete list of people.
Test environment: Windows 10 64x, Chrome 88.0.4324.190, Edge 88.0.705.81
Reproducibility: Always
Steps to reproduce:
1) Open https://dev-opakare.com/job-list.
2) Enter any zipcode or name in 'Search zipcode' field.
3) Click on [Search] button.
Actual result: Incomplete result of the list of caregivers or families
Expected result: the requested user is displayed in the list.

ID:  6
Summary:  When log in for the first time to ScootApi application and wait for sms code  button [Проверить] overlaps the timer till next try to request sms code
Severity: minor
Description: When user login for the first time and have to enter sms code, the button [Проверить] overlaps the timer which indicates when user can ask for sms code again
Test environment: iPhone SE
Workaround if touch the screen and pull it up, timer becomes visible
Symptom: cosmetic flaw
Steps to reproduce:
1.Open scootApi on your mobile phone
2.Click on menu
3.Click ‘Профиль’
4. Click ‘Выйти’
5. Enter your phone number
Actual result: [Проверить] overlaps timer till next try to ask sms code and overlaps asterisks for sms code
Expected result: The timer and asterisks are visible.

ID:  7
Summary: The alert about no trip location change doesn't appear after setting another coordinates to the scooter which is off. Instead of it the alert Scooter_No_Signal appears
Severity: medium
Description: The alert about  no signal appears instead of the no trip location change alert on the fleet and scooter pages after setting another  location in Postman to the switched off scooter
Reproducibility: always
Symptom : missing feature
Steps to reproduce:
1 Open https://admin.scootapi.com/ Credentials: 
login: group3@it-academy.by
password: 2BwntG4gM5MtmVYKnk9WJy2XSGcxVb7K3
2 Select any scooter and turn it off if necessary, click on it
3 Check it's initial location
4 Open Postman and send a request to  https://api.scootapi.com/scooters/telemetry 
in the body set other coordinates to the scooter eg:
 [
   {
       "channel.id": 0,
       "serial_number": "DEMO_Sochi_721",
       "powered_on": false,
       "battery": 70,
       "geo": "43.54272254840334, 39.795897244165026"
   }
]
5. Open the scooter page
Actual result: Alert Scooter_no_signal  appears on the scooter page
Expected result: Alert no trip location change appears on the scooter page


 







