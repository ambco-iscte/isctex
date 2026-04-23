# 🎓 PhD Research Project Proposal

> [!IMPORTANT]
> If you're using Overleaf (you should; it's great), we recommend compiling the templates with LuaLaTeX and using the latest TeX Live version. **If your compilation times out (Overleaf is becoming increasingly stricter with compilation time limits for free accounts...), you may need to consider using the paid plan (monthly subscription) or a local TeX editor installed on your system (free).**

This LaTeX template is for the Research Project Proposal form required to apply to the [PhD Program in Information Science and Technology](https://www.iscte-iul.pt/course/53/doctorate-degree-phd-in-information-science-and-technology/candidacy) at Iscte. As with the Master's dissertation template, non-work-related information such as LaTeX package configurations is stored in a separate file to facilitate the writing of the form proper. 

The template can be used by importing the corresponding package at the beginning of the document:

```tex
\documentclass{proposal}
```

Your project proposal should begin by defining information on the author and the supervisor(s), along with the project's title and the program for which you are applying. The following is an example.
```tex
\title{The Title of Your Project}

\program{Doctoral Programme in Information Science and Technology}

\supervisor
{Ph.D. Professor Alice, Assistant Professor}
{Iscte - Instituto Universitário de Lisboa}

\supervisor
{Ph.D. Professor Bob, Assistant Professor}
{Iscte - Instituto Universitário de Lisboa}

\supervisor
{Ph.D. Professor Mallory, Assistant Professor}
{Iscte - Instituto Universitário de Lisboa}

\candidate{Your Full Name}
```

The remainder of your document is written in standard LaTeX within the `document` environment. References are automatically handled by BibLaTeX.

Unlike the other two templates, the Research Project Proposal template **does not check for sections exceeding their respective word limits**. You can check this yourself by pasting a snippet of LaTeX code into [this website](https://app.uio.no/ifi/texcount/online.php).