---
layout: post
title:      "Building Blocks : Tetris Javascript Project"
date:       2020-12-22 02:28:29 +0000
permalink:  building_blocks_tetris_javascript_project
---


Building this Project was fun and exciting for me! I created a Tetris game with Javascript, CSS and HTML as well! Throughout the planning of this project, I needed to know how to manipulate the DOM in my application. The DOM stands for Document Object Model. It represents the page so that programs can change the document structure, style, and content. The DOM represents the document as nodes and objects. That way, programming languages can connect to the page.

```
document.addEventListener('DOMContentLoaded', () => {
    const grid = document.querySelector('.grid')
    let squares = Array.from(document.querySelectorAll('.grid div'))
    const scoreDisplay = document.querySelector('#score')
    const startBtn = document.querySelector('#start-button')
```

Getting the blocks to stop on the page was a task on its own. However, thats when my Event Handlers came into play. Thats the beauty of javascript. But lets pause for a second and review what an event is. 


Events are fired inside the browser window, and tend to be attached to a specific item that resides in it — this might be a single element, set of elements, the HTML document loaded in the current tab, or the entire browser window. There are many different types of events that can occur. For example:

The user selects a certain element or hovers the cursor over a certain element.
The user chooses a key on the keyboard.
The user resizes or closes the browser window.
A web page finishes loading.
A form is submitted.
A video is played, paused, or finishes.
An error occurs.


Each available event has an event handler, which is a block of code (usually a JavaScript function that you create) that runs when the event fires. When such a block of code is defined to run in response to an event, we say we are registering an event handler. The EventTarget method addEventListener() sets up a function that will be called whenever the specified event is delivered to the target. Here is an example of using a addEventListener() for the start and pause button for my application:

```

//adding start and pause button 
startBtn.addEventListener('click', () => {
    if (timerId) {
        clearInterval(timerId)
        timerId = null 
    } else {
        draw()
        timerId = setInterval(moveDown, 1000)
        nextRandom = Math.floor(Math.random()*theBuildingblocks.length)
        displayShape()
    }
})
```

This project chanlleged me in manys ways, but I am excited to have put my coding skills to the test! Can't wait for the next project! 


