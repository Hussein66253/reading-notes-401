## Redux - Asynchronous Actions
### Redux Thunk
- Redux Thunk is a middleware that lets you call action creators that return a function instead of an action object. That function receives the store's dispatch method, which is then used to dispatch regular synchronous actions inside the body of the function once the asynchronous operations have completed.
- Redux Thunk middleware allows you to write action creators that return a function instead of an action.
- The thunk can be used to delay the dispatch of an action, or to dispatch only if a certain condition is met. 
- The inner function receives the store methods dispatch and getState as parameters.
- Redux Thunk looks for these special functions and handles the dispatching for you. This pattern allows you to centralize and re-use these services in different components. 
- This especially comes handy when you are making asynchronous API requests and you need to dispatch on promise success and error.
- The most common use-case for Redux Thunk is for communicating asynchronously with an external API to retrieve or save data.
- Redux Thunk makes it easy to dispatch actions that follow the lifecycle of a request to an external API.

### React Suspense
- Suspense is a new React feature that was announced recently at the JSConf Conference in Iceland. 
- It aims to help with handling async operations respectively in regard to CPU power and data fetching.
- Suspense allows you to defer rendering part of your application tree until some condition is met (for example, data from an endpoint or a resource is loaded).