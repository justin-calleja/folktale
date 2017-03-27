@annotate: folktale.data.task
category: Asynchronous Actions
---

A data structure that models an asynchronous action, as well as how any
resources associated with the asynchronous action are allocated and collected.

A `Task` helps with representing asynchronous actions without actually
executing them. This allows us to write pure functions which combine and
transform our `Task`s until we're ready to execute them and trigger any side
effects. Apart from lazy execution, we also get the ability to cancel
asynchronous actions and an automated (callback) way of cleaning up any
resources consumed by running our asynchronous actions. These are all features
which are not offered by constructs such as
[Promise](http://www.ecma-international.org/ecma-262/6.0/#sec-promise-constructor).


