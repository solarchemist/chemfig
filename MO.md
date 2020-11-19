# Methyl orange
<script type="application/ld+json">
{
  "@context":         "https://schema.org",
  "@type":            "MolecularEntity",
  "molecularFormula": "C14H14N3NaO3S",
  "smiles":           "[Na+].CN(C)c2ccc(/N=N/c1ccc(cc1)S([O-])(=O)=O)cc2",
  "url":              "https://solarchemist.github.io/chemfig/MO.html"
}
</script>

## info

* Molecular formula: C<sub>14</sub>H<sub>14</sub>N<sub>3</sub>NaO<sub>3</sub>S
* SMILES: [Na+].CN(C)c2ccc(/N=N/c1ccc(cc1)S([O-])(=O)=O)cc2
* [Wikimedia](https://commons.wikimedia.org/wiki/File:Methyl_orange.svg)

![Chemical structure formula](MO.svg)


## chemfig

```latex
% this file may be compiled with: `pdflatex --shell-escape <filename>.tex`
\documentclass[12pt,border=-2pt,tikz,convert=pdf2svg]{standalone}
\usepackage[T1]{fontenc}
\usepackage[latin1]{inputenc}
\usepackage{lmodern}
\usepackage{chemfig,chemmacros}
\usechemmodule{charges}
\renewcommand*{\familydefault}{\sfdefault}
\renewcommand*\printatom[1]{\ensuremath{\mathsf{#1}}}
\setchemfig{atom sep=1.5em}
\setchemfig{double bond sep=.6ex}
\setchemfig{bond style={thick,cap=round}}
\pagestyle{empty}
\begin{document}
\begin{tikzpicture}
   \node (n1) {\chemfig{
      ([7]H_3C-N(-[5]H_3C)-[:0]%
      *6(=-=(-N=[::60]N-*6(=-=(-S(=[::+90]O)(=[::-90]O)%
      (-\charge{20=\scalebox{0.75}{\textbf{\fsscrm}}}{O}-%
      [,1.15,,,draw=none]\charge{160:0.5pt=\scalebox{0.75}{\textbf{\fsscrp}}}{Na}))%
      -=-))-=-))%
   }};
\end{tikzpicture}
\end{document}
```
