# 🎓 PhD Thesis

> [!IMPORTANT]
> If you're using Overleaf (you should; it's great), we recommend compiling the templates with LuaLaTeX and using TeX Live Version 2024.

This LaTeX template is for your PhD Thesis, or for the yearly reports for the same doctoral programme at Iscte. As with the previous templates, non-work-related information such as LaTeX package configurations is stored in a separate file.

The package can be used in two ways, depending on if you want your thesis document or a yearly report.

For the thesis proper:
```tex
\usepackage{dcti}
```

For yearly reports:
```tex
\usepackage[report]{dcti}
```

Your thesis should begin by defining information on the thesis, namely, its title, author's name, supervisor(s), jury / supervision committee, doctoral programme name, department name, and date.
```tex
\title{Title of a Great PhD Thesis}

\author{Your Full Name}

\program{Name of the Doctoral Programme}{Your PhD Specialty}

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


\jury
{Ph.D. Professor John}
{Iscte - Instituto Universitário de Lisboa}

\jury
{Ph.D. Professor Alice}
{Iscte - Instituto Universitário de Lisboa}

\jury
{Ph.D. Professor Jane}
{Iscte - Instituto Universitário de Lisboa}

\jury
{Ph.D. Professor Doe}
{Anonymous University, Department of ???, Typesetting Research Center}


% Submission Date (Month, Year)
\date{Month}{Year}
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
- All these fields must be defined: the thesis title, programme name, department name, author name, and submission date (month and year);
  - Months should be capitalised and fully written out, e.g. "January" instead of "january" or "Jan";
  - The thesis submission year should be greater than or equal to the current year.
- The thesis must have at least 1 supervisor, and no more than 3;
- The thesis monitoring committee / defence jury must have exactly 4 members.

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