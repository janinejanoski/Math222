# PreTeXt Slideshow Template

Use this template repository to quickly start a new [PreTeXt](https://pretextbook.org) project for a slideshow entirely in the cloud, using GitHub Codespaces.  

## Structure

If you are building a slideshow for an entire course, you may find it useful to use a `section` for each day of class to make it easy to navigate. 

## Annotated vs blank

Use `component="a"` as an attribute on anything that you want in the instructor version of the slides but do not want to appear in the "blank" slides you will write on during class. Sometimes, it is cleanest to have two versions of something (or you need a placeholder in the blank slides), so you can put `component="b"` on whatever should appear in the blank slides.

## Building

There are two build targets: `slides` and `slides-annotated`. 

## Viewing

View whichever target you have built using the usual view process. Note that because this is HTML output, what you see may suggest that information is visible that gets cut off once you are connected to a projector or if you export to PDF to annotated on a tablet.

Press the ESC key on your keyboard when viewing the slideshow as HTML to see a zoomed out view that makes it easy to advance to another section.

## Converting to PDF

Instructions yet to come. PreTeXt is using an old version of Reveal.js, and its print to PDF feature is not great. We're going to try upgrading to a newer version of Reveal.js, which hopefully will make that better. If not, there's a utility called `decktape` that we are trying to get set up to work in a PreTeXt Codespace or Docker container.