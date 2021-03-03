---
layout: post
title:      "The Marathon Continues "
date:       2021-03-03 14:01:07 +0000
permalink:  the_marathon_continues
---


For my last Flatiron project, I created a Trello clone that would allow users to manage their dashboards for projects, to-do list etc. The idea sprung upon me during a work meeting. I knew that for my final project, I wanted to create an application that I could use in the future and build upon the application after my graduation from the Flatiron program. In the early stages of the project build, I debated on implementing user authentication. After deciding to forgo that step in my applicaiton, that is the first step adding modifications to the application. 

There were many struggles building this application, and understanding redux was definetely one of the many causes of bugs and issues that I faced. Redux is a predictable state container designed to help you write JavaScript apps that behave consistently across client, server, and native environments and are easy to test. What a great tool right? After I figured out redux, I came acorss another obstacle. How can I drag and drop my lists and cards across the application to get a similar feel to the real trello application? 

The Answer.... DnD. Drag and drop is a very widely seen easy to use feature that adds great convenience to your users. But it is always a huge task if implemented using vanilla JavaScript as it will include huge calculations depending on its implementation (such as dropping in a list ). But React comes up very handy in drag and drop (or simply dnd) feature.  
```
//Step 1. Make the list first with its children being draggable
//Step 2.  The next task is to keep track of the item being dragged
//Step3. We will try to find over which child it is hovering at any given time
//Step 4. Our last step is to reshuffle the list when you finally drop the element over any of the other children
```

The npm package that I installed that would allow me to follow these steps can be found here: [https://github.com/atlassian/react-beautiful-dnd/blob/master/docs/about/installation.md]. 


Overall, this project challenged me in every way possible. With my journey coming to an end here at Flatiron, I am excited to open the next chapter in my coding journey! 

