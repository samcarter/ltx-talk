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

  [frame layout](Frame Layout)

  [Lists](Lists)

  [Math](Math)

 
</div>


some general description of the example structure.
some general description of the example structure.
some general description of the example structure.
some general description of the example structure.
some general description of the example structure.




## Frame  Layout

### background images

```latex
{% include_relative background-image.tex %}
```

### head and foot

```latex
{% include_relative footer-text.tex  %}
```

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

## Overays

```latex
{% include_relative overlays-opacity.tex %}
```

```latex
{% include_relative titlepage-styling.tex %}
```

```latex
{% include_relative verbatim-alt-env.tex %}
```

```latex
{% include_relative verbatim-content.tex %}
```



```latex
{% include_relative float-centering.tex %}
```
