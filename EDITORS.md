This file includes instructions for adding new books to the site.

Adding a new book
=================

- Create a new file in the `_books` directory with the name of the book followed by `.md`, for example if the book is called "My Amazing Story", create a new file called `my-amazing-story.md`.
  - Your best approach would be to copy-paste the conent of an
  existing booking book's file.
  - At the top of the file there is some metadata - everything between the first `---` and last `---` (e.g. the name of the author, the ISBN, the links to Amazon etc) needs to be updated for each book.
    - If something doesn't apply for the current book (e.g. perhaps there is no eBook ISBN or no translator), just leave those bits blank.
  - Anything after the last `---` will be shown as text on the page.  This would be a good place to put reviews and other info about the book.
- Upload the book cover image to the `assets/images` directory with the same naming convention as the file above, e.g. `my-amazing-story.jpg`

