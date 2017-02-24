If you are a content creator follow this simple steps in order to maintain and update the FSD website. 

Pages are stored under `/contents`. You can create new pages directly inside this folder. If you do so, remember to also add your page in `/contents/index.json` otherwise it will not be displayed in the sidebar, more information [here](#). The following is a basic page structure:

```html
<header>
  ...
</header>
<section>
  ...
</section>
<section>
  ...
</section>
<section>
  ...
</section>
<footer>
  ...
</footer>
```con

Every page features a `<header>`. It includes the title of the page, a brief description (not mandatory) and the table of contents. The table of contents reflects the section titles of the page. The structure is like the following:

```html
<header>
  <h1>Page title</h1>
  <p>
    Page description
  </p>
  <ul>
    <li>
      <a href="#section-title">Section title</a>
    </li>
    <li>
      <a href="#section-title">Section title</a>
    </li>
    <li>
      <a href="#section-title">Section title</a>
    </li>
  </ul>
</header>
```

Remember to add the `href` attribute to the links in the table of contents. A good practice is to simply translate the title to lowercase and replace spaces with hyphens.

Right after the header you can add your content. Every page section should be wrapped in a `<section>` tag. Inside the section you can use the plain `html` to write down your contents.