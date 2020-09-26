## Event Driven Programming:
- In computer programming, event-driven programming is a programming paradigm in which the flow of the program is determined by events such as user actions (mouse clicks, key presses), sensor outputs, or messages from other programs or threads.
- Event driven programming is flexible as the programming code follows a logical order from start to finish and the flow is determined by events. This allows the coder to be flexible about the order in which they carry out the code.

- Most actions in JS are event driven
>- UI Events
>- Express Routes
>- Model Lifecycle Hooks
>- React

- A Main Loop listens for event triggers and calls the associated event handler for that event.
- An Event Handler is a callback function that will be called when an event is triggered.

## EventEmitter:
- it allows us to get started incorporating Event-Driven Programming in our project right away.

## Removing Listeners;
- To remove event listeners in EventEmitter we can use the removeListener or removeAllListeners method.