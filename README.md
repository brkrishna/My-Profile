# Project: Profile - Ramakrishna Rao Bodi

This is the GitHub repository for the project you named "My-Profile", generated from the "yaxt-blackledge-infocards" website template at [yax.com](https://yax.com).

From here, deploy your website for free hosting. Just click a button to deploy your website to [Netlify](https://www.netlify.com/), [Vercel](https://vercel.com/), or [Render.com](https://render.com/). During the process, you will create a second repo for deployment. Name it what you like; I suggest "My-Profile-deploy".

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/brkrishna/My-Profile)

[![Deploy to Vercel](https://vercel.com/button)](https://vercel.com/import/project?template=https://github.com/brkrishna/My-Profile)

[![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy)

For help, open a GitHub issue and mention [DanielKehoe](https://github.com/DanielKehoe) or email [support@yax.com](mailto:support@yax.com?subject=[GitHub]%20My-Profile).

## Stackless newsletter

It is early days for Yax. If you are curious about what we are doing, go to [stackless.community](https://stackless.community/) and sign up for the newsletter, all about Yax and building websites without frameworks or build tools.



# Blackledge Infocards

This is a website built using the [yax.com](https://yax.com/) website builder project. It was designed by the Yax team for Peter Blackledge, the first subscriber to the [Yax Tutorials](https://tutorials.yax.com/).

The website is styled with the [Basic.css](https://vladocar.github.io/Basic.css/) stylesheet by [Vladimir Carrer](http://www.vcarrer.com/). No CSS classes are needed; styles are applied using only HTML5 tags.

## Pages

The website has a home page, about page, and an unlimited number of content pages.

## Editing content

This template doesn't use an on-page editor. Instead, you can edit the files directly on GitHub. Click a filename and look for the "Edit this file" pen icon. After committing your changes (which saves the file), your website will automatically update (if you are editing files created in a repo that was previously deployed to Netlify, Vercel, or Render.com).

## Markdown files

Content for each page comes from [Markdown](https://www.markdownguide.org/) files. Markdown is well-suited for content and easier to edit than HTML. The name of each Markdown file matches the HTML file for each page (so the `about.html` page gets content from an `about.md` file). The home page gets content from two Markdown files, `index-intro.md` and `index-closing.md` for intro and closing sections.

## Home page

The home page contains a title which is read from a file named `manifest.json`. The home page also displays an unlimited number of "information cards" each containing a title, summary, and link to a content page. The content for the cards is read from the `manifest.json` file.

## Manifest file

Edit the `manifest.json` file to change the home page title or the information cards.

## Adding content pages

Add or remove pages from the `manifest.json` list to add or remove cards on the home page. Files for the content pages are in the `content` folder. It contains nine pairs of `.html` and `.md` files. Duplicate an `.html` and `.md` file if you need another content page (be sure to add it to the list in the `manifest.json` file).

## About page

Edit the `about.md` file to change the about page.

## Navigation bar

Each page has a navbar with links to the home page and about page. The navbar is generated by a custom tag, <yax-blackledge-navbar>, created in JavaScript. You can edit the file `assets/scripts/yax-blackledge-navbar.js` to add or change links.

## Custom elements

The website uses five HTML custom elements:
- `<yax-blackledge-cards>`: reads `manifest.json` and displays cards
- `<yax-blackledge-navbar>`: navigation
- `<yax-blackledge-title>`: reads `manifest.json` and displays a title
- `<yax-markdown>`: reads Markdown files to display content
- `<yax-blackledge-heading>`: displays title/summary on content pages from `manifest.json` 

## Cards per row

On the home page, you can change the number of cards displayed per row by editing the `index.html` file. For example, change `<yax-blackledge-cards cards_per_row="3">` to `<yax-blackledge-cards cards_per_row="4">`.
