* Title : What is ANR?
* Tip-number : 05
* Tip-username : Bhagyasree
* Tip-Description :  What is ANR (application not responding)? What is the reason for this problem and what is the solution for that problem?.

---
- [ANR] (#WhatIsANR?)
- [Reason to occur] (#WhatIsReason?)
- [Solution] (#SolutionToSolve)
- [View ANR errors] (#HowToView)

## <a name="WhatIsANR?"> ANR </a>

ANR (Application Not Responding) is not exactly an error. It is shown when your application is very sluggish and takes a lot of time to respond, thus making the user wait. The user won't appreciate if your application makes them wait for a long time. So, the Android framework gives the user an option of closing your application.

![](Images/anr.png)

## <a name="WhatIsReason?"> Reason to occur </a>

ANR occurs, if we are doing any other heavy functionality(network access) along with UI in single main thread. If two heavy functionalities happen in single thread, it will delay the response to users and hence stop your process.

The ANR dialog is displayed to the user based on two possible conditions. One is when there is no response to an input event within 5 seconds, and the other is when a broadcast receiver is not done executing within 10 seconds.

## <a name="SolutionToSolve"> Solution </a>

* Run only UI components in Main Thread not Network calls


## <a name="HowToView"> View crashes & ANR errors </a>

If your app stops responding, ANR error dialog will appear wich is shown above. ANR data is only available on your Google Play Developer Console.

To help you troubleshoot these issues, you can use your Developer Console ANR data to help you find the type of issue, location information, and how often the errors have occurred.

Your ANR statistics include all instances that are reported by users.