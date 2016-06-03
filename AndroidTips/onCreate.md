
* Title :  What will happen if I remove super.oncreate() from oncreate() function of activity
* Tip-number : 03
* Tip-username : Madhan
* Tip-Description : What will happen if I remove super.oncreate() from oncreate() function of activity


###What will happen if I remove super.oncreate() from oncreate() function of activity?
Every Activity you make is started through a sequence of method calls. onCreate() is the first of these calls.

Each and every one of your Activities extends android.app.Activity either directly or by subclassing another subclass of Activity.

In Java, when you inherit from a class, you can override its methods to run your own code in them. A very common example of this is the overriding of the toString() method when extending java.lang.Object.

When we override a method, we have the option of completely replacing the method in our class, or of extending the existing parent class' method. By calling super.onCreate(savedInstanceState);, you tell the Dalvik VM to run your code in addition to the existing code in the onCreate() of the parent class. If you leave out this line, then only your code is run. The existing code is ignored completely.

However, you must include this super call in your method, because if you don't then the onCreate() code in Activity is never run, and your app will run into all sorts of problem like having no Context assigned to the Activity (though you'll hit a SuperNotCalledException before you have a chance to figure out that you have no context).

In short, Android's own classes can be incredibly complex. The code in the framework classes handles stuff like UI drawing, house cleaning and maintaining the Activity and application lifecycles. super calls allow developers to run this complex code behind the scenes, while still providing a good level of abstraction for our own apps.
