* Title : Difference between this & getapplicationcontext()
* Tip-number : 11
* Tip-username : Raasesh
* Tip-Description :  What is the difference between this & getapplicationcontext() ? which one to use and when to use?

---
- [this] (#WhatIsthis?)
- [where to use this] (#Wherethis)
- [getApplicationContext()] (#WhatIsgetApplicationContext())
- [where to use getApplicationContext()] (#WheregetApplicationContext)

## <a name="WhatIsthis?"> this </a>

We use this to refer to the current activity within the Application


## <a name="Wherethis"> where to use this </a>

"this" is used in scenarios where the context of the current activity needed to be used.

Example: used in intent while moving from one activity to another to keep track of previous activities. 


## <a name="WhatIsgetApplicationContext()"> getApplicationContext() </a>

We use getApplicationContext to refer the Application class, which is same throughout the entire lifecycle of the Application.


## <a name="WheregetApplicationContext"> where to use getApplicationContext() </a>

"getApplicationContext()" are used during scenarios where   the context of the current activity is not required.

Example: Toast