# Firebase Phone Authentication :globe_with_meridians:

Firebase Phone Number authentication offers a form of passwordless authentication, wherein users are authenticated on their access to another secure platform, instead of authenticated based on their possession of a password.

The secure platform in the case of Firebase phone number authentication is the user's cell phone. Authentication requires the users to have both the correct cell phone number and physical access to that phone. However, authentication using only a phone number can also be less secure than the other available methods because possession of a phone number can be easily transferred between users.

### Firebase Authentication Flow
 * A user logs on to your web app and is presented with a login field that asks for their phone number.
 * The user enters their phone number into the login field.
 * Firebase's reCAPTCHA verifier swings into action by ensuring that the phone number verification request comes from one of the app's allowed domains.
 * Once the user clicks Log In, a verification code is sent to the user's phone.
 * The user is now requested to type the verification code they received by SMS.
 * Firebase validates the verification code. If correct, a new user account is created and linked to the phone number.
 
 ## Getting Started
 These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. 
 
* Go to [Firebase Console](https://console.firebase.google.com/u/0/) website.
* Create a Firebase Project and choose Add Firebase to your web app.
* Copy the js code snippet and paste in the index.html of this project.


``` html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Firebase Phone Authentication</title>
  <!-- Replace the config -->
  <script src="https://www.gstatic.com/firebasejs/4.3.1/firebase.js"></script>
  <script>
    // Initialize Firebase
    var config = {
      apiKey: "AIzaSyD3r_s3BOy-jtMxSvgyu7tp4fzZvSqOwAc",
      authDomain: "",
      databaseURL: "",
      projectId: "",
      storageBucket: "",
      messagingSenderId: "297418262661"
    };
    firebase.initializeApp(config);
  </script>
  <!-- / Replace the config -->
  
  <!-- Firebase UI -->
  <script src="https://cdn.firebase.com/libs/firebaseui/2.3.0/firebaseui.js"></script>
  <link type="text/css" rel="stylesheet" href="https://cdn.firebase.com/libs/firebaseui/2.3.0/firebaseui.css" />
  <link href="style.css" rel="stylesheet" type="text/css" media="screen" />

</head>
<body>

</body>

```







