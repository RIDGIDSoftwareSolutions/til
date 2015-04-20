In clojure, sets are functions of their members. If I define a set, then call this set (as a function) on a member that it doesn't contain. Things get all nilly.  
If I call this set on a member it does contain, the member will be returned from the set.

As an example:
--------------
```clojure
user=> (def daves-i-know (conj #{} "Dave" "Davey" "David" "Davo"))
#'user/daves-i-know
user=> (daves-i-know "Davidicus")
nil
user=> (daves-i-know "Dave")
"Dave"
user=> 
```
