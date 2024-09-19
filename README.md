# Docs Landing Page
In support of the diverse range of tools in the Wild Me suite, we want to provide in-depth documentation that covers usage in the interface, development against the product, interacting with the machine learning, and information on how to contribute. To do this, we need to have separate docs for each product, and a landing page to connect all of these different docs sections. This is that central landing page!

## Contributing content
For the base page, you can make changes to `config.toml` and the pages under `/content/services/`. For the product todo lists, edit the pages under `/content/post/`. To adjust the about page, edit `/content/about.md`.

## Adjusting themes and styles
You can make changes to anything under `/assets/`. Add any new images to `/public/images` and use descriptive naming. Do not make changes to the theme styles as they get rebuilt on each deploy.

## Dev
This page was made with [hugo](https://gohugo.io/), and a modified version of the theme [Initio](https://themes.gohugo.io/themes/hugo-initio/).

### Pre-reqs
- Install Hugo (https://gohugo.io/installation/)
- fork and clone this repo

### Making Changes
To edit text, you will want to adjust the contents of `hugo.toml`. To change the page structure, you will make changes to the pages in the `layouts` folder. To change styles or javascript, edit the files in `public`; changes to the same files in `themes` will be reverted on build.

### Testing locally
1. In your terminal, `cd` to the top level of this repository (where the `hugo.toml` file is located).
1. Use the command `hugo server` to start a local server
1. In your browser, check your changes at `http://localhost:1313`
1. Refresh the browser after each change.
1. When happy with your changes, build with `hugo` and commit.

If your changes are not displaying, you may need to stop the hugo server (`Ctrl+C`) and restart it for the system to cleanly rebuild.
