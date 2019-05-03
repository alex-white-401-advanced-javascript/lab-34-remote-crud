![CF](http://i.imgur.com/7v5ASc8.png) LAB 34
=================================================

## Remote CRUD

### Author: Alexander White

### Links and Resources
* [PR]()
* [CodeSandbox]()

### Modules
#### React Components
##### `index.js`
Entry point for React application. Establishes connection with Redux store by wrapping `App` in `<Provider />`.

##### `app.js`
Class component that connects to Redux store `get` and `destroy` actions and all `records` stored in the store's state. Renders a list of records with "Edit" and "Delete" buttons, which trigger actions.

##### `record.js`
Class component that connects to Redux store `post`, `put`, and `patch` actions and the `activeRecord` stored in the store's state. Makes a `GET` request to an API server and a form based on the JSON schema returned. When the form is submitted, triggers the appropriate CRUD action based on what was entered:
* new record - `post`
* updating entire record - `put`
* updating parts of record - `patch`

#### UML
![UML Diagram]()
