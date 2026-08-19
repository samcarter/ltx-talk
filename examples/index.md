<script src="https://texlive.net/cm6-test/cm6.bundle.min.js"></script>
<script src="https://texlive.net/runlatex3-cm6.js"></script>
<script>
function generatepreamble(t,e) {return e.getValue();}
      runlatex.overleafURI=null;
      
      runlatex.texts ={
	  "Open in Overleaf": "",
	  "TeXLive.net":      "Generate Tagged PDF", 
	  "Delete Output":    "Delete Output",
	  "Compiling PDF":    "Compiling Tagged PDF",
          "Added Code":       "",
	  "End Added Code":   "",
	  "Top Caption":      "",
	  "metadata":         ""
      }
runlatex.editorlines=20;

</script>

# Examples of using the `ltx-talk` class

<div style="float:right; width: 8em; padding:1em;border:solid thin black; background-color:#EFEFEF" markdown=1>

  [frame layout](#frame-layout)

  [Lists](#lists)

  [Math](#math)

  [Something](#something)

 </div>

## Introduction

The examples on this page demonstrate various features of the `ltx-talk` class.
The example may be used as-is or may be edited using the built in editor.

The **Generate Tagged PDF** button will run LaTeX (`lualatex-dev`) on the file
and return

* a list of result links to the PDF,
* a validation report using **veraPDF**
* A form showing the structure tree and Validation using `show-pdf-tags`
* The log of the LuaLaTeX run
* A Link to ngPDF which shows the structure tree, the PDF and a derived HTML
  version of the document.

## Lists

Lists are perhaps the most common structure in presentation frames.

### Revealing one items at a time

A very common pattern: reveal the list one item at a time.

```latex
{% include_relative list-overlays.tex %}
```

### Applying actions

Actions can adjust how content appears: here we highlight as we go.

```latex
{% include_relative list-actions.tex %}
```

## Presentation design

### Customizing header colors

Choosing a color scheme for the header and footer is one common way to make a
presentation more visually appealing.

```latex
{% include_relative header-footer-color.tex %}
```

### Inserting background images

Background images are another common customization.

```latex
{% include_relative background-image.tex %}
```

### Ordering frame header and footer items

Currently, control of the content in headers and footers is quite simple: you
can choose the entries and their ordering.

```latex
{% include_relative footer-text.tex  %}
```

### Titlepage styling

There is more control available in terms of the title page.

```latex
{% include_relative titlepage-styling.tex %}
```

### 'Float' alignment

'Floats' do not really float in presentations, but they can still be useful as
part of the overall structure.

```latex
{% include_relative float-centering.tex %}
```

## Math mode

### Math font setup

Math mode works in the standard LaTeX way: here we make some changes to the
font.

```latex
{% include_relative math-fonts.tex %}
```

## Controlling overlays

### Overlay opacity example

Overlays use opacity (transparency) to make material invisible: by adjusting the
amount, part-visible content is possible.

```latex
{% include_relative overlay-opacity.tex %}
```

## Verbatim material

### Verbatim content

The standard approach to verbatim content uses the `frame*` environment.

```latex
{% include_relative verbatim-content.tex %}
```

### Demonstrating the class itself

To show the `frame*` environment itself, a second name is safest: this is shown
here using standard LaTeX commands.

```latex
{% include_relative verbatim-alt-env.tex %}
```

## Presentation structure

### Tracking total frames

Various counters are available: the overall length of the presentation is common
requirement.

```latex
{% include_relative totalframes.tex %}
```
