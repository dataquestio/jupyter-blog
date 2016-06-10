jupyter-blog
---------------------

This is an example repo that shows a minimal configuration that allows you to create a personal blog using Jupyter notebooks.  

See [this](https://www.dataquest.io/blog/how-to-setup-a-data-science-blog/) blog post for more details, and a guide on how to setup and deploy a blog.

Reproducing this example
---------------------

You can reproduce this setup on your own computer by following the steps below:

* Create a virtualenv.
* Install everything in `requirements.txt`.
* Setup your `.gitignore` file.
* Run `pelican-quickstart`.
* Create a `plugins` folder.
* Run `git init`.
* Run `git submodule add git://github.com/danielfrg/pelican-ipynb.git plugins/ipynb`.
* Create any notebooks you want in the `content` folder.
    * Remember to create corresponding `.ipynb-meta` files.
* Edit pelicanconf.py to the lines that activate the `pelican-ipynb` plugin.
* Run `pelican content`.
* Switch to the `output` directory and run `python -m pelican.server`.