# File Structure

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

View below to see what each folder does and contains.

## TOC

- [File Structure](#file-structure)
  - [TOC](#toc)
  - [docs](#docs)
  - [docs \> assets](#docs--assets)
  - [docs \> Section](#docs--section)
  - [docs \> Section \> images](#docs--section--images)
  - [docs \> Section \> Categories](#docs--section--categories)
  - [docs \> CNAME](#docs--cname)
  - [docs \> requirements.txt](#docs--requirementstxt)
  - [docs \> ... \> index.md](#docs----indexmd)
  - [docs \> ... \> .pages](#docs----pages)
  - [docs \> ... \> Pages.md](#docs----pagesmd)

## docs

This is the main folder that mkdocs reads and prepares for the website. Anything outside of this folder will NOT be included in the website.

## docs > assets

This is assets which are for the website **as a whole**. For example, we have the Overture logo in here to display on the website, and on the favicon (browser tab).

## docs > Section

This is where the guides are located for a specific section. The section can be titled anything. For example, `docs > Domino` will hold all the guides pertaining to Domino. If you'd like to create new guides for something that doesn't have a section yet, make a new folder:

```txt
docs/
├─ MySection/
│  ├─ guide files go here...
```

## docs > Section > images

This is where images are stored for their respective [sections](#docs--section). Images should be named using lowercase_snake_case.

Good Example:

-   this_is_a_good_name.png

Bad Examples:

-   thisIsNot.png
-   OrThis.png
-   neither-is-this.png
-   OR_THIS.png
-   and no spaces thanks.png

You can also add subfolders here if you feel like it should be a bit more organized.

## docs > Section > Categories

Categories are like subsections of sections. They are just to group similar guides together and help with organization. A good example of this is the OmniMIDI guide which is looks like the following

```txt
docs/
├─ OmniMIDI/
│  ├─ Soundfonts/
│  │  ├─ configuration.md
│  │  ├─ recommendations.md
```

Here we just grouped the configuration of soundfonts and recommended soundfonts into one.

## docs > CNAME

This should not be edited as it tells Github Pages (what we use to host the Black MIDI Guides) what domain the website should be on. You can temporarily edit this file if you'd like to preview your changes online ([we recommend using the local method instead](Contributing.md#starting-a-local-preview)), although please edit it back to `guides.blackmidi.wiki` after you're ready to submit your changes.

## docs > requirements.txt

These are the python3 pip dependencies needed to build the website.

## docs > ... > index.md

Anywhere you see index.md, that is going to be the main entry point for that URL. For example, `docs > index.md` is the page used for https://guides.blackmidi.wiki/, and `docs > Domino > index.md` is the page used for https://guides.blackmidi.wiki/Domino/.

## docs > ... > .pages

This is what tells [mkdocs-awesome-pages-plugin](https://github.com/lukasgeiter/mkdocs-awesome-pages-plugin) how to structure the pages in the website.

For example, lets take a look at the `docs > .pages` file:

```yaml
nav:
    - Home: index.md
    - Domino
    - Piano From Above: PFA
    - OmniMIDI
```

All .pages must start with the `nav:` element, and the list will contain the pages shown, and how they are presented

For more information on how to use this, [visit here](https://github.com/lukasgeiter/mkdocs-awesome-pages-plugin#features)

## docs > ... > Pages.md

This is simply a placeholder for any pages you create. Feel free to create as many as you'd like
