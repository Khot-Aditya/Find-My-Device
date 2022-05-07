# Find-My-Device

In case when you lost or can't locate your mobile device you can use friend or family member's smart phone and simply message on your number "FindMyDevice" (default trigger) you can change it and set a custom trigger, when your lost device receives trigger word, this service will get activated then collects location and device state, it will send back this details to the number which SMS was received from, then you can find your lost device's location and in which state it is for example is your device moving from one place to another etc. 

You can set list of contacts to receive trigger from likewise you can set custom contacts list to send notification that your mobile device is lost and they will get it's position and other details. You can set notification to indicate that device is lost and contact the owner, you can also set PIN to restrict unwanted access.

* Service:
	1. Find My Device activates when SMS is received on the device.
	2. It then checks if the SMS sender's contact matches with the database created by the user.
	3. If contact number does match, then it checks for trigger word to reply with location and device state.
	4. If trigger matches, then service collects data as follows:<br/>
          	a) Device's current latitude and longitude.<br/>
         	b) Network single area.<br/>
          	c) Device is moving from one place or not.<br/>
          	d) Device's facing direction.<br/>
          	c) Internet connection.<br/>
          	d) Battery status.<br/>
          	e) etc.<br/>
	5. Within 1s data is sent back to sender and device can be located (Considering all parameters are collected).


* Permissions:
	1. Location Service
	2. SMS Service
	3. Access to Contacts
	4. Access to Phone
	5. Others Sensors

* Unfinished Features:
	1. Email service.

* Screenshots

<img src="Find My Device/Thumbnail.png" alt="screenshot" width="auto" height="300px"/>
<img src="Find My Device/Main Screen.png" alt="screenshot" width="auto" height="300px"/>
<img src="Find My Device/Service Screen.png" alt="screenshot" width="auto" height="300px"/>
<img src="Find My Device/Password.png" alt="screenshot" width="auto" height="300px"/>
<img src="Find My Device/About Screen.png" alt="screenshot" width="auto" height="300px"/>
