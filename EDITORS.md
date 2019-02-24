This file includes instructions for adding new books to the site.

Adding a new book
=================

- Create a new file in the `_books` directory with the name of the book followed by `.md`, for example if the book is called "My Amazing Story", create a new file called `my-amazing-story.md`.
- Copy-paste the following template into the new file, and complete the fields as required, eg. if the ISBN was "123456789", you'd end up with `isbn_physical: 1234567890`.
  ```
  ---
  title: 
  author: 
  translation: 
  isbn_physical: 
  isbn_ebook: 
  region: 

  amazon: 
  goodreads: 

  cover:  /assets/images/...
  permalink: /...

  layout: book
  ---
  Description of the book goes here.
  ```
  - If something doesn't apply for the current book (e.g. perhaps there is no eBook ISBN or no translator), just leave those bits blank.
  - Make sure that the `---` at the start and end of the metadata section is not accidentally lost.
- Upload the book cover image to the `assets/images` directory with the same naming convention as the file above, e.g. `my-amazing-story.jpg`

