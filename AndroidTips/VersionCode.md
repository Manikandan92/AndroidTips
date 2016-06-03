* Title :  What is the importance of version code and version name attributes in manifest file?
* Tip-number : 04
* Tip-username : Madhan
* Tip-Description : What is the importance of version code and version name attributes in manifest file?

###What is the importance of version code and version name attributes in manifest file?
Versioning is important because:

- Users need to have specific information about the application version that is installed on their devices and the upgrade versions available for installation.
- Other applications — including other applications that you publish as a suite — need to query the system for your application's version, to determine compatibility and identify dependencies.
- Services through which you will publish your application(s) may also need to query your application for its version, so that they can display the version to users. A publishing service may also need to check the application version to determine compatibility and establish upgrade/downgrade relationships.