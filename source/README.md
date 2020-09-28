About action pack:
	Cloud Foundry is an open platform as a service, providing a choice of clouds, developer frameworks, and application services. Cloud Foundry makes it faster and easier to build, test, deploy and scale applications.
	It is an open source project and is available through a variety of private cloud distributions and public cloud instances.
	The Cloud Foundry Action Pack for CA Continuous Delivery Automation (formerly known as CA Automic Release Automation) allows you to build visual workflows to fully automate common Cloud Foundry related activities around authentication, services, and applications.

Available Actions:

		1.	Login
		2.	Logout
		3.	Start Application
		4.	Restart Application
		5.	Stop Application
		6.	Push Application
		7.	Scale Application
		8.	Delete Application
		9.	Change Target
		10.	Create Service
		11.	Create Domain
		12.	Bind Service
		13.	Delete Service
		14.	Unbind Service
		15.	Create Route
		16.	Map Route
		17.	Unmap Route
		18.	Create User Provided Service
		19.	Delete Route


Supported Platforms:

	1. Oracle JDK 1.7 or higher must be installed on Agent OS and "java" must be set as executable on the same.
	2. The Agent should be able to access the Cloud Foundry URL(s) in order to make HTTP requests.
	3.	CF CLI tool version 6.14.1 or higher must be installed on the Agent machine and set as an executable.
	4.	You should have connection details to connect to Cloud Foundry Services.

Cloud Foundry pack depends on

	- Automation.Engine » AutomationEngine (minimum version Automation.Engine 11.2)
	- Package.Filesystem » PCK.AUTOMIC_FILESYSTEM (minimum version Package.Filesystem 1.1)
	- Package.ITPA.Shared » PCK.ITPA_SHARED (minimum version Package.ITPA.Shared 1.1)
