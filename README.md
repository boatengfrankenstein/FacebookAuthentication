# FacebookAuthentication
This android application simply demonstrates how integrate  facebook authentication with android. 
It follows a similar example of the facebook sample app "scrumptious".The authentication gets the user id and 
the profile picture. You can also get other information of the user as well, by simply using the user object, so far
as its not null. To succesfully integrate facebook login with your app, you must first create and submit a haskey 
from your app and submit it to facebook. Facebook inturn , gives you a unique which u can add to your manifest.
The app as usual will require certain permissions such as internet acess, and a special meta -data from facebook. 
Please ensure that you do this in your manifest.You can check the manifest of this app for more details. 
You will also have to explicitly declare an activity in your manifest for com.facebook.loginActivity.

You have three java files. 
FacebookLogIn (Activity)
Selection Fragment
Splash Fragment

FacebookLogin Activity makes a call to the UI Life Cycler  in the oncreate method as well as sets up the other fragments.
uiHelper = new UiLifecycleHelper(this, callback);
        uiHelper.onCreate(savedInstanceState);
        
        The UiLifecycleHelper class mangaes the users session.
        The UiLifecycleHelper class can manage the authentication flow and keep tabs on the session state through a 
        Session.StatusCallback callback implementation that your activity or fragment passes in to the UiLifecycleHelper instance. 
        The Session.StatusCallback implementation can then be set up to react to session changes and take action.
