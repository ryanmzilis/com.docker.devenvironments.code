If you are a content creator follow these simple steps in order to maintain and update the Photon Design System website.

- [Page structure](#page-structure)
- [Page header](#page-header)
- [Page contents](#page-contents)
- [Custom page components](#custom-page-components-coming-soon)

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

Every page features a `<header>`. It includes the title of the page and a brief description (not mandatory but advised). The structure is like the following:

```html
<header>
  <h1>Page title</h1>
  <p>Page description</p>
</header>
```

## Page contents

### Sections

Right after the header you can add your content. Every page section should be wrapped in a `<section>` tag. Inside the section you can use the plain `html` to write down your contents.

```html
<section>
  <h2>Section title A</h2>
  <p>...</p>
  <h3>Section subtitle A</h3>
  <p>...</p>
</section>
<section>
  <h2>Section title B</h2>
  <p>...</p>
</section>
```

### Headings

Inside your sections follow the headings hierarchy as shown in the example above. You can use `h2`, `h3` and `h4`. A section always starts with an `h2`. 

### Images

When you need to add an image use the `<figure>` tag. If necessary you can also add a caption with `<figcaption>`.

```html
<section>
  <h2>Section title</h2>
  <p>...</p>
  <figure>
    <img src="images/page-title/image.jpg" alt="Image description">
    <figcaption>Image caption</figcaption>
  </figure>
</section>
```

Images are stored under `/images`. We organize images per pages. So every page has a folder where its images are saved. If you create a new page please also create a corresponding folder in this directory.

### Links

As for all other contents links do not need any CSS class. Simply add an `a` element with a `href` attribute.

```html
<p>
  Some text with a <a href="https://name.domain">link</a>.
</p>
```

### Related

If you want to point to links or resources related to what you are writing about you can add a module with the `blockquote` tag.

```html
<blockquote>
  <h4>Related title</h4>
  <ul>
    <li>
      <a href="#!">Related link</a>
    </li>
    <li>
      <a href="#!">Related resource</a>
    </li>
  </ul>
</blockquote>
```

## Custom page components

Sometimes you may need components that are more complex than bodies of text or images. You can create them under the `/includes` folder. These components are built with HTML and CSS and can include CSS classes. Make sure to check the CSS guidelines under [Developing](https://github.com/firefoxux/photon/wiki/Developing#css) page.

