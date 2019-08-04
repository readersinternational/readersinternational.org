# Documenation for Editors
This file includes instructions for adding new books to the site.

## Adding a new book

* Take the title of the book and create a hyphenated-name for it, for example if the book is called "My Amazing Book", the hyphenated-name will be `my-amazing-book`. We'll be using this in several places.
* Create a new file in the `_books` directory with the hyphenated-name of the book followed by `.md`, for example `my-amazing-book.md`.
* Copy-paste the following metadata template into the top new file (make sure that the `---` is the first thing on the first line - no extra sapces or blank lines - and that the `---` at the bottom is not missed.)

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

  cover:  ./assets/images/...
  permalink: /...

  layout: book
  ---
  ```

* Fill in the details for the book - if something does not apply for a particular book then just leave that bit blank.
  - `title` This is the title of the book, e.g. 'My Amazing Book'
  - `author` This is the author's name, e.g. 'John Smith'
  - `translation` Short sentence about translation, e.g. 'Translated from Welsh by Albert Banks"
  - `isbn_physical` The ISBN for the physical printed book, e.g. '123456789'
  - `isbn_ebook` The ISBN for the eBook, e.g. '123456789'
  - `region` Must be one of `europe`, `africa`, `asia` or `latam`.  If this is not set, or is not one of the 4 options it will not appear in the book list.
  - `amazon` Link to the eBook on amazon (include the http:// etc)
  - `goodreads`Link to the good reads review page (include the http:/// etc)
  - `cover` Link to the image file to use for the book - this should be `/assets/images/` and then the hypenated-name with the image extension, e.g. `/assets/images/my-amazing-book.jpg`
  - `permalink` This should be the hyphenated-name e.g. `my-amazing-book`
* Upload the cover image into the `assets/images` folder - make sure its name matches the hyphenated-name used for the book elsewhere, e.g. `my-amazing-book.jpg`.

## Cover Images

Top-tips for good cover images:
 
1. Aim for an image size of roughly 600 to 800 pixels on the image's longest side (typically the height).
   * It doesn't have to be an exact size - something in 600 to 800 ballpark area is fine.
   * Anything less than this and the image will look too small on the page, and may appear too blurry.
1. Save the images as a `.jpg` or a `.png`.
1. Aim for a file size of at most 100kb.
   * If the images are too large then it might take a long time to load.


## Troubleshooting issues

### Book is not appearing on the site

1. Make sure that the file added for the book is in the `_books` directory.  It *must* be in the `_books` directory and cannot be anywhere else.
1. Make sure that the file added for the book ends in `.md`.
1. Make sure that the very first thing in the file for the book is `---` on its own line.  There *cannot* be any spaces or blank lines before the `---`.
1. Make sure that there is another `---` at the end of the metadata section on its own line. There cannot be any spaces before or after it.
1. Make sure that there are no spaces before any of the metadata items - e.g. `title`, `author` etc.  Each one must be on its own line without any spaces before it.
1. Make sure that `region` has a value of either `europe`, `africa`, `asia` or `latam`.

### The book has no image

1. Make sure the cover image exists in the `assets/images` directory.
1. Make sure the cover image file name matches the one in the metadata section of the book's `.md` file.
