Introduction
------------

Thank you for taking the time to contribute to this community project aimed at promoting planetary surface sciences within the French community. To ensure a certain uniformity in the writing of this guide, please follow the following recommendations.

Format and Style
---------------

The articles in this guide are written in English using a [markdown](https://fr.wikipedia.org/wiki/Markdown) syntax (`.md`) and are grouped in the `docs/` folder. If you are not familiar with this language, you can refer to [these examples](https://jupyterbook.org/reference/cheatsheet.html) to get started easily. Markdown is the native language of GitHub for submitting changes through their web interface. Feel free to use the <kbd>preview</kbd> button to visualize your results.

If the content of your article suits it, you can write it directly in [Jupyter Notebooks](https://jupyterbook.org/file-types/notebooks.html) (`.ipynb`).

All the articles are reformatted using [Jupyter-Book](https://jupyterbook.org) and GitHub to be displayed on the [web page of the Planetary Surfaces Pole platform](https://pdssp-docs.github.io).


Submitting a Change, Proposing a Modification, or an Addition
--------------------------------------------------------------

1. Fork this repository to add it to your GitHub space by clicking [here](https://github.com/pdssp/pdssp-docs/fork).
2. You can add one (or more) articles directly from GitHub or by copying the project locally (see section below).
3. Once written, remember to add your article to the table of contents (`docs/_toc.yml`) and if it's your first contribution, please add your name and affiliation to the list in the `AUTHORS.md` file.
4. Submit a Pull Request with your additions to the project.
5. The changes will be manually reviewed by one of the members of the pole.
6. The online guide will be automatically updated with your new article :rocket:


Editing this Guide Locally
----------------------------

To edit the guide locally, start by getting a copy of the project (after forking it):

```bash
git clone https://github.com/<GH_USERNAME>/pdssp-docs
cd pdssp-docs
```

Make your edits in the docs/ folder.

If you want to preview how your article looks before submitting it, you need to install the project's dependencies:

```bash
pip install -r requirements.txt
```

Then execute the following command to build your article:

```bash
jupyter-book build docs/
```

The result is available in the _build/html/ folder and can be viewed in your web browser.

```bash
jupyter-book build docs/
```
