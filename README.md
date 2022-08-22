# Firebase-Authentication
A repository contaning everything required to implement google authentication in your website

This repository will teach you how you can implement and use google authentication in your website.

step-
1.we will be using google firebase,it provides auth,analytics everyting at one place, so much preffered

go to https://console.firebase.google.com/ to get started.
create a new project and name it.
add webapp to project
select script,copy  and paste below <?body> in index file
Go to authentication, sign in methods,google, set name and email, done,
Go to index file , paste 

<script type="module">
    // Import the functions you need from the SDKs you need
    import { initializeApp } from "https://www.gstatic.com/firebasejs/9.9.3/firebase-app.js";
    import { getAnalytics } from "https://www.gstatic.com/firebasejs/9.9.3/firebase-analytics.js";
    import { getAuth ,GoogleAuthProvider } from "https://www.gstatic.com/firebasejs/9.9.3/firebase-auth.js";
    // TODO: Add SDKs for Firebase products that you want to use
    // https://firebase.google.com/docs/web/setup#available-libraries
  
    // Your web app's Firebase configuration
    // For Firebase JS SDK v7.20.0 and later, measurementId is optional
    const firebaseConfig = {
      apiKey: "AIzaSyDay_IbPkMMeW2ywhdgs-uFQBmYUSPuU8Y",
      authDomain: "my-links-tech-7.firebaseapp.com",
      projectId: "my-links-tech-7",
      storageBucket: "my-links-tech-7.appspot.com",
      messagingSenderId: "917637648357",
      appId: "1:917637648357:web:6779c8c012e98b59a3290c",
      measurementId: "G-DBM8WSHDNG"
    };
  
    // Initialize Firebase
    const app = initializeApp(firebaseConfig);
    const analytics = getAnalytics(app);
    const auth = getAuth(app);
    const provider = new GoogleAuthProvider(app);
  </script>
</html>
