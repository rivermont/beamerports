BeamerPorts
=========

BeamerPorts is my personal project, to develop LaTeX Beamer presentation themes that are not instantly recognisable as Beamer. Specifically, I want to port some great PowerPoint & Powerdot themes to Beamer.

Please send feature requests, bug reports and improvement ideas to the issue tracker.

Median
--------
Median was originally a PowerPoint theme. You can use it like this:

    \usetheme{Median}

If you're compiling with XeLaTeX or LuaLaTeX, you can also do

    \usepackage[no-math]{fontspec}
    \usetheme[beteckna]{Median}

in which case the theme will load the Beteckna fonts. These are GPL fonts that were obtained from their now defunct website through WaybackMachine. They were the most similar to the Twentieth Century fonts in the original PowerPoint theme. Be aware though that there is no bold italic.

#### Things to be aware of
The theme depends on these packages:
- TikZ/PGF
- datetime
- textpos, _without_ the `[absolute]` option


The following features are workarounds because I didn't find the way to hook into some Beamer mechanisms:
- `\sectionframe` should be used instead of `\frame{\sectionpage}`
- `\begin{xplainframe}` and `\end{xplainframe}` should be used instead of `\begin{frame}[plain]` etc.

