## To-do App 

This project is part of a intensive React training by Rocketseat, this is the first challenge.

# Challenge
 - Create a new task with a random id, don't allow to create if the title was empty
 - Change between true or false the field "isComplete" of a task based on id
 - Remove a task based on id.

# Solution
- To create the task, I've decided to create the id with `Date.now() / Math.random()`, so I used a useState to set the task based on the input value.
- To change the value, I've made a `map()` and inserted a condition to check if the `task.id` was equal `id` (parameter), when I found the item, I returned the isComplete with !task.isComplete, in this way the user can check and uncheck the item.
- To remove, I've made a `filter()` to search the item using the id and I returned the items differents of the return.

