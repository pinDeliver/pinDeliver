# Users
All people that will work with planning and follow-up needs a login to pinDeliver. That means that they have to be registered as users. Drivers will use the Go-app for their work tasks and they start the app through a clickable link instead of logging in with User ID and password.

A user can have different permissions, both in which functions they can use in the platform and which delivery groups they have access to.

A newly created pinDeliver account will always have one user created and then you can add unlimited users on your own.

The login method can be of three different types:
* Username and password
* Microsoft Office 365 login
* API login (it is recommended to not use an api user to login to the interface)

To create a new user you select Admin/Users from the main menu. A list of all created users is shown and you just click **Add new user** in the bottom of the list. The settings for the user are grouped in different tabs, see below. Fill in all relevant fields in the user card and click **Create user** to save it. See image and field explanations below for each tab.

![Users](/images/users_list.png)

### Basic information
The first settings tab is the basic settings with name and similar values.

![User](/images/user_basic_information.png)

|Field|Explanation|
|-----|----------|
|Username|The login username for the user. If Office 365 should be used as login method this should be the Office 365 account, normally the users email address.|
|First name|The first name of the user.|
|Last name|The last name of the user.|
|Language|Select the language the user wants to use for the pinDeliver interface.|
|Phone number|The phone number for the user. For information only.|
|Email|The email for the user.|
|Use for api|If the user should be used for an integration. In that case you must generate an api key by pushing **New key**.|
|Password|Type in a password for the user. The password needs to be changed when the user login for the first time. For an Office 365 or api user the password will not be used.|
|Confirm password|type in the same password again.|
|Api key|Shows the generated api key for an api user.|

## Permissions
Once the user is created you need to assign permissions for the user. Permissions is equal to different functionality in the platform. It is possible to select individual functionalities for the user. Below you can see recommended "user permission groups" for different user types. But this is all up to your company.

![User permissons](/images/user_permissions.png)

|Permission|Explanation|
|-----|----------|
|Optimize route|A user with this permission can do route optimization and modify the routes.|
|Assign route|Can assign drivers to a route.|
|Manage vehicles|Can add, change and delete vehicles.|
|Manage drivers|Can add, change and delete drivers.|
|Manage delivery groups|Can add, change and delete delivery groups.|
|Manage users|Can add, change and delete users.|
|View reports|Can view and export follow-up reports.|
|Manage senders|Can add, change and delete senders.|
|Manage orders|Can add, change and delete planning orders and customer orders.|
|Send customer messages manually|Can trigger messages to the customers manually from Office.|
|API documentation|Can access the API menu.|
|Administer company|Can administrate company settings that are common for the whole license (all delivery groups, senders etc).|
|Can view driver contact details|Can view driver details like phone number and email.|
|Manage surveys|Can add, change and delete surveys. Can activate and deactivate surveys.|
|Manage traffic restrictions|Can add, change and delete traffic restrictions for the whole license.|

### Permission groups/User roles
You don´t find any predefined permission groups (or user roles) in pinDeliver. This is of course because each company can have different needs. Below you can see a suggestion for user roles. A specific user can of course have two or more roles and then you can just combine permissions for that user.

* Transport planning
* Customer service
* Administrator
* Superuser

|Permission| Transport planning |Customer service|Administrator|Superuser|
|-----|:----------:|:----------:|:----------:|:----------:|
|Optimize route|X||||
|Assign route|X||||
|Manage vehicles|||X|X|
|Manage drivers|||X|X|
|Manage delivery groups|||X|X|
|Manage users|||X|X|
|View reports|X|X||X|
|Manage senders|||X|X|
|Manage orders|X||||
|Send customer messages manually|X||||
|API documentation||||X|
|Administer company||||X|
|Can view driver contact details|X|X|||
|Manage surveys||X|||
|Manage traffic restrictions|||X|X|

### Company
On this tab you select which companies the user should have access to. For most users and companies you will only be able to select your own company.

![User company](/images/user_company.png)

### Delivery groups
On this tab you select which delivery groups a user should have access to. By default a user will have access to all delivery groups and then nothing needs to be changed. But to limit the access you select the *Access only to the following delivery groups* and then you just drag´n´drop the delivery group from the red "No access"-square to the green "Access"-square to the left. You can also use the arrows between the squares to move all groups at once. (This is useful if a user should have access to more or less all delivery groups. Give access to all and then remove the few that should not be accessed, or vice versa.)

![User delivery groups](/images/user_delivery_groups.png)

### Senders
On this tab you select which senders a user should have access to. By default a user will have access to all senders and then nothing needs to be changed. But to limit the access you select the *Access only to the following senders* and then you just drag´n´drop the senders from the red "No access"-square to the green "Access"-square to the left. You can also use the arrows between the squares to move all senders at once. (This is useful if a user should have access to more or less all senders. Give access to all and then remove the few that should not be accessed, or vice versa.)

![User senders](/images/user_senders.png)
