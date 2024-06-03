# Todo-list

1. Stwórz interaktywną listę zadań, gdzie użytkownicy będą mogli dodawać oraz usuwać istniejące zadania.

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>To-Do List</title>
  <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
</head>
<body>
  <div class="container mt-5">
    <h1 class="text-center">To-Do List</h1>
    <div class="input-group mb-3">
      <input type="text" class="form-control" id="taskInput" placeholder="Add a new task">
      <div class="input-group-append">
        <button class="btn btn-primary" id="addTaskBtn">Add Task</button>
      </div>
    </div>
    <ul class="list-group" id="taskList"></ul>
  </div>
  <script></script>
</body>
</html>
```
