* Title :  What is the difference between this & getapplicationcontext() ? which one to use when?
* Tip-number : 06
* Tip-username : Madhan
* Tip-Description : What is the difference between this & getapplicationcontext() ? which one to use when?

###What is the difference between this & getapplicationcontext() ? which one to use when?

- "this" pointer always points to current class object and the application context points to the entire process. 
- There is only one app context available. 
- If you want to use some views whose life time is through out your application life time then go for application context, otherwise use "this" pointer(which may be an activity context).