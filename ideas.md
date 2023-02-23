# Random ideas of things that might or might not get implemented

## using LaTeX's standard shipout routine and box
- set the margins of the document to cover the style elements, such that the
    text block (`\textheight` and `\textwidth`) really just cover the content
    area of a frame
- use `shipout/background` and `shipout/foreground` to draw the current style's
    elements, frame title, etc.
- use `\newgeometry`/`\restoregeometry` to adapt the text block for special
    slides like the title frame
