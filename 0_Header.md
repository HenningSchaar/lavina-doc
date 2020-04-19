---
documentclass: article
classoption: 
- oneside
fontsize: 11pt
geometry:
- a4paper
- left=3cm
- right=3cm
- top=2cm
- bottom=2cm
- bindingoffset=0.5cm
bibliography: Meine Bibliothek.bib
csl: hennings-bachelorarbeit-samac-et-al.csl
date: \today
header-includes: |
 \usepackage[T1]{fontenc}
 \usepackage{baskervillef}
 \usepackage[varqu,varl,var0]{inconsolata}
 \usepackage[scale=.95,type1]{cabin}
 \usepackage[baskerville,vvarbb]{newtxmath}
 \usepackage[cal=boondoxo]{mathalfa}
 \usepackage{blindtext}
 \usepackage[english]{babel}
 \usepackage{ragged2e}
 \usepackage{tocloft}
 \usepackage[utf8]{inputenc}
 \usepackage[export]{adjustbox}
 \usepackage{graphicx}
 \graphicspath{ {Graphics/} }
 \usepackage[font=small,labelfont=bf]{caption}
 \usepackage[rightcaption]{sidecap}
 \usepackage[right]{eurosym}
 \usepackage{lmodern}
 \usepackage{fancyhdr}
 \usepackage{color}
 \usepackage{amssymb}
 \usepackage{mathtools}
 \usepackage{capt-of}
 \usepackage[german]{nomencl}
 \let\abbrev\nomenclature
 \newcommand{\changefont}{%
    \fontsize{9}{11}\selectfont}
 \usepackage{chngcntr}
 \counterwithin{figure}{section}
 \counterwithin{table}{section}
 \setcounter{tocdepth}{4} 
 \usepackage[onehalfspacing]{setspace}
...



\pagenumbering{gobble}



\title{Lavina: Sound Engine based on Swarm Behaviour for Novel 3D Audio Composition Techniques}
\date{2020, April}
\author{Jonas Ohland and Henning Schaar, University Of Applied Sciences Darmstadt}

\maketitle

\section*{Abstract}

The motion of a flock of birds is a common phenomenon in nature, which can be seen in other organisms such as schools of fish or herds of land animals. A flock can be understood as a particle system which operates under certain rules that result in complex behaviour. 
One way to model this behaviour in computer sciences is to model the paths of each bird or particle individually. Lavina is such a model, with the added functionality of sound synthesis for each particle which is then represented in acoustic space. Composers may use Lavina to create a timeline for parameter changes to the flocking behaviour as well as the sound generation to create novel compositions with unexpected outcomes while retaining artistic control over the final performance.

\justifying 

\pagenumbering{arabic}

\pagestyle{fancy}
\fancyhf{}
\renewcommand{\footrulewidth}{0.2pt}
\renewcommand{\headrulewidth}{0pt}
\fancyfoot[LO]{\changefont Jonas Ohland, Henning Schaar | University of Applied Sciences Darmstadt | 2020}
\fancyfoot[RO,LE]{\thepage}

\twocolumn 
