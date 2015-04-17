TIL about anonymous types in C#. I hadn't seen these before until I paired with @colatt and was tempted to define an entirely new class when taking JSON from one webservice and relaying it to another. AT's saved a few lines of code :) Score! Checkout [this](https://msdn.microsoft.com/en-us/library/bb397696.aspx) to learn more.

Example:
```C#

var myAnonymousType = { Name = "Dave", TwitterHandle = "@daveshah" }

string name = myAnonymousType.Name
string twitters = myAnonymousType.TwitterHandle

...

```
