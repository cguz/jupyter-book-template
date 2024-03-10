# Jupyter Book template


Building a Jupyter Book broadly consists of these steps:

- Create your book’s content. You structure your book with a collection of folders, files, and configuration. [Anatomy of a Jupyter Book](https://jupyterbook.org/en/stable/start/create.html#anatomy-of-a-book).

- Build your book. Using Jupyter Book’s command-line interface you can convert your pages into either an HTML or a PDF book. [Build your book](https://jupyterbook.org/en/stable/start/build.html).

- Publish your book online. Once your book is built, you can share it with others. Most common is to build HTML, and host it as a public website. [Publish your book online](https://jupyterbook.org/en/stable/start/publish.html).


## Installation

Create a virtual environment:

    $ python3.10 -m venv .env
    $ source .env/bin/active

Install jupyter book

    $ pip install -U jupyter-book

## Create your book's content

    $ jupyter-book create book-template

## Build your book

It will create a set of static websites.

    $ jupyter-book build book-template

To rebuild:

    $ jupyter-book build --all book-template

## Publish you book online

- Create a github repository without a README.md
- In the same folder of our book-template, execute the following:

    $ git init
    $ git add README.md book-template
    $ git commit -m "First jupyter book template"
    $ git branch -M main
    $ git remote add origin https://github.com/cguz/jupyter-book-template.git
    $ git push -u origin main

- Install ghp-impot:

    $ pip install ghp-import

- Create the branch gh-pages with the content of the _build/html/

    $ ghp-import -n -p -f book-template/_build/html

- The website should be visible in :

    https://cguz.github.io/jupyter-book-template/intro.html

- If not, Go to: 

    Options -> GitHub Pages to ensure that the gh-pages branch is configured

# References

- [Jupyter Book](https://jupyterbook.org/en/stable/start/create.html)