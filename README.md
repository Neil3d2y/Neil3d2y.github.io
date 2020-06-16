# Patatap Project

Use Paperscript internally in HTML
1. to make VSCode syntax highlighting
```diff
![C:\Users\{user name here}\AppData\Local\Programs\Microsoft VS Code\resources\app\extensions\html\syntaxes\html.tmLanguage.json
```
Update above file with the part `paperscript`


2. Why to do that
[Cross Origin Resource Sharing](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS)

Cross-Origin Resource Sharing (CORS) is a mechanism that uses additional HTTP headers to tell browsers to give a web application running at one origin, access to selected resources from a different origin. A web application executes a cross-origin HTTP request when it requests a resource that has a different origin (domain, protocol, or port) from its own.

For security reasons, browsers restrict cross-origin HTTP requests initiated from scripts. For example, XMLHttpRequest and the Fetch API follow the same-origin policy. This means that a web application using those APIs can only request resources from the same origin the application was loaded from unless the response from other origins includes the right CORS headers.


## ingredients

1. [paperjs](http://paperjs.org/)

2. [Neuronal Synchrony](https://github.com/jonobr1/Neuronal-Synchrony) `assets/A`


### canvas
[canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial)

`<canvas>` is an HTML element which can be used to draw graphics via scripting (usually JavaScript). This can, for instance, be used to draw graphs, combine photos, or create simple (and not so simple) animations. The images on this page show examples of `<canvas>` implementations which will be created in this tutorial.


To Use:
1. create a `canvas` element in `<body>` and assign with an Id
2. write paperscript in HTML referencing to the `canvas`



### Paper.js
Animation Library

#### Global Scope 
[View](http://paperjs.org/reference/view/)

use boave to get the size of visible area in project coordinates.

#### Mathmatical Operations
[algebraic operators](http://paperjs.org/tutorials/geometry/mathematical-operations/)
```
// Define a point to start with
var point1 = new Point(10, 20);

// Create a second point that is 4 times the first one.
// This is the same as creating a new point with x and y
// of point1 multiplied by 4:
var point2 = point1 * 4;
console.log(point2); // { x: 40, y: 80 }

// Now we calculate the difference between the two.
var point3 = point2 - point1;
console.log(point3); // { x: 30, y: 60 }

// Create yet another point, with a numeric value added to point3:
var point4 = point3 + 30;
console.log(point4); // { x: 60, y: 90 }

// How about a third of that?
var point5 = point4 / 3;
console.log(point5); // { x: 20, y: 30 }

// Multiplying two points with each other multiplies each 
// coordinate seperately
var point6 = point5 * new Point(3, 2);
console.log(point6); // { x: 60, y: 60 }
```

### Howler.js
[Howler.js](https://github.com/goldfire/howler.js/#quick-start)
Audio Library

```
var sound = new Howl({
  src: ['sound.mp3']
});
 
sound.play();
```