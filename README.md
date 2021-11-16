# Find-My-Device

Hello,

My name is Aditya, I made "Find My Device" app to upload on play store, but for personal reasons it is canceled and now I need to sell this project. In case when you lost or can't locate your mobile device you can use your friend's or family member's smart phone and simply message on your number "FindMyDevice" (default trigger) you can change it and set a custom trigger, when your lost device receives trigger word, Find My Device app's service will get activate and start collecting location and device state after collecting (takes about 500ms - 1s), it will send back to the number which SMS was received from, then you can find your lost device's location and in which state it is for example is your device is moving from one place to another then it will send "device is on move" otherwise it will respond with "device is not moving". 

You can set list of contacts to receive trigger from likewise you can set custom contacts list to send notification that your mobile device is lost and they will get it's position and state. You can set notification to indicate that your device is lost and contact the owner. You can set PIN to Find My Device app to restrict unwanted access. In case of accidental trigger (Unlikely) you can check Find My device app's service logs from About > Privacy Policy > Logcat.﻿

* How it Works:
	1. Find My Device activates when SMS is received on the device.
	2. It then checks if the SMS sender's contact matches with the database created by the user.
	3. If contact number does match, then it checks for trigger word to reply with location and device state.
	4. If trigger matches, then service collects data as follows:
          	a) Device's current latitude and longitude.
         	 	b) Network single area.
          	c) Device is moving from one place or not.
          	d) Device's facing direction.
          	c) Internet connection.
          	d) Battery status.
          	e) etc.
	5. Within 1s data is sent back to sender and device can be located (Considering all parameters are collected).


* Permissions used by Find My Device:
	1. Location Service
	2. SMS Service
	3. Access to Contacts
	4. Access to Phone
	5. Others Sensors

* Unavailable Features:
	1. Email service is unfinished.
	2. Password to boot device.

* Find My Device is compatible with android.﻿
* Changes to UI can be made.
