## Getting Started:


###### Description

Cloud Foundry is an open platform as a service, providing a choice of clouds, developer frameworks, and application services. Cloud Foundry makes it faster and easier to build, test, deploy and scale applications.
It is an open source project and is available through a variety of private cloud distributions and public cloud instances.
The Cloud Foundry Action Pack for CA Continuous Delivery Automation (formerly known as CA Automic Release Automation) allows you to build visual workflows to fully automate common Cloud Foundry related activities around authentication, services, and applications.
		
###### Actions


1.   Login
     Action Description: This action is used to authenticate against Cloud Foundry services with the provided credentials and generate an authentication token.

2.   Logout
     Action Description: This action is used to logout from Cloud Foundry for the user whose authentication token is provided.

3.   Change Target
     Action Description: This action is used to change the target i.e. organization and/or space for the user whose authentication token is provided.

4.   Start Application
     Action Description: This action is used to start each instance of the given application for the user whose authentication token is provided. Make sure that your application runs fine on your local system before starting the application as it would result in failure of the action.

5.   Stop Application
     Action Description: This action is used to stop a running application in Cloud Foundry. This action would fail if specified application name doesn?t exist. 

6.   Restart Application
     Action Description: This action is used to restart each instance of the given application for the user whose authentication token is provided. The action will fail if application does not exists in Cloud Foundry.

7.   Push Application
     Action Description: This action is used to push an application to Cloud Foundry for the user associated to the provided authentication token. It allows a user to deploy a single application to Cloud Foundry or deploy multiple application using a manifest file.

8.   Delete Application
     Action Description: This action is used to delete an application in Cloud Foundry. This action will not fail even if specified application doesn?t exist in Cloud Foundry.

9.   Scale Application
     Action Description: This action is used to scale an existing application either horizontally (create or destroy additional instances) or vertically (modifying available disk space or memory) or both. 

10.  Create Service
     Action Description: This action is used to create a service instance in Cloud Foundry from the marketplace of services.

11.  Create User Provided Service
     Action Description: This action is used to create an instance of user provided service.

12.  Delete Service
     Action Description: This action is used to delete a service instance in Cloud Foundry. The name of service is case-sensitive in Cloud Foundry. This action would not fail if specified service doesn?t exist.

14.  Bind Service
     Action Description: This action is used to bind a service instance to an application in Cloud Foundry. If the user binds a service that an application is already bound to, the action will not fail but will give the message that application is already bound to the given service.

16.  Unbind Service
     Action Description: This action is used to unbind a service instance from an application in Cloud Foundry.

17.  Create Domain
     Action Description: This action is used to create private domain for specified 'organization' in Cloud Foundry.

18.  Create Route
     Action Description: This action is used to create a route in Cloud Foundry for the user whose authentication token is provided. If the user creates an already existing route, the action will not fail but will give the message that it already exists.

19.  Map Route
     Action Description: This action is used to map the domain to an application in Cloud Foundry with an optional hostname in the current targeted organization and space. This action also creates the route if it does not already exist.

20.  Unmap Route
     Action Description: This action is used to unmap a route from an application in Cloud Foundry in the current targeted organization and space.

21.  Delete Route
     Action Description: This action is used to delete the specified route from Cloud Foundry for the user whose authentication token is provided. This action will delete the route across the Cloud Foundry, irrespective of the target organization and space.]]></DOC>

		
###### Compatibility:

1. Open JDK Java 11
2. Oracle Java 1.7

###### Prerequisite:

1. Automation Engine should be installed.
2. Automic Package Manager should be installed.
3. ITPA Shared Action Pack should be installed. 
4. PCK.AUTOMIC_FILESYSTEM Action Pack should be installed. 
5. The Agent should be able to access the Cloud Foundry URL(s) in order to make HTTP requests.
6.	CF CLI tool version 6.14.1 or higher must be installed on the Agent machine and set as an executable.
7.	You should have connection details to connect to Cloud Foundry Services.

###### Steps to install action pack source code:

1. Clone the code to your machine.
2. Go to the package directory.
3. Run the command apm upload in the directory which contains package.yml (source/):

Ex. apm upload -force -u <Name>/<Department> -c <Client-id> -H <Host> -pw <Password> -S AUTOMIC -y -ia -ru


###### Package/Action Documentation

Please refer to the link for [package documentation](source/ae/DOCUMENTATION/PCK.AUTOMIC_CLOUDFOUNDRY.PUB.DOC.xml)

###### Third party licenses:

The third-party library and license document reference.[Third party licenses](source/ae/DOCUMENTATION/PCK.AUTOMIC_CLOUDFOUNDRY.PUB.LICENSES.xml)

###### Useful References

1. [About Packs and Plug-ins](https://docs.automic.com/documentation/webhelp/english/AA/12.3/DOCU/12.3/Automic%20Automation%20Guides/help.htm#PluginManager/PM_AboutPacksandPlugins.htm?Highlight=Action%20packs)
2. [Working with Packs and Plug-ins](https://docs.automic.com/documentation/webhelp/english/AA/12.3/DOCU/12.3/Automic%20Automation%20Guides/help.htm#PluginManager/PM_WorkingWith.htm#link10)
3. [Actions and Action Packs](https://docs.automic.com/documentation/webhelp/english/AA/12.3/DOCU/12.3/Automic%20Automation%20Guides/help.htm#_Common/ReleaseHighlights/RH_Plugin_PackageManager.htm?Highlight=Action%20packs)
4. [PACKS Compatibility Mode](https://docs.automic.com/documentation/webhelp/english/AA/12.3/DOCU/12.3/Automic%20Automation%20Guides/help.htm#AWA/Variables/UC_CLIENT_SETTINGS/UC_CLIENT_PACKS_COMPATIBILITY_MODE.htm?Highlight=Action%20packs)
5. [Working with actions](https://docs.automic.com/documentation/webhelp/english/AA/12.3/DOCU/12.3/Automic%20Automation%20Guides/help.htm#ActionBuilder/AB_WorkingWith.htm#link4)
6. [Installing and Configuring the Action Builder](https://docs.automic.com/documentation/webhelp/english/AA/12.3/DOCU/12.3/Automic%20Automation%20Guides/help.htm#ActionBuilder/install_configure_plugins_AB.htm?Highlight=Action%20packs)

###### Distribution: 

In the distribution process, we can download the existing or updated action package from the Automation Engine by using the apm build command.
Example: apm build -y -H AE_HOST -c 106 -u TEST/TEST -pw password -d /directory/ -o zip -v action_pack_name
			
			
###### Copyright and License: 

Broadcom does not support, maintain or warrant Solutions, Templates, Actions and any other content published on the Community and is subject to Broadcom Community [Terms and Conditions](https://community.broadcom.com/termsandconditions)

###### Questions or Need Help? 

Join the [Automic Community Integrations](https://community.broadcom.com/communities/community-home?CommunityKey=83e49dd4-b93e-464a-a343-2bb1e51c13ec) to discuss this integration.
