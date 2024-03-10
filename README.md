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
- 


# References

- [Jupyter Book](https://jupyterbook.org/en/stable/start/create.html)