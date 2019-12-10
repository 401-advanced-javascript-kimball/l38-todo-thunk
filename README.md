# l38-todo-thunk

* [submission PR](https://github.com/401-advanced-javascript-kimball/l38-todo-thunk/pull/1)
* [travis](https://travis-ci.com/401-advanced-javascript-kimball/l38-todo-thunk)

# LAB - 

## Project Name

### Author: Student/Group Name

### Links and Resources
* [submission PR](http://xyz.com)
* [travis](http://xyz.com)
* [back-end](http://xyz.com) (when applicable)
* [front-end](http://xyz.com) (when applicable)

#### Documentation
* [api docs](http://xyz.com) (API servers)
* [jsdoc](http://xyz.com) (Server assignments)
* [styleguide](http://xyz.com) (React assignments)

### Modules
#### `modulename.js`
##### Exported Values and Methods

###### `foo(thing) -> string`
Usage Notes or examples

###### `bar(array) -> array`
Usage Notes or examples

### Setup
#### `.env` requirements
* `PORT` - Port Number
* `MONGODB_URI` - URL to the running mongo instance/db

#### Running the app
* `npm start`
* Endpoint: `/foo/bar/`
  * Returns a JSON object with abc in it.
* Endpoint: `/bing/zing/`
  * Returns a JSON object with xyz in it.
  
#### Tests
* How do you run tests?
* What assertions were made?
* What assertions need to be / should be made?

#### UML
Link to an image of the UML for your application and response to events

----------

# LAB - Remote APIs

Using asynchronous action creators via 'thunk', wire CRUD functionality into the To Do application, with Redux

## Before you begin
Refer to *Getting Started*  in the [lab submission instructions](../../../reference/submission-instructions/labs/README.md) for complete setup, configuration, deployment, and submission instructions.

## Getting Started

Starter code has been provided for you in the `/lab/starter-code` folder. 

Open [Code Sandbox](http://codesandbox.io) and Create a new application. When prompted, choose "From GitHub" and then paste in the URL to today's starter code folder from your fork of the class repository.

You will be submitting the URL to this working sandbox as part of your assignment.

## Assignment
### To Do - Reduxified and Fully Connected
* Upgrade the provided `todo` application 
* Keep the settings context in place so that you can manage those options within the components
* Use Redux for global state management
* For the to do form, if you're using JSON Schema Forms ...
  * Fetch the To Do schema from the server in the form component on it's initial render
  * Bonus points if you do this with `<Suspense>`
  * Convert the To Do forms to use the live schema
* For all CRUD ops, convert the native `fetch...()` calls from being in the components to instead invoking action methods
  * These should return functions that dispatch the real action
  * You'll need to have `thunk` in place to make this work
* Update the results in the store
  * **Question** -- Do you update the full store after every write operation or do you try and keep your store in sync manually?  How you approach/answer this will determine what action(s) you dispatch.

### Styling
* Clearly, this needs a little bit of TLC
* Use your generic design to apply core styling and layout
* Use your creativity ...
  * A pop-up modal for the details instead of a simple list?
  * Accordions?
  * Slide Out?
  * Rotator?

### Testing
* tests that ensure the list module functions correctly with error-check parameters

### Stretch Goals:
* Paginate the results.  The initial calls to the people list will give a total number people, pages, and a link to the next page.
* Create a new component for navigation that will use those links to draw a list of pages to fetch, and then keep re-calling that initial fetch method to update the list based on what page you are "on"
* Multi-User / Event Driven ... Once you're fully wired for CRUD, re-integrate the Q connection (the `useQ()` hook) and do event driven updates

### Assignemnt Submission Instructions
Refer to the the [lab submission instructions](../../../reference/submission-instructions/labs/README.md) for the complete lab submission process and expectations

----------

