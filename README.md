<div align="center">
  <img src="Resources/Header.png" width="65%" alt="ISTA LaTeX Templates"/>
  <br><br><br>

  **Not affiliated with ISCTE!**

  <br><br>
</div>

# Master's Dissertation
**Updated for [ISTA's Style Guidelines](https://www.iscte-iul.pt/conteudos/estudantes/informacao-academica/percurso-academico/area-mestrado/926/entrega-de-dissertacao-ou-trabalho-de-projeto) as of July 15th, 2024.**

This template serves as an adaptation of ISTA's style guidelines for dissertations or projects to be used with LaTeX. The template has been structured so that all non-work-related details, such as LaTeX package configurations and the like, are stored in a separate file so as to not hinder the author's writing process.

Your dissertation/project report should begin by defining the work, along with its author and supervisor(s). The following is a barebones example of how this can be achieved in the template.

```tex
\title{Title of a Great Dissertation}

\author{Your Full Name}

\program{Master's in Using LaTeX}

\department{Department of Typesetting}

\supervisor{Doctor}{Supervisor}{Assistant Professor}{Iscte - Instituto Universitário de Lisboa}

\date{Month}{Year}

\acknowledgements{Write here your acknowledgements and, if applicable, any grants or sources of funding.}

\dedication{Write here your dedication.}

\acronyms{
    \acro{DSR}{Design Science Research}
    \acro{IS}{Information System}
}
```

Additionally, you should include an abstract and keywords, remembering to add a second version translated to Portuguese if required.
```tex
\resumo
{
    Escreva aqui o resumo em Português.
}
{ Palavras-chave, separadas, por, vírgulas }

\abstract
{
    Write here the abstract in English.
}
{ Keywords, separated, by, commas }
```

The remainder of your document is written in standard LaTeX within the `document` environment. References are automatically handled by BibTeX. The [ISTA Master's Dissertation](ISTA%20Master's%20Dissertation) folder contains a sample project you can use with [Overleaf](https://www.overleaf.com/) (where it was made!) or similar LaTeX development environments. It contains a pre-structured file with some example content on how to use LaTeX.

<br>

# Research Project Proposal
**Updated for the [Information Science and Technology PhD Research Project Proposal](https://www.iscte-iul.pt/assets/files/2022/08/03/1659547576152_Modelo_de_Projeto_de_Investiga__o_PhD_DCTI.pdf) MS Word template as of July 15th, 2024.**

This LaTeX template is for the Research Project Proposal form required to apply to the [PhD Program in Information Science and Technology](https://www.iscte-iul.pt/course/53/doctorate-degree-phd-in-information-science-and-technology/candidacy) at Iscte. As with the Master's dissertation template, non-work-related information such as LaTeX package configurations is stored in a separate file to facilitate the writing of the form proper. 

Your project proposal should begin by defining information on the author and the supervisor(s), along with the project's title and the program for which you are applying. The following is an example.
```tex
\title{The Title of Your Project}

\program{Doctoral Programme in Information Science and Technology}

\date{Lisboa}{Month}{Day}{Year}

\supervisor{Doctor}{Supervisor}{Assistant Professor}{Iscte - Instituto Universitário de Lisboa}

\candidate {Your Full Name}
```

The remainder of your document is written in standard LaTeX within the `document` environment. References are automatically handled by BibTeX. The [PHD Research Project Proposal](PHD%20Research%20Project%20Proposal) folder contains a sample project with a pre-structured file that you only need to fill out, including the sections which are required by the project proposal guidelines.
