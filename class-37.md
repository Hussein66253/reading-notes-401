## combineReducers
- The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore. 
- The resulting reducer calls every child reducer and gathers their results into a single state object.
- combineReducers is a utility function to simplify the most common use case when writing Redux reducers.
- combineReducers enforces several rules to help users avoid common errors.
- In order to assemble the new state tree, combineReducers will call each slice reducer with its current slice of state and the current action, giving the slice reducer a chance to respond and update its slice of state if needed.
- It's very common to have multiple combined reducers in various places, which are composed together to create the root reducer.

### State Shape
- createStore function can take preloadedState as its second argument.
- combineReducers takes an object full of slice reducer functions, and creates a function that outputs a corresponding state object with the same keys. This means that if no preloaded state is provided to createStore, the naming of the keys in the input slice reducer object will define the naming of the keys in the output state object. 