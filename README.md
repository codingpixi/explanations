# explanations

##6.3: Talking About the Back End

**routes (routes/catalog.js)**
- acts as a front end to MongoDB (which is an open source NoSQL DB that uses a document-oriented data model).
- is a MongoDB object modeling tool designed to work in an asynchronous environment.
- schema-based solution to model your application data. It includes built-in type casting, validation, query building, business logic hooks and more, out of the box.

**controller (controllers/authorController.js)**
- virtual properties
- controller functions to get the requested data from the models, create an HTML page displaying the data, and return it to the user to view in the browser.

**model models/Author.js and models/Book.js**
- are created using schemas from the mongoose.model( ) method
- models are defined using the schema interface.

**schemas**
- allows you to define the fields stored in each document along with their validation requirements and default values.
- a schema can have an arbitrary number of fields - each one represents a field in the document stored in MongoDB

**virtuals**
- virtual properties are document properties that you can get and set but that do not set persisted to MongoDB.

**views (views/author_detail.pug)**
- values to specify the folder where the template will be stored. Next set the view engine value to specify the template library.

**mongoose**
- is a MongoDB object modeling tool designed to work in an asynchronous environment
- provides a straight-forward, schema-based solution to model your application data. It includes built-in type casting, validation, query building, business logic hooks and more, out of the box.
- acts as a front end to MongoDB (which is an open source NoSQL DB that uses a document-oriented data model).
- is a MongoDB object modeling tool designed to work in an asynchronous environment.
- schema-based solution to model your application data. It includes built-in type casting, validation, query building, business logic hooks and more, out of the box.

**a pug template**
- template rendering engine
- uses a representation of HTML where the first word in any line usually represents an HTML element, and indention of subsequent lines is used to represent any content nested within those elements *(using different markup languages that can be compiled into HTML)*
- formerly known as Jade

[MDN Resource](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs)

From the site http://localhost:3000/catalog/author/58f7843f1c671a306efc7dc4 which is from the local server we developed utilizing npm. After clicking on the All Authors to Isaac Asimov link the URL pattern is (route) decision of the action is based on the POST and GET data which reads the information from the database. In this time the method specifies what template view is to be used to display the page that has the authors information.

The catalog.js file is handling the routing based on the URL link requested and responding with the locations assigned by the HTML verb GET. The authorController.js file is orchestrating how to handle the virtual information compiled or the errors that may occur.

Mongoose is the schema solution used to model this application.
