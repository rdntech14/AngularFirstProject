
### What is SPA (Single Page Application)
SPA is single page applicatin , where you have only one view and which gets updated with dynamic contents to display , spa is basically application for mutiple devices like mobile , ipad, tablets and TV etc.

### Advantages
 Single Page Application is good for making Responsive Websites, Support mobile, Tablet & Desktop. No extra queries to the server to download pages. Performance improvement, Single Page Application can improve performance in many ways, Single time file load each of HTML, CSS, JS

 Since single-page applications don't update the entire page but only required content, they significantly improve a website's speed. Most resources (HTML/CSS/Scripts) are only loaded once throughout the lifespan of an application. Only data is transmitted back and forth

### Why do we need Asynchronous work?
The simple answer is we want to improve the user experience. We want to make our application more responsive. We want to deliver a smooth user experience to our users without freezing the main thread, slowing them down and we don’t want to provide the jenky performance to our users. We also want to do heavy work and complex calculations on our servers as mobile devices are not very powerful to do the heavy lifting. So we need asynchronous work for network operations.

### What exactly are asynchronous data streams?

**Asynchronous** -  in JavaScript means we can call a function and register a callback to be notified when results are available, so we can continue with execution and avoid the Web Page from being unresponsive. This is used for ajax calls, DOM-events, Promises, WebWorkers and WebSockets.

**Data**, raw information in the form of JavaScript data types as: Number, String, Objects (Arrays, Sets, Maps).

**Streams**, sequences of data made available over time. As an example, opposed to Arrays you don’t need all the information to be present in order to start using them.

### What is Reactive Programming? (Rx Programming)
s
Reactive Programming Is Programming With Asynchronous Data Streams

Reactive programming is an asynchronous programming paradigm concerned with data streams and the propagation of change.

RX = OBSERVABLE + OBSERVER + SCHEDULERS

**Observable**: An Observable is a stream of values emitted over time. Observable packs the data that can be passed around from one thread to another thread. They basically emit the data

**Observers**: Observers consumes the data stream emitted by the observable. Observers subscribe to the observable

**Schedulers**: Remember that Rx is for asynchronous programming and we need a thread management. There is where schedules come into the picture. Schedulers are the component in Rx that tells observable and observers, on which thread they should run.

### What is RxJS
RxJS stands for *R*eactive E*x*tensions for *J*ava*S*cript, and its a library that gives us an implementation of Observables for JavaScript in Angular.
