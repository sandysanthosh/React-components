<!-- portfolio-docs-v1 -->
# React Components

> A learning project exploring React components and front-end composition.

## Repository Context

| Item | Details |
|---|---|
| Project type | Learning project |
| Technologies | React, JavaScript, HTML, CSS |
| Primary focus | Reusable UI components and client-side development |
| Status | Historical learning project. |

## What This Repository Demonstrates

- Practical, hands-on exploration of **reusable ui components and client-side development**
- Ability to organise examples and technical material for later reuse
- Breadth across web, backend, API, and software-engineering concepts

## Getting Started

Install dependencies with `npm install`, then run `npm start` when a package manifest is present.

### Key contents

`package-lock.json`, `package.json`, `public`, `src`

## Portfolio Note

This repository is part of my earlier learning and experimentation archive. My current professional focus is **Java, Spring Boot, microservices, REST APIs, Kafka, cloud-native engineering, and banking technology**. See my [GitHub profile](https://github.com/sandysanthosh) for current positioning and featured work.

---

## Original Documentation

# React Crash Course (TodoList)

This is the code for the crash course on YouTube

## Quick Start

```bash
# Install dependencies
npm install

# Serve on localhost:3000
npm start

# Build for production
npm run build
```
react is a javascript library

mainly used for UI

make-end javscript much eaasier
much more interactive ui
virtual dom

JXS-easily incorporate js in markup

easy to work with teams

CLI tool for creating react

anatomy og component:

class based compoent:

class post extends react.component{

state={

title:'post one',
body: 'this is my post',
}

render(){
return{
<div>
<h3>{ this.state.title } </h3>
<p>{ this.state.body } </p>
</div>
}



to install:

creater react app using npm:

->package.json:

dependency information
react version
react native- mobile apps
react script- dev server

script:

start scripts


public:

index.html- single page application framework

<div id="root"></div>   - main app components inside this app



->index.js:

importing all components:

react,reactDom,

document.getelementByID('root')->this refers to 

main app root

->APP.js:

import react and compoents

mainapp.css - global method

render()- life cycle method

{} - include javascript here

jsx: class name


#### React CRUD

```

import React, { useState } from "react";

const App = () => {
  const [todos, setTodos] = useState([
    { id: 1, task: "Buy groceries" },
    { id: 2, task: "Do laundry" },
  ]);

  const addTodo = (task) => {
    setTodos([...todos, { id: todos.length + 1, task }]);
  };

  const removeTodo = (id) => {
    setTodos(todos.filter((todo) => todo.id !== id));
  };

  const updateTodo = (id, updatedTask) => {
    setTodos(
      todos.map((todo) =>
        todo.id === id ? { ...todo, task: updatedTask } : todo
      )
    );
  };

  return (
    <div>
      <h1>Todo List</h1>
      <ul>
        {todos.map((todo) => (
          <li key={todo.id}>
            {todo.task}
            <button onClick={() => removeTodo(todo.id)}>Remove</button>
            <button onClick={() => updateTodo(todo.id, "Updated task")}>
              Update
            </button>
          </li>
        ))}
      </ul>
      <button onClick={() => addTodo("New task")}>Add Todo</button>
    </div>
  );
};

export default App;


```

