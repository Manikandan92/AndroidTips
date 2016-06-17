* Title : What is the mandatory life cycle function that will get called in case of configuration changes??
* Tip-number : 09
* Tip-username : Bhagyasree
* Tip-Description :  What is the mandatory life cycle function that will get called in case of configuration changes?.

## Liefcycle method called in case of configuration changed

When the configuration changes, the life cycle onPause() and onSaveInstanceState() will be called with out fail. There is an exceptional case if the programmer is handling configuartion changes manually, then in that case it will not call above lifecycles.
