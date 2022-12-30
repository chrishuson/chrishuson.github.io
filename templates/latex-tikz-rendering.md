# Render LaTeX code in a MarkDown file (TiKZ)


```latex {cmd=true hide=true}
\documentclass{standalone}
\usepackage{tikz}
\begin{document}
    Hello World!
\end{document}
```

```latex {cmd=true hide=true}
\documentclass{standalone}
\usepackage{tikz}
\begin{document}
  \begin{tikzpicture}[scale=1]
    \draw[thick] (0,0)node[below left]{$P$}--
      (4,0) node[below]{$Q$}--
      (55:4) node[above]{$R$}--cycle;
  \end{tikzpicture}

\end{document}
```