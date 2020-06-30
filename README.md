# ZacharyKatancik-Book
# Pro MERN Stack 2nd Edition book project


## Chapter 10

Lot's of new features this chapter! Depending on the section, we either worked on the front-end or the back-end, implementing each side of our new features. In chapter 10, we added the capability to filter our issues by effort, to edit our issues, and send them to the database, as well as delete issues, send them to a "trash collection" and then implement that in the ui.

A lot of the under the hood work that occured in this chapter had to do with the user inputting text, allowing for queries to be out of sync, then when a use hits a button, resyncing them if valid or reloading the field if invalid. This required a surprising amount of code to make happen correctly and efficiently. However, once we sort of got the hang of allowing temporary asyncronicities, then a submit button validating, we were able to reuse a lot of the ideas used early on in the effort filter and the edit issue functions on the close and delete functions later. 

![master](/readme_images/ch10-1.png)
![master](/readme_images/ch10-2.png)


---


## Chapter 9

To begin with Chapter 9, we installed the React Router, which allows us to route requests on the client side as opposed to the server side. As a part of this, we rewrote the parts of our code that handled URL queries, first using hashrouting, and then browser routing.

In terms of functionality, we added a navigation bar, a filter drop down, and a long description select button. These each make use of URL queries in slightly different ways. The picture below shows our new hyperlinks and the active link color we added to indicate the active link, as well as the URL change, and the long description shown for issue ID 1.

The last thing we did was a quick adjustment, converting our code from using a hash router to a browser router.


![master](/readme_images/ch9-1.png)


---


## Chapter 8

In this chapter we continued to make tweaks to our existing javascript to make it more modular, both from a loading and compiling standpoint and a visual one for developers. We installed a tool called Webpack that allowed us to connect these modular pieces, as JS was not originally intended to work in a modular fashion. 

As well, we installed Webpack Hot Module Replacement. As I understand it, this kind of works like a regular version control system, where when changes are made to one module, the changes are saved and recompiled, not the entire application. This saves time as a developer and could impact users so the entire app doesn't have to be rebuilt if tweaks are deployed. In the end, we also installed a debugging feature called sourcemaps, which allows us to debug our code without having to look at the raw JS.


![master](/readme_images/ch8-1.png)


---


## Chapter 7

Chapter 7 was about separating our front end and our backend, adding a proxy for safety around cookie useage, and lastly, linting our code to adhere to the Airbnb lint standard. To split our front-end and back end, we divided our code into api (back-end) and ui (front-end). These each now include their own server, the api server runnning coordination from MongoDB and waiting for user requests, and the ui server, which hosts index.html and the display properties of the issuetracker. 

Each of these split components contain their own .eslintrc files. These files, along with the installed eslint software, allowed us to check the code style of our js files. In the book, we use Airbnb's js code-style standards. Much of the code changes I did included fixes to standardize the code to the linter. Much of that time devoted to changing my indentation from increments of 4 spaces to increments of 2. Lastly, after getting a clean lint on each file, we added a proptype check to the issueadd function in our App.jsx file.


![master](/readme_images/ch7-1.png)
![master](/readme_images/ch7-2.png)


---


## Chapter 6

In this chapter we learned allllllll about MongoDB, working in the mongo shell, common command line arguments for adding, filtering, preventing duplictes, clearing, etc. documents from the database. We learned how to format new documents in the database and how to categorize/  index them. As well, we installed mongodb in our issue tracker application, and set up an initialize database file for it. Lastly, made changes to the server to allow changes to be appended and read from the database, as opposed to program memory. Our newest server code stores and reads all server-side info from a mongoDB database called issuetracker.


![master](/readme_images/ch6-1.png)


---


## Chapter 5

In this chapter we discussed and worked with Express, REST API, GraphQL, displaying errors, and valudation checks at a server query level. A large chuck of the chapter is using GraphQL to test our back-end in querying, mutating, and error-handling at a server level. In the screenshots below, I used a couple of hand-writen sever queries to pull information from our task manager and for checking an invalid input error. 

Though discussed briefly, and if I'm understanding correctly, we chose to use GraphQL as our API standard instead of REST. To explore this, we can explore our functionality thorugh the Playground tool that is paired with GraphQL. As well as noted in the books summary and towards to beginning of the book, we're using a CRUD (Create, Read, Update, Delete) approach. pattern in this implication. And the goal of these tools is to create and read tasks on the server side for eventual database-side storage and updating, and eventually ability to delete. 

We also used Express, which is a router for different requests that a user inputs and the server outputs. Using Express, our application takes requests and matches them to a route. For example, a GET request will be mapped to our in-built get() method. Built into express are several properties of request and response objects that we can use with Middleware functions. 


![master](/readme_images/ch5-1.png)
![master](/readme_images/ch5-2.png)


---


## Chapter 4

In this chapter we worked with state and props, as well as handling user input through a text submit box. We talked about state changes with parent's and children, and how to respect that hierarchy structure. We also talked about how only parents and children can communicate, nothing outside, like a sibling inheritence relationship. In the end of the chapter, we worked with stateless components and converting them to pure functions. Overall, a ton of meat in this chapter with lots of unfamiliar JS/React specific details, syntax, and state being a new topic for me.

![master](/readme_images/ch4-1.png)


---


## Chapter 3

In this chapter we began the issue tracker project as mentioned to be the main project in the book. We used tables and classes, as well as built the project using a .jsx file and node to build our .js file. We also learned how to set up classes in React, and how to pass information between classes within our .jsx file. Still getting used to the syntax of everything React, it seems that passing information as parameters to other files and functions is different than I 've seen in the past, as well, getting used to the act of mixing in the html and css elements into the JS stuff and how that all works.

![master](/readme_images/ch3-1.png)


---


## Chapter 2

I was able to implement a Hello World! application both with an intro to server implementation and server-less. While following along in the book, we used several different node, express, react applications to modify our raw input javascript for different browser compatibility, and implementations for dividing up our code across files and directories. We also used in-built applications to refactor our code to split theses files up, and tell the computer and server where to look to find these instructions. Overall, I had a hard time completely understanding what I was doing while following these instructions at an in-depth level, but did get a general idea on most topics.

![master](/readme_images/ch2-1.png)

![master](/readme_images/ch2-2.png)