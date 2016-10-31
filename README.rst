==================
Remark.js snippets
==================

Copyright (c) 2016 Jérémie DECOCK (www.jdhp.org)

* Read online: http://www.jdhp.org/docs/remarkjs_snippets/remarkjs_snippets.html
* PDF version: http://www.jdhp.org/dl/pdf/remarkjs_snippets.pdf
* Source code: https://github.com/jdhp-docs/remarkjs-snippets

About Remark.js
===============

Official web sites:

* http://remarkjs.com
* https://github.com/gnab/remark
* https://github.com/gnab/remark/wiki

Official demo: http://remarkjs.com/#1

The Markdown source code of these slides are embeded in the HTML document of
the demo (i.e. go to http://remarkjs.com/#1 and type Ctrl+u to read the source
code of the demo within Firefox).

Main features
-------------

Presentation mode
~~~~~~~~~~~~~~~~~

1. press 'C' to clone the (browser) window;
2. position the two windows on the two screens (presenter screen and audience
   screen) and enable the browser's fullscreen mode;
3. then press 'P' on the presenter screen to show notes.

See http://remarkjs.com/ (slide 14) for more info.

Syntax highlighting
~~~~~~~~~~~~~~~~~~~

See http://remarkjs.com/

Maths: Latex using MathJax
~~~~~~~~~~~~~~~~~~~~~~~~~~

See https://github.com/gnab/remark/wiki/LaTeX-using-MathJax

Colured Terminal Listings
~~~~~~~~~~~~~~~~~~~~~~~~~

See http://joshbode.github.io/remark/ansi.html#1

Alternatives
------------

See `this article <http://caseywatts.github.io/2012/12/12/markdown_to_slide_presentation/>`_.

HTML based
~~~~~~~~~~

* `S5`_
* `Reveal.js`_
* `Impress.js`_
* `Deck.js`_

(Modified) Markdown based
~~~~~~~~~~~~~~~~~~~~~~~~~

* `Landslide`_
* `Markdown Presenter`_
* `KeyDown`_

Usage
=====

HTML embedded
-------------

::

    <!DOCTYPE html>

    <!---
        Remark (License MIT)
        - http://remarkjs.com
        - https://github.com/gnab/remark/wiki
        - https://github.com/gnab/remark
    -->

    <html>
        <head>
            <style type="text/css">
                /* Slideshow styles */
            </style>
        </head>
        <body>
            <textarea id="source">
    class: center, middle

    # Title

    ---

    # Agenda

    1. Introduction
    2. Deep-dive
    3. ...

    ---

    # Introduction

            </textarea>

            <script src="http://remarkjs.com/downloads/remark-latest.min.js"> </script>
            <!-- Offline version : <script src="remark.js"> </script> -->

            <script>
                var slideshow = remark.create();
            </script>
        </body>
    </html>

External file
-------------

::

    <!DOCTYPE html>

    <!---
        Remark (License MIT)
        - http://remarkjs.com
        - https://github.com/gnab/remark/wiki
        - https://github.com/gnab/remark
    -->

    <html>
        <head>
            <style type="text/css">
                /* Slideshow styles */
            </style>
        </head>
        <body>
            <script src="http://remarkjs.com/downloads/remark-latest.min.js"> </script>
            <!-- Offline version : <script src="remark.js"> </script> -->

            <script>
                var slideshow = remark.create({
                    sourceUrl: 'slides.md'
                });
            </script>
        </body>
    </html>



.. _S5: http://meyerweb.com/eric/tools/s5/
.. _Reveal.js: https://github.com/hakimel/reveal.js/
.. _Impress.js: https://github.com/bartaz/impress.js/
.. _Deck.js: https://github.com/imakewebthings/deck.js
.. _Landslide: https://github.com/adamzap/landslide#notes
.. _Markdown Presenter: http://www.splinter.com.au/markdown-presentations/
.. _KeyDown: https://github.com/infews/keydown
