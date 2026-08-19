---
title: "Tagging of Heading Structures in LaTeX"
---

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

# Ltx-talk Examples

<div style="float:right; width: 8em; padding:1em;border:solid thin black; background-color:#EFEFEF" markdown=1>

  [frame layout](#frame-layout)

  [Lists](#lists)

  [Math](#math)

  [Something](#something)

 
</div>

## Introduction

The examples on this page demonstrate various features of the `ltx-talk` class.
The example may be used as-is or may be edited using the built in editor.

The **Generate Tagged PDF** button will run LaTeX (`lualatex-dev`) on the file and return

* a list of result links to the PDF,
* a validation report using **veraPDF**
* A form showing the structure tree and Validation using `show-pdf-tags`
* The log of the lualatex run
* A Link to ngPDF which shows the structure tree, the PDF and a derived HTML version of the document.




## Frame Layout

### Background Images

```latex
{% include_relative background-image.tex %}
```

### ordering frame header and footer items

```latex
{% include_relative footer-text.tex  %}
```

### Customising colors

```latex
{% include_relative header-footer-color.tex %}
```

### frame counters


```latex
{% include_relative totalframes.tex %}
```

## Lists

### actions
```latex
{% include_relative lists-actions.tex %}
```

### overlays

```latex
{% include_relative lists-overlays.tex %}
```

## Math

### Math Font setup
```latex
{% include_relative math-fonts.tex %}
```

## Something

### Overlay Opacity example
```latex
{% include_relative overlays-opacity.tex %}
```

### titlepage styling
```latex
{% include_relative titlepage-styling.tex %}
```

### Verbatim 1
```latex
{% include_relative verbatim-alt-env.tex %}
```

### Verbatim 2

```latex
{% include_relative verbatim-content.tex %}
```


### Float alignment

```latex
{% include_relative float-centering.tex %}
```
