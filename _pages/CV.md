---
layout: page
title: CV
permalink: /CV/
---
\documentclass[11pt,a4paper,sans]{moderncv}        % possible options include font size ('10pt', '11pt' and '12pt'), paper size ('a4paper', 'letterpaper', 'a5paper', 'legalpaper', 'executivepaper' and 'landscape') and font family ('sans' and 'roman')

% moderncv themes
\moderncvstyle{casual}                             % style options are 'casual' (default), 'classic', 'banking', 'oldstyle' and 'fancy'
\moderncvcolor{blue}                               % color options 'black', 'blue' (default), 'burgundy', 'green', 'grey', 'orange', 'purple' and 'red'
%\renewcommand{\familydefault}{\sfdefault}         % to set the default font; use '\sfdefault' for the default sans serif font, '\rmdefault' for the default roman one, or any tex font name
\nopagenumbers{}                                  % uncomment to suppress automatic page numbering for CVs longer than one page

% character encoding
%\usepackage[utf8]{inputenc}                       % if you are not using xelatex ou lualatex, replace by the encoding you are using
%\usepackage{CJKutf8}                              % if you need to use CJK to typeset your resume in Chinese, Japanese or Korean

% adjust the page margins
\usepackage[scale=0.75]{geometry}
%\setlength{\hintscolumnwidth}{3cm}                % if you want to change the width of the column with the dates
%\setlength{\makecvtitlenamewidth}{10cm}           % for the 'classic' style, if you want to force the width allocated to your name and avoid line breaks. be careful though, the length is normally calculated to avoid any overlap with your personal info; use this at your own typographical risks...

