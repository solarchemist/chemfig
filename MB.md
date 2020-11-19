# Methylene blue
<script type="application/ld+json">
{
  "@context":         "https://schema.org",
  "@type":            "MolecularEntity",
  "molecularFormula": "C16H18ClN3S",
  "smiles":           "CN(C)c1ccc2c(c1)sc-3cc(=[N+](C)C)ccc3n2.[Cl-]",
  "url":              "https://solarchemist.github.io/chemfig/MB.html"
}
</script>

## info

* Molecular formula: C<sub>16</sub>H<sub>18</sub>ClN<sub>3</sub>S
* SMILES: CN(C)c1ccc2c(c1)sc-3cc(=[N+](C)C)ccc3n2.[Cl-]
* [Wikimedia](https://commons.wikimedia.org/wiki/File:Methylene_blue.svg)

![Chemical structure formula](MB.svg)


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
      [7]H_3C-N(-[6]CH_3)-[:30]*6(=-%
      (*6(=\charge{-90:1.5pt=\scalebox{0.75}{\textbf{\fsscrp}}}{S}%
      (-[,1.05,,,draw=none]\charge{90:0.5pt=\scalebox{0.75}{\textbf{\fsscrm}}}{Cl})-%
      (*6(-=(-N(-[1]CH_3)-[6]CH_3)-=-=))--N=-))--=-)%
   }};
\end{tikzpicture}
\end{document}
```
