# Contributing

Thank you for considering to contribute to the Black MIDI Guides! These guides are open for anyone to contribute to in any way possible. All improvements are welcome, from typos to full guides.

This markdown file is made to help you make your contributions optimally.

**You will need a Github account to contribute.**

## TOC

- [Contributing](#contributing)
  - [TOC](#toc)
  - [How to contribute](#how-to-contribute)
  - [Setup](#setup)
  - [First steps](#first-steps)
  - [Starting a local preview](#starting-a-local-preview)
  - [File structure](#file-structure)
  - [Editing the guides](#editing-the-guides)
  - [Editing style](#editing-style)
    - [Main Page](#main-page)
    - [Getting Started page](#getting-started-page)
    - [Other Pages](#other-pages)

## How to contribute

We appreciate all contributions. Contributions typically mean updates to the source code of a repository, but we also count other forms of contributing such as publishing issues. After all, without the issues being pointed out, how will we know what to improve on?

This is why contributing to the Black MIDI Guides can be in many shapes and sizes. We welcome the smallest contributions as much as the biggest contributions. All improvements are welcome, from typos to full guides.

That being said, some of the different ways to contribute are:

-   **[Submitting an issue](https://github.com/OvertureMIDI/Black-MIDI-Guides/issues/new/choose)** for bug reports, new ideas, or new improvements
-   **Editing existing guides** to further improve something or to fix some error
-   **Making new guides** to help users with other things

The rest of this document focuses on the last 2, but submitting an issue is just as good as the other options! Remember, we welcome everyone to contribute!

## Setup

Before you get started, we will assume you will be editing the guides locally on your PC. This means you will download all the files, edit them, then upload your changes.

If you will be editing the guides locally, you will need [Git](https://git-scm.com/downloads) to clone the files from Github to your PC, and then upload your changes later.

Overture also uses [Visual Studio Code](https://code.visualstudio.com/) to edit these files as it provides some helpful extensions and tools. You are free to use any editor you wish to use as all files are simple markdown files.

You will also need [Python3](https://www.python.org/downloads/) to build and preview the guides using mkdocs.

## First steps

Start by [creating a fork of the repository](https://github.com/OvertureMIDI/Guides/fork). This is where you will make your changes and then submit them via a pull request later.

> See [Github Docs > Forking a Repository](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo#forking-a-repository) to see more information on how to fork a repository.

After you made a fork, proceed by cloning your fork to any location on your PC.

> See [Github Docs > Cloning a Repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository#cloning-a-repository) to see how to clone your repository

You now should have all of the up-to-date files from the guides locally on your PC. You are now ready to edit the guides!

## Starting a local preview

**For this example, `~/Documents/Coding/Guides` will be the location where we cloned the Black MIDI Guides to. Anytime you see "root" below will refer to the location you cloned your fork to.**

The Black MIDI Guides uses [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/). This means you will need to install the python requirements on your PC. You can do so by running the following command in a terminal at the root of the files.

```bash
$ # This is at the root of the repository
$ pip install -r docs/requirements.txt
```

This will install all of the dependencies you will need to build and preview the mkdocs site.

After you have installed all the dependencies, you can now run the following command to start a preview of the guides locally on your machine. After running the command, you should also see the output shown similar to below.

```bash
$ # This is at the root of the repository
$ mkdocs serve # Run a preview of the site locally
INFO    -  Building documentation...
INFO    -  Cleaning site directory
[...]
INFO    -  [15:40:52] Watching paths for changes: 'docs', 'mkdocs.yml'
# If you see this line here it means your preview is now available locally!
INFO    -  [15:40:52] Serving on http://127.0.0.1:8000/
```

After you have started mkdocs locally, you can now navigate to the link provided to you to see the Black MIDI Guides being hosted locally on your PC! In this case, we will navigate to `http://127.0.0.1:8000/` in a web browser.

## File structure

The guides follows the following directory structure.

```txt
docs/
├─ assets/
│  ├─ logo.svg
├─ [Section]/
│  ├─ images/
│  │  ├─ [Images].png,jpg,gif
│  ├─ [Categories]/
│  │  ├─ .pages
│  │  ├─ [pages].md
│  ├─ .pages
│  ├─ index.md
│  ├─ [pages].md
├─ .pages
├─ CNAME
├─ index.md
├─ requirements.txt
```

For more in-depth information on what goes where, visit the [File Structure](../repo/File-Structure.md) guide.

## Editing the guides

All the pages are simple markdown files. If you don't know how to use markdown, it's very simple to learn. Here are some resources to help you get started:

-   https://www.markdowntutorial.com/ - Interactive tutorial
-   https://www.markdownguide.org/cheat-sheet/ - A cheat sheat to see the cool things you can do with markdown
-   https://www.markdownguide.org/basic-syntax/

Because of the fact we use Material for MkDocs, we also can use more advanced things like tabs, info boxes, and more cool things! For a complete list of all the features you have at your disposal, visit the [Reference page on the Material for MkDocs website](https://squidfunk.github.io/mkdocs-material/reference/).

Although, here are some things that we have used in the Black MIDI Guides.

-   [Admonitions](https://squidfunk.github.io/mkdocs-material/reference/admonitions/#usage) (Info, Warn, Error boxes + dropdowns)
-   [Content tabs](https://squidfunk.github.io/mkdocs-material/reference/content-tabs/#usage)
-   [Tables](https://squidfunk.github.io/mkdocs-material/reference/data-tables/#usage)
-   [Emojis + Icons](https://squidfunk.github.io/mkdocs-material/reference/icons-emojis/#usage)

Using markdown and the tools provided by Material for MkDocs, you can effortlessly create and edit pages on the Black MIDI Guides.

## Editing style

In the Black MIDI Guides, we try to make the pages a similar style to keep things consistent. While these aren't **required** to follow, we ask you to try to stick to it as much of you can.

> If there is something you don't how to apply the style, you can still submit it and we will try our best to fix it up in the cleanup branch.

### Main Page

For the main page (index.md), you can use our template below!

```md
# TOPIC

Here are some TOPIC guides to help you get started.

??? info "What is TOPIC?"

    > General information about the TOPIC here

## Different TOPIC Versions

> If your topic has multiple versions, like if your topic is a software, you can address them here and address which would you will talk about!

## Common Links

Here are some of the common things people ask for when dealing with TOPIC.

-   [Getting Started](getting-started.md)
-   > More links here
```

### Getting Started page

For the Getting Started page (getting-started.md), you can use our template below!

```md
# Getting Started

This guide will help you get started with TOPIC.

## Prerequisites

> Here you can talk about anything you must do before you approach this topic. For example, softwares can require frameworks to install first, so you can address those here.

## Setup / Installation

> This is the main portion of the Getting Started guide! Here you will show how to setup whatever it is you're talking about. Please add picture too!

> You are also free to create more headings and sections to your heart's content

## Next Steps

Here are some links to helpful things to do next!

-   > Links to other pages
```

### Other Pages

Besides the two main pages, there isn't really a template to follow. You are free to freestyle the rest of the pages you may need. Although here are some pointers to follow:

-   **Link to external resources.** You should link to outside resources if there is a simplication of things, for those who want to learn more
-   **Put requirements near the top.** If your guide requires the user to have followed another guide, be sure to address it clearly with a [warn admonition](https://squidfunk.github.io/mkdocs-material/reference/admonitions/#usage)
-   **Use images as much as you can!** To a reasonable extent, try to add images for better guiding.
    -   **Add images to help users find what you're talking about.** Try to include images when you say something along the lines of "Click on edit, then select all," or, "Click the Google Drive download option".
    -   **Multi-language images.** If your program has around 2 popular languages try to also include images for the 2 languages to help everyone out! If there are too many languages then we understand
        -   **Use [tabs](https://squidfunk.github.io/mkdocs-material/reference/content-tabs/#usage) to separate them!** Like the Domino guides, you can use tabs to organize the different language images and not take that much space.
-   **Try to address any potential problems.** If there are some issues that can occur, a simple [admonition](https://squidfunk.github.io/mkdocs-material/reference/admonitions/#usage) will suffice. If there are a LOT of issues that can occur, make an FAQ page, or link to an existing page (can be external).

Again, these aren't _required_ to be followed, but we ask that you try your best to adhere to them as much as you can.