% personal data
\name{Declan}{Bennett}
\title{Curriculum vitae}                               % optional, remove / comment the line if not wanted
\address{Scrouthea east}{Clonmel}{Co. Tipperary}% optional, remove / comment the line if not wanted; the "postcode city" and "country" arguments can be omitted or provided empty
\phone[mobile]{+353-85-7571540}                   % optional, remove / comment the line if not wanted; the optional "type" of the phone can be "mobile" (default), "fixed" or "fax"
%\phone[fixed]{+2~(345)~678~901}
%\phone[fax]{+3~(456)~789~012}
\email{declanbennett@hotmail.com}                               % optional, remove / comment the line if not wanted
\homepage{https://bennettdeclan.academia.edu/}                         % optional, remove / comment the line if not wanted
\social[linkedin]{declan-bennett}                        % optional, remove / comment tscientifiche line if not wanted
%\social[twitter]{jdoe}                             % optional, remove / comment the line if not wanted
\social[github]{declan93}                              % optional, remove / comment the line if not wanted
%\extrainfo{additional information}                 % optional, remove / comment the line if not wanted
%\photo[64pt][0.4pt]{picture}                       % optional, remove / comment the line if not wanted; '64pt' is the height the picture must be resized to, 0.4pt is the thickness of the frame around it (put it to 0pt for no frame) and 'picture' is the name of the picture file
%\quote{Some quote}                                 % optional, remove / comment the line if not wanted

% bibliography adjustements (only useful if you make citations in your resume, or print a list of publications using BibTeX)
%   to show numerical labels in the bibliography (default is to show no labels)
\makeatletter\renewcommand*{\bibliographyitemlabel}{\@biblabel{\arabic{enumiv}}}\makeatother
%   to redefine the bibliography heading string ("Publications")
%\renewcommand{\refname}{Articles}

% bibliography with mutiple entries
%\usepackage{multibib}
%\newcites{book,misc}{{Books},{Others}}
%----------------------------------------------------------------------------------
%            content
%----------------------------------------------------------------------------------
\begin{document}
%\begin{CJK*}{UTF8}{gbsn}                          % to typeset your resume in Chinese using CJK
%-----       resume       ---------------------------------------------------------
\makecvtitle

\section{Education}
\cventry{2016}{BSc. Biotechnology}{NUI Galway}{Galway}{\textit{2.1}}{Modules: Biochemistry, Microbiology, Industrial Processes, French, Genetics, Pharmacology and Business} 
\cventry{2017}{MSc. Biomedical Genomics}{NUI Galway}{Galway}{\textit{1.1}}{NGS data analysis, Bioinformatics, Programming, Statistical Computing in R, Medical Genomics and Probabilistic Models }% arguments 3 to 6 can be left empty


\section{Research Experience}
\subsection{Master Thesis}
\cvitem{Title}{\emph{Inferring the somatic mutation rate from population NGS data}}
\cvitem{Supervisor}{Prof. Cathal Seoighe}
\cvitem{Description}{The somatic mutation
rate was estimated using overlapping paired-end exome sequencing data. This estimated
rate was then treated as a quantitative trait and used as the basis of an association study,
in order to uncover genetic loci associated with an elevated somatic mutation rate in
multiple human populations}
%\begin{itemize}%
%\item Winner of the inaugoral Roche prize for best MSc Biomedical Genomics research project;
%\end{itemize}
\subsection{BSc Final Year Project}
\cvitem{Title}{\emph{A neurocognitive analysis of genes that are both associated with memory
formation and schizophrenia}}
\cvitem{Supervisor}{Dr. Derek Morris}
%\cvitem{description}{}
\section{Achievements}
%\begin{itemize}%
\cventry{2017}{Winner of the inaugural Roche prize for best MSc Biomedical Genomics research project}{}{}{}{}
%\end{itemize}
\section{Experience}
%\subsection{Vocational}
\cventry{October 2017 -- Present}{Bioinformatics Internship}{Supervisor: Prof Cathal Seoighe}{NUI Galway}{Investigation of genes in cancer under selection for downregulation via NMD. Investigation of transcription-associated strand asymmetry in highly expressed ASE haplotypes.}{}
\cventry{April 2015 -- July 2015}{Research Assistant}{Laboratoire de Biotechnologie et Chimie Marines}{Vannes}{France}{Performing biochemical analysis of highly proliferative red seaweed, \textit{Solieria Chordalis}.}
%\cventry{May 2014 -- Aug 2014}{Sales assistant}{Country Pork}{Clonmel}{}{Selling and preparing cold and cooked meats. Maintaining standards outlined in the HACCP. Complying with all health, sanitation and legal regulations\newline}%
%Detailed achievements:%

\cventry{May 2013 -- Apr 2014}{Electrical trade assistant}{Electrical Energy}{Sydney, NSW}{Australia}{Installation of high-voltage insulated switch gear\newline{} Managing cable installation}
%\subsection{Miscellaneous}
%\cventry{year--year}{Job title}{Employer}{City}{}{Description}
%\newpage
\section{Skills}
\cvlistitem{In depth knowledge of Next Generation Sequencing technologies}
\cvlistitem{Extensive experience in statistical programming languages and genome
association analysis toolsets mainly R and plink}
\cvlistitem{
Familiar with shell scripting and working at the command line}
\cvlistitem{Experience in Python scripting language}
\cvlistitem{Comfortable working with unix based operating systems}
\cvlistitem{Significant report writing and presentation experience}
\cvlistitem{Strong data analysis and visualisation skills developed through taught
modules and research}
\cvlistitem{Strong collaboration and team working skills demonstrated throughout my
studies and at work}
\cvlistitem{
Adaptable and flexible individual who is highly motivated and excited by new
opportunities/challenges - happily applied myself in a variety of distinct roles}
\cvlistitem{Active decision maker and strong attention to detail}
\cvlistitem{Excellent work ethic and commitment to quality}
\cvlistitem{Ability to take own initiative when necessary}


\section{Computer skills}
\cvdoubleitem{category 1}{R, Python}{category 4}{Unix environment}
\cvdoubleitem{category 2}{Microsoft office}{category 5}{High performance computing}
\cvdoubleitem{category 3}{Bash scripting}{category 6}{Plink}

\section{Interests}
\cvitem{Cycling}{Avid road cyclist}
\cvitem{Music}{Amateur guitar and piano}
%\cvitem{hobby 3}{Descriptioscientificn}

%\section{Extra 1}
%\cvlistitem{Item 1}
%\cvlistitem{Item 2}
%\cvlistitem{Item 3. This item is particularly long and therefore normally spans over several lines. Did you notice the indentation when the line wraps?}

%\section{Extra 2}
%\cvlistdoubleitem{Item 1}{Item 4}
%\cvlistdoubleitem{Item 2}{Item 5\cite{book1}}
%\cvlistdoubleitem{Item 3}{Item 6. Like item 3 in the single column list before, this item is particularly long to wrap over several lines.}

\section{References}
\subsection{}
\newcommand{\cvreference}[7]{%
    \textbf{#1}\newline% Name
    \ifthenelse{\equal{#2}{}}{}{\addresssymbol~#2\newline}%
    \ifthenelse{\equal{#3}{}}{}{#3\newline}%
    \ifthenelse{\equal{#4}{}}{}{#4\newline}%
    \ifthenelse{\equal{#5}{}}{}{#5\newline}%
    \ifthenelse{\equal{#6}{}}{}{\emailsymbol~\texttt{#6}\newline}%
    \ifthenelse{\equal{#7}{}}{}{\phonesymbol~#7}}

\newcommand{\cvdoublecolumn}[2]{%
  \cvitem[0.75em]{}{%
    \begin{minipage}[t]{\listdoubleitemcolumnwidth}#1\end{minipage}%
    \hfill%
    \begin{minipage}[t]{\listdoubleitemcolumnwidth}#2\end{minipage}%
    }%
}

\cvdoublecolumn{\cvreference{Prof Cathal Seoighe}
	{Established Professor of Bioinformatics}
    {School of Mathematics, Statistics and Applied Mathematics}
    {National University of Ireland, Galway}
    {}
    {cathal.seoighe@nuigalway.ie}
    {}
    {}%
    }
    {\cvreference{Dr Pilib \'{O} Broin}
    {Lecturer in Bioinformatics}
    {School of Mathematics, Statistics and Applied Mathematics}
    {National University of Ireland, Galway}
    {}
    {pilib.obroin@nuigalway.ie}
    {+353 91 49 2337 }%
    }
%\cvitem{}{\emph{References available upon request}}
%\begin{cvcolumns}
%  \cvcolumn{}{\begin{itemize}\item Cathal Seoighe \item \item Person 3\end{itemize}}
%  \cvcolumn{Category 2}{Amongst others:\begin{itemize}\item Person 1, and\item Person 2\end{itemize}(more upon request)}
%\end{cvcolumns}
% Publications from a BibTeX file without multibib
%  for numerical labels: \renewcommand{\bibliographyitemlabel}{\@biblabel{\arabic{enumiv}}}% CONSIDER MERGING WITH PREAMBLE PART
%  to redefine the heading string ("Publications"): \renewcommand{\refname}{Articles}
\nocite{*}
\bibliographystyle{plain}
\bibliography{publications}                        % 'publications' is the name of a BibTeX file

% Publications from a BibTeX file using the multibib package
%\section{Publications}
%\nocitebook{book1,book2}
%\bibliographystylebook{plain}
%\bibliographybook{publications}                   % 'publications' is the name of a BibTeX file
%\nocitemisc{misc1,misc2,misc3}
%\bibliographystylemisc{plain}
%\bibliographymisc{publications}                   % 'publications' is the name of a BibTeX file

\clearpage
%-----       letter       ---------------------------------------------------------
% recipient data
%\recipient{}{}
%\recipient{Regeneron Recruitment team}{Regeneron\\777 Old Saw Mill River Road\\ Tarrytown\%\New York}
%\date{August 7, 2017}
%\opening{Dear Sir or Madam,}
%\closing{Yours faithfully,}
%\enclosure[Attached]{curriculum vit\ae{}}          % use an optional argument to use a %string other than "Enclosure", or redefine \enclname
%\makelettertitle

%I have enclosed a copy of my Curriculum Vitae for your consideration for any suitable
%positions that may arise.\par
%I completed my BSc in Biotechnology in NUI Galway in 2016 and I have just completed my MSc in Biomedical Genomics. During my undergraduate studies, my
%modules included biochemistry, microbiology, pharmacology, business, immunology
%and French. I also completed a 3-month work placement in a research laboratory in
%France in my third year, which allowed me to build upon my laboratory skills and gain
%valuable hands-on experience. My final year project then allowed me to explore a
%different side of research, as I used computational techniques such as Plink and
%SPSS to investigate genes associated with Schizophrenia and cognitive impairment.\par
%I chose to study the MSc in Biomedical Genomics as it is the first of its kind in Ireland
%and offers a combination of molecular and computational modules. My modules
%include genomic techniques, medical genomics, probabilistic models, statistical
%computing in R, mathematical molecular biology, molecular cancer biology and data
%analysis. During this year, I expanded my understanding of underlying
%scientific principles and technologies and developed quantitative and computational
%skills that enabled me to analyse large datasets generated using the latest genomic %techniques. I am very interested in pursuing a career in the field of bioinformatics or %computational biology, and my recent experience has strengthened my desire to work in this %area.\par
%I am happy to discuss my application with you further and I am available for interview
%at any convenient time. Please feel free to contact me on 085-7571540 or by email
%at declanbennett@hotmail.com.

%\makeletterclosing

%\clearpage\end{CJK*}                              % if you are typesetting your resume in Chinese using CJK; the \clearpage is required for fancyhdr to work correctly with CJK, though it kills the page numbering by making \lastpage undefined
\end{document}

