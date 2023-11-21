# Talk at IAG Science Day 2023

This is a 4-minute talk aimed at a general audience about
some of the current research in the [CompGeoLab](https://www.compgeolab.org/).
It's for the [2023 IAG Science Day](https://www.iag.usp.br/eventos/science-day-2023)
and will be streamed on YouTube.

Slides: https://www.leouieda.com/iag-science-day-2023 | [download a PDF version](https://github.com/leouieda/iag-science-day-2023/releases/download/submitted/IAG.Science.Day.2023.-.Leonardo.Uieda.pdf)

## Template

These slides were made from the template: https://github.com/leouieda/talk-template

## What's included

`index.html`: This is the master document that sets up reveal.js and
its plugins and loads the slide content from `slides.md`.
**Change the HTML `<title>` tag here**.

`slides.md`: Markdown file with the actual slide content. The template
includes some slides that demo the custom CSS classes available.
**Add your content here.**

`css/style.less`: Custom styling and CSS classes (using
[Less](http://lesscss.org/)). Edit to tweak colours, sizes, fonts,
spacing, etc.

`assets`: Images used in the presentation. You can probably delete all
of these when making your slides. Replace the `favicon.png` with a
32 x 32 px image to customize the icon (this is set in `index.html`).

`fonts`: Sources for the fonts used:
[FontAwesome](https://fontawesome.com/),
[Atkinson Hyperlegible](https://brailleinstitute.org/freefont),
[Ubuntu Mono](https://design.ubuntu.com/font/).
Included in the repository for offline access. You could remove them and
include fonts from a CDN (like Google Fonts) in `index.html`.

`packages`: "Vendored" versions of reveal.js, Less, and
[KaTeX](https://katex.org/) (for maths) that are used.
Having them in the repository is important for using the slides offline
(on a plane or lecture room without easy internet access).

`serve.py`: Python script that serves the slides and reloads them
whenever the source files change. Very handy for development.
See below for instructions.

## Serving the slides locally

Unfortunately, you can't just open the `index.html` file on browser
to view your slides.
Reveal.js requires an actual local server.
You can set one up however you'd like.
Below, I provide instructions for doing so in Python (which is what
I use most of the time) but it would work with any other local
server.

First, install the [livereload](https://github.com/lepture/python-livereload)
Python package:

```
pip install livereload
```

or

```
conda install livereload -c conda-forge
```

Then, start a server at http://localhost:8008 by running:

```
python serve.py
```

The slides will open on your default browser and will automatically reload
when you update any of the files in the repository.

## License

The template (`slides.md`, `index.html`, and `css/style.less`) is licensed under a
<a href="https://creativecommons.org/licenses/by/4.0/">Creative Commons
Attribution 4.0 International License</a>.
