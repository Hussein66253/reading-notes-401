## Custom Hooks
- Custom Hooks offer the flexibility of sharing logic that wasn’t possible in React components before. 
- You can write custom Hooks that cover a wide range of use cases like form handling, animation, declarative subscriptions, timers...etc
- useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one.
- useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks.
- Hooks return data or behaviors (functions) that are required to reuse their internal functionality
- Hooks are imported into components