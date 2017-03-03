If you are a content creator follow these simple steps in order to maintain and update the FDS website.

- [Page structure](#page-structure)
- [Page header](#page-header)
- [Page contents](#page-contents)
- [Custom page components](#custom-page-components)
- [Content linting](#content-linting)

## Page structure

Pages are stored under `/contents`. You can create new pages directly inside this folder. If you do so, remember to also add your page in `/contents/index.json` otherwise it will not be displayed in the sidebar, more information [here](#). The following is a basic page structure:

```html
<header>
  ...
</header>
<section>
  ...
</section>
```

## Page header

Every page features a `<header>`. It includes the title of the page, a brief description (not mandatory) and the table of contents. The table of contents reflects the section titles of the page (only level two headings). The structure is like the following:

```html
<header>
  <h1 id="page-title">Page title</h1>
  <p>Page description</p>
  <ul>
    <li>
      <a href="#section-title-a">Section title A</a>
    </li>
    <li>
      <a href="#section-title-b">Section title B</a>
    </li>
  </ul>
</header>
```

Remember to add the `href` attribute to the links in the table of contents. A good practice is to simply translate the title to lowercase and replace spaces with hyphens. This `href` has to be the same as the `id` specified in the headings below.

## Page contents

### Sections

Right after the header you can add your content. Every page section should be wrapped in a `<section>` tag. Inside the section you can use the plain `html` to write down your contents.

```html
<section>
  <h2 id="#section-title-a">Section title A</h2>
  <p>...</p>
  <h3 id="#section-subtitle-a">Section subtitle A</h3>
  <p>...</p>
</section>
<section>
  <h2 id="section-title-b">Section title B</h2>
  <p>...</p>
</section>
```

### Headings

Inside your sections follow the headings hierarchy as shown in the example above. You can use `h2`, `h3` and `h4`. Remember that every heading should have an `id` attribute that is equal to the `href` specified in the table of contend in the header.

### Images

When you need to insert an image use the `<figure>` tag. If necessary you can also add a caption with `<figcaption>`.

```html
<section>
  <h2 id="section-title">Section title</h2>
  <p>...</p>
  <figure>
    <img src="images/page-title/image.jpg" alt="Image description">
    <figcaption>Image caption</figcaption>
  </figure>
</section>
```

Images are stored under `/images`. We organize images per pages. So every page has a folder where its images are saved. If you create a new page please also create a corrisponding folder in this directory.

### Links

As for all other contens links do not need any CSS class. Simply add an `a` element with a `href` attribute.

```html
<p>
  Some text with a <a href="https://name.domain">link</a>.
</p>
```

## Custom page components

Sometimes you need components that are more complex than bodies of text or images. You can create them under the `/shared` folder. These components are built with HTML and CSS and can include CSS classes. Make sure to check the CSS guidelines under the [How it works](#) page.

## Content linting

If you happen to see your text set in Comic Sans it means that you missed somthing. It could be a an `id` in your heading or a `<section>` around your contents.

