BeamerPorts
=========

BeamerPorts is my personal project, to develop LaTeX Beamer presentation themes that are not instantly recognisable as Beamer. Specifically, I want to port some great PowerPoint & Powerdot themes to Beamer.

Please send feature requests, bug reports and improvement ideas to the issue tracker.

#### Things to be aware of
The themes depend on these packages:

- TikZ/PGF

- textpos, _without_ the `[absolute]` option


The following features are workarounds because I didn't find the way to hook into some Beamer mechanisms:

- `\sectionframe` should be used instead of `\frame{\sectionpage}`

- `\begin{xplainframe}` and `\end{xplainframe}` should be used instead of `\begin{frame}[plain]` etc.



Median
--------
Median was originally a PowerPoint theme. You can use it like this:

    \usetheme{Median}

If you're compiling with XeLaTeX or LuaLaTeX, you can also do

    \usepackage[no-math]{fontspec}
    \usetheme[beteckna]{Median}

in which case the theme will load the Beteckna fonts. These are GPL fonts that are available from their now defunct website [through WaybackMachine](http://web.archive.org/web/20130517030302/http://gnu.ethz.ch/linuks.mine.nu/beteckna/). They were the most similar to the Twentieth Century fonts in the original PowerPoint theme. Be aware though that there is no bold italic and several European accents are missing.

Klope
------
Klope was ported from the KlopeSpring theme of Powerdot.