# cx Design Manual

This is a GitHub pages repository for the [**cx Design Manual**](http://cxdesignmanual.com).

This project was ideated, designed, and developed by [Chris Berridge](http://www.cxpartners.co.uk/who-we-are/chris-berridge/), [Luke Jones](http://www.cxpartners.co.uk/who-we-are/luke-jones/), [Michelle O’Loughlin](http://www.cxpartners.co.uk/who-we-are/michelle-oloughlin/), and [Yunmie Kim](http://www.cxpartners.co.uk/who-we-are/yunmie-kim/) during the first cx Visual Design Summit in August 2014.

If you wish to make an update to the assets, content, or design of this project, please contact a member of the design department.

This site was designed and built to suit the environments which cxpartners employees work in. That means it is not responsive or fluid, and has only been browser-tested in Safari, Chrome, and Firefox. We discussed the use case and decided that this manual will most likely be read in a production environment where assets can be used and downloaded. Not on a tablet or mobile phone.

## Modifying / updating the design manual

The Design Manual is powered using Jekyll and GitHub Pages. Every time a change is pushed to Git, it is updated online without the requirement for manual upload via FTP, and provides a repository that is accessible and editable by anyone who needs to make changes.

The initial setup is quick, so editing can begin in a matter of minutes.

###How to use

The Design Manual lives in a Git repository so is editable by anyone who has access. Anyone with an intermediate level of knowledge in these areas can make changes to the Design Manual. The following technologies are used:

* [Git](https://help.github.com) – A version control system
* [GitHub Pages](https://pages.github.com) – Quick site publishing and free hosting provided by GitHub. Everything that is committed to the Master branch of the Git repository will be pushed to the live site.
* [Jekyll](https://jekyllrb.com) – An easy-to-use, database free static website generator that runs on your system. GitHub pages works with Jekyll by default, so everything is published automatically.
* HTML
* [LESS](http://lesscss.org/) – A CSS pre-processor, allowing users to create variables (e.g. @blue), nest CSS, and many other things in a very fast manner.

Use [Atom by GitHub](https://atom.io) with the LESS extension installed to automatically compile the LESS documents.

###Getting started

1. Either download Xcode and use Git via command-line, or [download GitHub for Mac](https://desktop.github.com)
1. Open terminal and follow [Jekyll Installation Instructions](http://jekyllrb.com/docs/installation/) on the website
1. Clone the Design Manual Git repository

###Making changes

Once you have the repository on your system, you can run Jekyll by opening up Terminal, and typing in `cd` followed by a space, dragging the repository folder from Finder into the Terminal window, and pressing enter.

> When you drag your folder into Terminal, it will change into something like this:
>
> `cd /Users/Your\ Name/Dropbox/design-manual.github.io`
>
> This command 'changes directory' to the folder you have dragged in – simples.

Once you are in the correct folder, type in `jekyll serve`, this will provide you with a URL to visit in your browser (e.g. `127.0.0.1:4000`) and automatically generate a static site every time you update a file.

###What to edit

* LESS: All changes should be made to `_main.less` and `_lib.less`. `_main.less` contains all regular style information, and `_lib.less` contains all of the LESS variables such as colours, font families, and styles. `style.css` is an automatically generated file, so will be overwritten every time a .less file is saved.
* Pages: The main pages are just basic HTML files (e.g. `typography.html`, `index.html`, and `colour.html`). They can be edited as any standard HTML page.
* `<head>`: This can be found in `_includes/head.html`.
* Main header: This can be found in `_includes/masthead.html`
* Images: Add images and assets to the `img` folder in each corresponding directory. Make sure these are retina (@2x) PNGs that have been compressed using software such as ImageOptim.

###What to avoid

* **Do not make modifications to the `_site` folder**. This folder is automatically generated by Jekyll and GitHub pages. Editing these files _will_ cause data loss everywhere.
* `_layouts` is used for primary layouts of the site, modifying this could break the site.

###Need further help?

A member of the development team will be able to assist your efforts. Whilst this may seem overwhelming, it is an efficient way of creating a design manual that anyone can edit.
