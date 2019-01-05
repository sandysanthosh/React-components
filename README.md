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
