# Library
A dynamic, browser-based digital library built with JavaScript, HTML, and CSS. Users can store, manage, and display a collection of books by interacting with a form and dynamically updating the DOM. 

## Features

- Add new books with a form (title, author, page count, read status).
- Each book is assigned a unique ID using `crypto.randomUUID()`.
- Display books as cards or rows using dynamic DOM manipulation.
- Remove books from the library with a dedicated delete button.
- Toggle a book’s read status via a prototype method.
- Maintains a clear separation between data (book objects) and presentation (DOM).

## Concepts Practiced

- **Object-Oriented JavaScript**: Using constructors and prototypes.
- **DOM Manipulation**: Dynamically creating, modifying, and deleting elements.
- **Event Handling**: Responding to user interactions.
- **Form Handling**: Preventing default form behavior with `event.preventDefault()`.
- **Data Binding**: Associating DOM elements with data using `data-*` attributes.
- **Code Modularity**: Keeping data logic and display logic separated.

## How It Works

- All books are stored in an array named `myLibrary`.
- A constructor function (`Book`) is used to create book objects.
- A separate function (`addBookToLibrary`) takes input, creates a new book, and adds it to the array.
- Each book is displayed on the page via a rendering function that loops through `myLibrary`.
- Buttons are provided for:
  - Deleting books (using their unique `id`)
  - Toggling their read status (via a prototype method)
