<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Simple To‑Do (localStorage)</title>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>
  <main class="app" id="app">
    <h1>To‑Do List</h1>

    <form id="todo-form" aria-label="Add todo">
      <label for="todo-input" class="visually-hidden">New todo</label>
      <input id="todo-input" name="todo" type="text" placeholder="What needs to be done?" autocomplete="off" required />
      <button type="submit" id="add-btn">Add</button>
    </form>

    <section class="controls">
      <div class="filters" role="tablist" aria-label="Filter todos">
        <button class="filter active" data-filter="all" role="tab" aria-selected="true">All</button>
        <button class="filter" data-filter="active" role="tab" aria-selected="false">Active</button>
        <button class="filter" data-filter="completed" role="tab" aria-selected="false">Completed</button>
      </div>
      <div class="actions">
        <button id="clear-completed">Clear completed</button>
      </div>
    </section>

    <ul id="todo-list" class="todo-list" aria-live="polite"></ul>

    <footer class="footer">
      <span id="items-left">0 items left</span>
    </footer>
  </main>

  <script src="app.js" defer></script>
</body>
</html>
