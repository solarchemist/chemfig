# Water
<script type="application/ld+json">
{
  "@context":         "https://schema.org",
  "@type":            "MolecularEntity",
  "molecularFormula": "C20H12N3O7SNa",
  "smiles":           "C1=CC=C2C(=C1)C=CC(=C2O)/N=N/C3=C4C=CC(=CC4=C(C=C3O)S(=O)(=O)[O-])[N+](=O)[O-].[Na+]",
  "url":              "https://solarchemist.github.io/chemfig/EBT.html"
}
</script>

## info

* Molecular formula: C<sub>20</sub>H<sub>12</sub>N<sub>3</sub>O<sub>7</sub>SNa
* SMILES: C1=CC=C2C(=C1)C=CC(=C2O)/N=N/C3=C4C=CC(=CC4=C(C=C3O)S(=O)(=O)[O-])[N+](=O)[O-].[Na+]

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
\renewcommand*\printatom[1]{\ensuremath{\mathsf{#1} } }
\setchemfig{atom sep=1.5em}
\setchemfig{double bond sep=.6ex}
\setchemfig{bond style={thick,cap=round} }
\pagestyle{empty}
\begin{document}
\begin{tikzpicture}
   \node (n1) {\chemfig{ %
      ([:-30]*6((-=^[::+60]-[::+60]=^[::+60]-[::+60])=-(-OH)=%
      (-N=[::60]N-*6(=(-OH)-=(-S(=[::+90]O)(=[::-90]O)%
      (-\charge{30=\textbf{\fsscrm} }{O}-%
      [,1.25,,,draw=none]\charge{155:1pt=\textbf{\fsscrp} }{Na}))-%
      *6(-=(-NO_2)-=--)=-))-=-))%
   } };
\end{tikzpicture}
\end{document}
```

