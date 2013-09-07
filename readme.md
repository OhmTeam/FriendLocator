FriendLocator
=============

This is a simple Android app for Facebook that loads your friends list, then loads the locations of all of your friends at the push of a button.

## Requirements/Setup
You have to already be set up to work with Android projects. Beyond that, there are just a few things you need to do before this will run.

  1. Add your "androiddebugkey" to the allowed "Key Hashes" on the Facebook App summary page for "FriendMapper" here: [https://developers.facebook.com/apps/572255019482219/summary/](). Instructions for doing so are in the middle of *Step 4* on the [getting started/facebook sdk for android](https://developers.facebook.com/docs/android/getting-started/facebook-sdk-for-android/) page. Look for `keytool -exportcert ...`

  2. Add the Facebook SDK as a reference to the eclipse project, once you've imported it to your workspace. Instructions for this are on the "getting started" tutorial mentioned above. A relevant screenshot is located under the header "Link to the SDK project and configure the Facebook app ID".

## What it Does

Once you've got the Eclipse project to compile successfully, run it (default shortcut is Ctrl+F11). You should see a Facebook "Log In" button. Click it to log in to Facebook. Once you have done that, a "Load Friends" button will appear. Clicking that will spawn a few HTTP requests to the Facebook API, loading your friends list, then loading info on their locations (latitude, longitude). This info will be logged under the "MainFragment" tag in your LogCat view. There is currently no UI for the friend+location info.