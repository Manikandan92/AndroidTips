* Title :  What will happen if I remove onCreate() & onStart() from activity? Will it run?
* Tip-number : 07
* Tip-username : Pangaj J G
* Tip-Description : What will happen if I remove onCreate() & onStart() from activity? Will it run?

###What will happen if I remove onCreate() & onStart() from activity? Will it run?
- Implementing the [Activity life cycle](http://developer.android.com/reference/android/app/Activity.html#ActivityLifecycle) based on the functionality support becomes a standard one
- Programmer can skip those functions which doesn't affect the application 
- If the programmer skip Override functions, the application will call single line of code

```
protected void onCreate(Bundle savedInstanceState) {
    super.onCreate(savedInstanceState);
}
protected void onStart() {
    super.onStart();
}
```