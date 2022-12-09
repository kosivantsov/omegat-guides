# OmegaT user guides [cApStAn]

Welcome to the **OmegaT user guides** repository, maintained by the [cApStAn](http://www.capstan.be) Tech Team.

This repository contains different OmegaT user guides authored as Markdown files with a modular approach, meant to be built as a static website with MkDocs.

## Commands

To start the live-reloading docs server:

```
mkdocs serve
``` 

To build the static documentation site:

```
mkdocs build
``` 

To print help message and exit:

```
mkdocs -h
``` 

To commit changes to this Github repository:

```
git add .
git commit -m "A description of the changes"
git push
``` 

To deploy the static website to [GitHub Pages](https://capstanlqc.github.io/omegat-guides/):

```
mkdocs gh-deploy
``` 


## Block inclusion for modularity

Some sections are common for all or several, whereas some other sections are guide-specific. Only one copy of common sections exist, and that is included as needed when composing the different guides using Django template syntax (e.g. `{% include 'foo.md' %}`).

Alternative appraoch using Jekyll: https://jekyllrb.com/docs/includes/

## Goals

Create documentation that is:

+ Easy to maintain with version control
+ Flexible and minimalistic editing
+ Compatible with many output formats
+ Reusable and platform-independent
+ Clean display
+ Compatible with custom domains and with embedding

Also, issues that we try to solve or avoid: 

- copy-pasting
- anyone can edit our guide in PISA Connect's documentation dashboard
- there's no backup in PISA Connect
- PISA Connect only offers editing in a WYSIWYG mode or in plain HTML code

## Steps

1. Exported all Dokuwiki pages as Markdown with the [DokuWiki to Markdown Plugin](https://www.dokuwiki.org/plugin:dw2markdown)
2. Tweaked formatting and paths to included files and images
3. Organized content as guides for different roles, based on the previous guides

## Todo / ways to help

+ Update images
+ Look for @todo in the files and find things to do
+ Test other building tools such as Pandoc, Sphinx, Jekyll, etc. and other hosting sites such as [BookStack](https://www.bookstackapp.com/), [GitBook](Gitbook) or [RTfD])
Hosting site: readthedocs.org)
+ Test other themes
+ Test other authoring formats like reStructuredText, AsciiDoc, Wiki etc.
+ Consider a custom URL in a cApStAn domain, info [here](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)


## Embedding

```html
<embed src="https://capstanlqc.github.io/ttt_docs/omegat/index.html" scrolling="no" frameborder="0" width="100%" height="600">
``` 

## Tips for writing guides

+ Use the Markdown [Tables Generator](https://www.tablesgenerator.com/markdown_tables) to create or edit markdown tables easily.

+ Keep it short (instructions don't need to be long or verbose to be clear)

+ Do's and dont's

| Don't | Do  | Comment |
|-------|-----|---------|
| **Project>Open Recent Project**    | **Project** > **Open Recent Project** | Separate both items in the path with " > ". Bold each separately     |


