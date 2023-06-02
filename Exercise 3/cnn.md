---
author: Behrooz Montazeran, Jannis Heising, Tomáš Sláma
papersize: a4
fontsize: 12pt
header-includes: |
	\usepackage{graphicx}
	\usepackage{fancyhdr}
	\usepackage[czech]{babel}
	\pagestyle{fancy}
	\lhead{ML Exercise 3}
	\rhead{Behrooz Montazeran, Jannis Heising, Tomáš Sláma}
	\setlength{\headheight}{20pt}
	\AtBeginDocument{\let\maketitle\relax}
	\renewcommand{\headrulewidth}{0.4pt}
	\renewcommand{\footrulewidth}{0.4pt}
geometry: margin=2.5cm
engine: lualatex
---

See the notebooks for answers to exercises 1-3.

# Exercise 4: CNN

## Network sketch

\begin{center}
\includegraphics[width=.8\linewidth]{ex_4_network_sketch}
\end{center}

## Sample image from test set

\begin{center}
\includegraphics[width=.4\linewidth]{ex_4_input}
\end{center}

## Three filters applied

\begin{center}
\includegraphics[width=.8\linewidth]{ex_4_filtered_input}
\end{center}

## Removing one convolutional layer

\begin{center}
\includegraphics[width=.4\linewidth]{ex_4_loss}
\includegraphics[width=.4\linewidth]{ex_4_loss_reduced}
\end{center}

The blue line is the training error and the orange line is the test error. The smaller network actually performed better than the initial one. This suggests that the proposed architecture is too large for the task at hand.
