## Installation

Install Node. If you use homebrew, do:

```bash
$ brew install node
```

Otherwise, you can download it from [nodejs.org](http://nodejs.org/download/). Then clone the repository and path to the folder.

```bash
$ git clone git@github.com:bwinton/StyleGuide.git
$ cd path/to/StyleGuide
```

Finally install all node dependecies:

```bash
$ npm install
```

## `npm` commands

To run (with hot-reloading!):

```bash
$ npm run serve
```

To build:

```bash
$ npm run build
```

## Table of contents

The global table of contents is automatically generated based on what is listed under `contents/index.json`. When you create a new page under `/contents` make sure to add such page also in this json file. If the page is a first level page use the following code. The file name should be the same as the one specified under `/contents`.

```json
{
  "title": "Page Title",
  "file": "page-title.html"
}
```

If the page is a second level page use the following code instead. Add as  many pages as you add under `/contents`.

```json
{
  "title": "Chapter Title",
  "pages": [
    {
      "title": "Page Title",
      "file": "page-title.html"
    },
    {
      "title": "Page Title Two",
      "file": "page-title-two.html"
    }
  ]
}
```

## CSS

When we write CSS we follow two approaches. Global styles are handled with [Tachyons CSS](http://tachyons.io/). We use this framework for the website layout and for the table of contents.

For everything which is related to a content page, so `.html` files living under `/contents`, we scope styles in SCSS. You can find these styles under `/src/styles/page.scss`. This approach enables editors and content creator to write plain HTML withouth worring about classes, id and CSS in general.
