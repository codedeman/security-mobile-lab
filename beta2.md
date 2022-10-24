
There’s another way of using GCD, and it’s worth covering because it’s a great deal easier in some specific circumstances. It’s called performSelector(), and it has two interesting variants: performSelector(inBackground:) and performSelector(onMainThread:).

Both of them work the same way: you pass it the name of a method to run, and inBackground will run it on a background thread, and onMainThread will run it on a foreground thread. You don’t have to care about how it’s organized; GCD takes care of the whole thing for you. If you intend to run a whole method on either a background thread or the main thread, these two are easiest.

For project 7, we can use this method to clear up the confusion with our showError() method. For example, we could refactor the fetching code into a fetchJSON() method that can then run in the background like this:
