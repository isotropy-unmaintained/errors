Filter Argument Count
=====================

The filter() method should only have a single parameter.

The follow is valid.
```javascript
async function getTodos(who) {
  return db.todos.filter(t => t.assignee === who);
}
```

The follow is NOT valid because the filter function has two parameters; t and x.
```javascript
async function getTodos(who) {
  return db.todos.filter((t, x) => t.assignee === who);
}
```
