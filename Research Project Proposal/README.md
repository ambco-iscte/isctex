# 🎓 PhD Research Project Proposal

> [!IMPORTANT]
> If you're using Overleaf (you should; it's great), we recommend compiling the templates with LuaLaTeX and using TeX Live Version 2024.

This LaTeX template is for the Research Project Proposal form required to apply to the [PhD Program in Information Science and Technology](https://www.iscte-iul.pt/course/53/doctorate-degree-phd-in-information-science-and-technology/candidacy) at Iscte. As with the Master's dissertation template, non-work-related information such as LaTeX package configurations is stored in a separate file to facilitate the writing of the form proper. 

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