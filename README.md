# LaTeX Journal Template
Custom commands and formatting for a journal using LaTeX, based on the `memoir` class. [Example output.](journal_main.pdf)

## Custom Commands
- `\newyear{<year>}` – Start a new year
- `\newday{<date>}{<header>}` – Start a daily entry
    - `date` – The date in YYYY-MM-DD format
    - `header` – Right-aligned title text, I use this for special events
- `\addcontents{<text>}` – Adds the text to the Table of Contents (TOC), without adding the text to the document
    - `text` – The TOC text
- `\retro{<header>}` – Add a retrospective entry, automatically added to TOC
    - `header` – The title of the entry
- `\degrees` – Degrees symbol
- `\begin{myblockquote}` – Start a block quote

## Other Useful Commands
- `\medbreak` – Add some whitespace
- `\needspace{<lines>\baselineskip}` – If an image is too low on the page to fit, this ensures that it will move to the next page instead of overflowing
- `\setlength{\parindent}{0cm}` – Change the paragraph indentation, I occasionally use this in block quotes
- Lists:
```
\begin{itemize}
\item First item
\item Second item
\end{itemize}
```
- `\includegraphics[width=<width>]{<filename>}` – Add an image from the `img` directory
    - `width` – I usually use `\textwidth` or multiply it (`0.5\textwidth`) to get a relative size
    - `filename` – The filename
- `\begin{wrapfigure}{<position>}{<width>}` – Image with text wrapping, check the [documentation](https://mirror.its.dal.ca/ctan/macros/latex/contrib/wrapfig/wrapfig-doc.pdf) or [Overleaf](https://www.overleaf.com/learn/latex/wrapping_text_around_figures)
    - `position` - I usually use `l` or `r`
    - `width` – Same as above
- `\begin{figure}[h]` – Images without text wrapping

## Image Attribution
<img src="img/wide.jpg" alt="drawing" width="200px"/>

[Jametlene Reskp on Unsplash](https://unsplash.com/photos/VDrErQEF9e4)

<img src="img/tall.jpg" alt="drawing" width="200px"/>

[Stephanie Cook on Unsplash](https://unsplash.com/photos/0yHhzZi2wPI)
