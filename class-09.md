# express()
 - `express()`the Creates an Express application. 
 - The express() function is a top-level function exported by the express module.
## express.json([options])
 - This is a built-in middleware function in Express. It parses incoming requests with JSON payloads and is based on body-parser.
 - Returns middleware that only parses JSON and only looks at requests where the Content-Type header matches the type option.
 - This parser accepts any Unicode encoding of the body and supports automatic inflation of gzip and deflate encodings.
## express.Router([options])
 - Creates a new router object.
## express.static(root, [options])
 - This is a built-in middleware function in Express. It serves static files and is based on serve-static.
## express.urlencoded([options])
 - This is a built-in middleware function in Express. It parses incoming requests with urlencoded payloads and is based on body-parser.
 - Returns middleware that only parses urlencoded bodies and only looks at requests where the Content-Type header matches the type option.
 - This parser accepts only UTF-8 encoding of the body and supports automatic inflation of gzip and deflate encodings.
## Middleware
 - Middleware are functions which are passed control during execution of asynchronous functions.
 - Middleware is specified on the schema level and is useful for writing plugins.
 ### Types of Middleware
 - document middleware
 - model middleware
 - aggregate middleware
 - query middleware
## Use Cases
 - complex validation
 - removing dependent documents (removing a user removes all his blogposts)
 - asynchronous defaults
 - asynchronous tasks that a certain action triggers
## Subdocuments
 - Subdocuments are documents embedded in other documents. In Mongoose, this means you can nest schemas in other schemas.
 - Mongoose has two distinct notions of subdocuments: arrays of subdocuments and single nested subdocuments.
 - What is a Subdocument?
   - Subdocuments are similar to normal documents. Nested schemas can have middleware, custom validation logic, virtuals, and any other feature top-level schemas can use.

## Adding Subdocs to Arrays
 - MongooseArray methods such as push, unshift, addToSet, and others cast arguments to their proper types transparently.
## Populate
 - Population is the process of automatically replacing the specified paths in the document with document(s) from other collection(s).
## Setting Populated Fields
 - You can manually populate a property by setting it to a document.