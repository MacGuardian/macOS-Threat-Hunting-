https://attack.mitre.org/techniques/T1555/001/

"Adversaries may acquire credentials from Keychain. 
Keychain (or Keychain Services) is the macOS credential management system that stores account names, passwords, private keys, certificates, sensitive application data, payment data, and secure notes. 
There are three types of Keychains: Login Keychain, System Keychain, and Local Items (iCloud) Keychain.
The default Keychain is the Login Keychain, which stores user passwords and information. 
The System Keychain stores items accessed by the operating system, such as items shared among users on a host. 
The Local Items (iCloud) Keychain is used for items synced with Apple’s iCloud service."

**Notes: credentials on macOS are stored under**
|Command: sudo ./keychaindump ~/Library/Keychains/login.keychain
 ---|

**Threat Hunt Recommendation: To search for this technique, keep an eye out for any processes that are pointing at the keychain 
or attempting to dump its contents. 
**

