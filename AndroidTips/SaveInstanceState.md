* Title : Can I save large images downloaded from internet in onsaveinstancestate()?
* Tip-number : 08
* Tip-username : Madhan
* Tip-Description :  Can I save large images downloaded from internet in onsaveinstancestate()?

## Save large images in onSaveInstanceState

onSaveInstanceState() function has to be used for saving small objects (transient states). If we want to save large objects use onRetainNonConfigurationInstance() function.