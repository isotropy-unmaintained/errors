Filter Parameter Count
======================

The filter() method should only have a single parameter.

The follow is valid.
```javascript
async function getTodos(who) {
  return db.todos.filter(todo => todo.assignee === who);
}
```

The follow is NOT valid, because the filter function has two parameters: todos and x.
```javascript
async function getTodos(who) {
  return db.todos.filter((todos, x) => todo.assignee === who);
}
```
