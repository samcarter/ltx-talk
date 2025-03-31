# `xbeamer` - A LaTeX class for producing presentations

## NOTICE

This is a *development draft*: the exact nature of what might be released,
including almost all features and the name the class, is still open.

## Description

The `xbeamer` class is focused on producing (on-screen) presentations, along
with support material such as handouts and speaker notes. Content is created in
a `frame` environment, each of which can be divided up into a number of slides
(actual output pages). A simple 'overlay' notation is used to specify which
material appears on each slide within a frame. The class supports a range of
environments to enable complex slide relationships to be constructed.

The appearance of slides is controlled by a template system. Many of the
elements of slides can be adjusted by setting simple key-based values in the
preamble. More complex changes can be implemented by altering specific,
targeted definitions without needing to rewrite entire blocks of code. This
allows a variety of visual appearances to be selected for the same content
source.

## Author

This package is maintained by Joseph Wright: joseph@texdev.net

## License

Released under the LaTeX Project Public License v1.3c or later. See https://www.latex-project.org/lppl.txt



# xbeamer

A re-implementation of `beamer` using `expl3` methods

This is a *development draft*: whether this goes forward to a release and what
form it might take is entirely open.
