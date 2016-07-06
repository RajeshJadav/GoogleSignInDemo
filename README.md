# GoogleSignInDemo
Demo project for adding Google Sign-In to your android app

Prerequisites:

To create a project, visit the developer’s console at: https://console.developers.google.com/project. After a few minutes you’ll be directed to the project’s home page.
Select ‘APIs & auth’ on the left hand side of the screen. Select ‘APIs’ and you’ll see a screen containing all available APIs.
Find the Google+ API. Click ‘Enable API’ to turn on the API. 

For configuring credentails you need to Get your SHA-1. You can access your SHA-1 in the debug keystore.

    On a Mac or Linux, this is in the ~/.android directory.
    On Windows it is at C:\Users\<your user name>\.android.C:\Users\<your user name>\.android.

Note that the .android folder is hidden so you will not be able to see it in Finder or Windows Explorer. Open a terminal (Command Prompt on Windows) and issue the following command (changing ~/.android.debug.keystore to the appropriate path for your OS):

    -keystore ~/.android/debug.keystore -alias androiddebugkey -storepass android -keypass android

In the developer's console, select the ‘Consent screen’ link in the APIs & auth section.You must provide your email address and App name.


Now that you have the SHA1 key, and the consent screen is configured, it’s time to create your credentials.Select the ‘Credentials’ link on the left. Under OAuth, select ‘Create new Client ID’. Choose ‘Installed Application’, and choose ‘Android’. Enter the Package name you will be using in your app. You'll be creating a new project so it can be whatever you like, such as com.yourname.codelab1. (You'll need to remember it when you create your project later.)
Add the SHA1 you got earlier. You can leave Deep Linking Disabled.

Important: Remember the package name you entered. You’ll need it later, because it has to match the package name of your app.

Click Create Client ID, and after a few moments you’ll be taken back to the credential screen, and the Client ID will be ready.



