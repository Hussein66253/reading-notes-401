- To manage routes you need to have separate modules from the main server, allowing to extract the logic, so routing changes the roles of the files in the server, the index.js is the Entry point, server.js is the exported server, models are for data and are known as data models, routes are for the routes and handlers.

## Express API?
 - The way to construct a web API is to follow the RESTful approach . REST APIs are resource-based interfaces. On the web this means that data resources are represented by URIs (paths) accessed via HTTP.

## routing in Express?
 - Routes can be managed in separate modules from the main server, Routing refers to how an application’s endpoints (URIs) respond to client requests.

 - You define routing using methods of the Express app object that correspond to HTTP methods; for example, `app.get()` to handle GET requests and app.post to handle POST requests.

 - Express 4.0 comes with the new Router. Router is like a mini express application. It doesn't bring in views or settings, but provides us with the routing APIs like **.use, .get, .param,** and **route**.

## Express Middleware
 - Express Middleware A series of functions that the request goes throug Each function receives **request**, **response** and **next** as *parameters*

 - Route Middleware `router.use()` Route middleware in Express is a way to do something before a request is processed. This could be things like checking if a user is authenticated, logging data for analytics, or anything else we'd like to do before we actually spit out information to our user.

## Route parameters
 - Route parameters are named **URL segments** that are used to capture the values specified at their position in the URL. The captured values are populated in the **req.params** object, with the name of the route parameter specified in the path as their respective keys.