# Reactive black 5
<script type="application/ld+json">
{
  "@context":         "https://schema.org",
  "@type":            "MolecularEntity",
  "molecularFormula": "C26H21N5Na4O19S6",
  "smiles":           "C1=CC(=CC=C1N=NC2=C(C3=C(C(=C(C=C3C=C2S(=O)(=O)[O-])S(=O)(=O)[O-])N=NC4=CC=C(C=C4)S(=O)(=O)CCOS(=O)(=O)[O-])N)O)S(=O)(=O)CCOS(=O)(=O)[O-].[Na+].[Na+].[Na+].[Na+]",
  "url":              "https://solarchemist.github.io/chemfig/RB5.html"
}
</script>

## info

* Molecular formula: C<sub>26</sub>H<sub>21</sub>N<sub>5</sub>Na<sub>4</sub>O<sub>19</sub>S<sub>6</sub> 
* SMILES: C1=CC(=CC=C1N=NC2=C(C3=C(C(=C(C=C3C=C2S(=O)(=O)[O-])S(=O)(=O)[O-])N=NC4=CC=C(C=C4)S(=O)(=O)CCOS(=O)(=O)[O-])N)O)S(=O)(=O)CCOS(=O)(=O)[O-].[Na+].[Na+].[Na+].[Na+]
* [Wikimedia](https://commons.wikimedia.org/wiki/File:Reactive_Black_5.svg)

![Chemical structure formula](RB5.svg)


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
\definesubmol{sulfonateright}{
   -S(=[::+90]O)(=[::-90]O)-\charge{20=\textbf{\fsscrm}}{O}-
   [:0,1.2,,,draw=none]\charge{160:0.5pt=\textbf{\fsscrp}}{Na}}
\definesubmol{sulfonateleftlower}{
   \charge{20=\textbf{\fsscrp}}{Na}-
   [:0,1.2,,,draw=none]\charge{160:0.5pt=\textbf{\fsscrm}}{O}-
   S(=[::+90]O)(=[::-90]O)-O}
\definesubmol{sulfonateleftupper}{
   O-S(=[::+90]O)(=[::-90]O)-\charge{160:0.5pt=\textbf{\fsscrm}}{O}-
   [:180,1.2,,,draw=none]\charge{20=\textbf{\fsscrp}}{Na}}
\definesubmol{upperbranch}{
   -N=[:180]N-[::0]*6(-=-(-S(=[::+90]O)
   (=[::-90]O)--[::-60]-!{sulfonateleftupper})=-=)}
\begin{tikzpicture}
   \node (n1) {\chemfig{
      % lower branch, from left-to-right
      [:0]!{sulfonateleftlower}-[:0]-[:60]-[:0]S(=[::+90]O)(=[::-90]O)-[:0]
      % single six-ring on lower branch starts here
      *6(-=-(-N=N-[:60]*6(-(!{sulfonateright})=-*6(-=(!{sulfonateright})-
      (!{upperbranch})=(-HO)-)=-(-H_2N)=))=-=)
   }};
\end{tikzpicture}
\end{document}
```
