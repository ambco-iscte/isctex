# 🎓 Master's Dissertation

> [!IMPORTANT]
> If you're using Overleaf (you should; it's great), we recommend compiling the templates with LuaLaTeX and using TeX Live Version 2024.

> [!WARNING]
> Sometimes (it depends on who verifies your dissertations' style guidelines compliance), ISTA asks that the Introduction chapter, and possibly the Conclusion chapter, not be numbered. To do this, you can append an asterisk to the `\chapter`, `\section`, `\subsection`, and `\subsubsection` commands to remove the numbering. For example: `\chapter*{Not a Numbered Chapter}`.

This template serves as an adaptation of ISTA's style guidelines for dissertations or projects to be used with LaTeX. The template has been structured so that all non-work-related details, such as LaTeX package configurations and the like, are stored in a separate file so as to not hinder the author's writing process.

The template can be used in two ways, depending on if you want your thesis document to include the ISCTE Business School logo (for the Master's in Data Science) or not (for the remaining Master's programmes).

For students of the Master's in Data Science (which is under joint tutelage of ISTA and IBS):

```tex
\usepackage[ibs]{dissertation}
```

For students of the Master's in Computer Science and Engineering or the Master's in Telecommunications Engineering:

```tex
\usepackage{dissertation}
```

Your dissertation/project report should begin by defining the work, along with its author and supervisor(s). The following is a barebones example of how this can be achieved in the template.

```tex
\title{Title of a Great Dissertation}

\author{Your Full Name}

\program{Master's in Using LaTeX}

\department{Department of Typesetting}

\supervisor
{Ph.D. Professor Alice, Assistant Professor}
{Iscte - Instituto Universitário de Lisboa}

\supervisor
{Ph.D. Professor Bob, Assistant Professor}
{Iscte - Instituto Universitário de Lisboa}

\supervisor
{Ph.D. Professor Mallory, Assistant Professor}
{Iscte - Instituto Universitário de Lisboa}

\date{Month}{Year}

\acknowledgements{Write here your acknowledgements and, if applicable, any grants or sources of funding.}

\dedication{Write here your dedication.}

\acronyms{
    \acro{DSR}{Design Science Research}
    \acro{IS}{Information System}
}
```

Additionally, you should include an abstract and keywords, both in English and Portuguese.
```tex
% Resumo, em Português
\begin{resumo}
Escreva aqui o resumo em Português. Existe um limite de 250 palavras. A tese deverá ter um Resumo em português e um em inglês (Abstract), contudo poderá também ter em outros idiomas, para além destes dois.

\keyword{Palavras-chave}
\keyword{separadas}
\keyword{por}
\keyword{vírgulas}
\end{resumo}

% Abstract, in English
\begin{abstract}
Write here the abstract in English. There is a 250 word limit. Your thesis should have an abstract in English and one in Portuguese (Resumo), however, it may have additional abstracts in other languages.

\keyword{Keywords}
\keyword{separated}
\keyword{by}
\keyword{commas}
\end{abstract}
```

The remainder of your document is written in standard LaTeX within the `document` environment. References are automatically handled by BibLaTeX.

The template checks your document the following restrictions, and will warn you if anything is out of place (so just relax and write):

- The Resumo and Abstract sections each have a 250 word limit. If you want to check your word counts manually, you can do so by pasting a snippet of LaTeX code into [this website](https://app.uio.no/ifi/texcount/online.php);
- The Resumo and Abstract sections should declare the same number of keywords, no less than 3 and no more than 6;
- All these fields must be defined: the dissertation title, programme name, department name, author name, and submission date (month and year);
  - Months should be capitalised and fully written out, e.g. "January" instead of "january" or "Jan";
  - The thesis submission year should be greater than or equal to the current year.
- The dissertation must have at least 1 supervisor, and no more than 2.

<br>

<details>
<summary><b>Notes on Compiling Locally</b></summary>

To compile the template locally, we recommend using [MiKTeX](https://miktex.org/) on Windows, and [TinyTex](https://yihui.org/tinytex/#for-other-users) on Linux, since both* can resolve package installations. We've had the best luck compiling with LuaLaTeX.

```bash
# inside the ISTA Master's Dissertation folder:
lualatex -shell-escape main.tex
```
<sup>*TinyTex resolves packages if you compile in R, using `tinytex::lualatex`; even then, in our experience it's not great. We recommend
doing `tlmgr install scheme-full` if you're having issues with the compilation.</sup>
</details>