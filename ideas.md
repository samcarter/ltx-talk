# Random ideas of things that might or might not get implemented

## using LaTeX's standard shipout routine and box
- set the margins of the document to cover the style elements, such that the
    text block (`\textheight` and `\textwidth`) really just covers the content
    area of a frame
- use `shipout/background` and `shipout/foreground` to draw the current style's
    elements, frame title, etc.
- use `\newgeometry`/`\restoregeometry` to adapt the text block for special
    slides like the title frame

## Things that are a bit painful in current beamer

- maybe overlays and framebreaks could be consolidated? The concept of overlays works really well, but framebreaks have always been troublesome. Does it need two different concepts? What if framebreaks would become normal overlays?
- customising navigations bars beyond simple changes, like colour or fonts, is not trivial with current beamer. Maybe xbeamer is a chance to think of an approach which is easier to customise.
- open the `\mode` mechanism for user defined modes. Inspired by the `beameraudience` package, this might be handy to produce presentations for different languages, medias, audiences etc. at the same time
- maybe one could get some inspiration from the `boxes` theme or `hackthefootline` package on how to make footlines and headlines more modular 



