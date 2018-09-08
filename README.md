# Implementing-attacks-on-android-and-creating-an-android-security-application
We have implemented our security application in two stages-
1.	Scan for installed applications and display permissions :
Background:
This module was designed with the basic idea that any APK/App/Update available on the internet can be malicious, several apps downloadable for free online were infected with malware that could harm the device, store credentials or any other information.
The App in Action:
When launched, the module has a Scan button which allows the user to scan all the installed apps in the device and then the user must click “All apps permissions” button which displays the list of all installed apps along with the list of permissions accessed by each individual app. 

2.	Detect potentially harmful applications
The App in Action:
In our application, we have identified 3 basic dangerous permissions and filtered out the apps and labeled the apps accessing these 3 permissions as potentially dangerous. READ_CONTACTS, INTERNET and READ_EXTERNAL_STORAGE are the permission levels considered as dangerous. When launched, the module has a Scan button which allows the user to scan all the installed apps in the device and then the user has to click the second button ” Potentially dangerous apps” to display the potentially harmful applications. 
As a part of showing how the security application can catch one of the implemented attacks, we have used the same apk used by meterpreter attack and installed the apk in our device and then try to scan for Potential malware app. The result was successful, and we were able to detect metasploit apk as potential threat.
