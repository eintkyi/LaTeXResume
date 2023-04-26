# LaTeXResume
Resume compiled in LaTeX


\documentclass[letterpaper,11pt]{article}
\usepackage[T1]{fontenc}
\usepackage{titlesec}
\usepackage{tgbonum}
\RequirePackage[default,semibold]{sourcesanspro}
\RequirePackage[10pt]{moresize}
\usepackage{anyfontsize}
\RequirePackage{csquotes}


%-----------------------------------------------------------
\usepackage[empty]{fullpage}
\usepackage{geometry}
\usepackage{ragged2e}
\usepackage[usenames,dvipsnames]{xcolor}
\definecolor{highlight}{RGB}{12, 90, 130} 
\raggedbottom
\setlength{\tabcolsep}{0in}
\RequirePackage[inline]{enumitem}
\setlength{\tabcolsep}{0in}


% Adjust margins to 0.5in on all sides
\addtolength{\oddsidemargin}{-0.5in}
\addtolength{\evensidemargin}{-0.5in}
\addtolength{\textwidth}{1.0in}
\addtolength{\topmargin}{-0.5in}
\addtolength{\textheight}{1.0in}

%-----------------------------------------------------------
%Custom commands
\newcommand{\resitem}[1]{\item #1 \vspace{-2pt}}

\newcommand{\ressubheading}[4]{
\begin{tabular*}{6.5in}{l@{\extracolsep{\fill}}r}
		\textbf{#1} & #2 \\
		\textit{#3} & \textit{#4} \\
\end{tabular*}\vspace{-6pt}}
\usepackage[absolute,overlay]{textpos}

\RequirePackage[nostruts]{titlesec}
\titlespacing{\section}{0em}{0.5em}{0em}
\titleformat{\section}{\color{highlight} \scshape \raggedright \large}{}{0em}{}[\vspace{-0.75em}\hrulefill]
% SUBSECTION FORMATTING
\titlespacing*{\subsection}{0em}{0em}{0em}
\titleformat{\subsection}{\bfseries}{}{0em}{}[]
% SUBTEXT
\newcommand{\subtext}[1]{\textit{#1}\par\vspace{-.75em}}

% tighter spacing than itemize
\setlist[itemize]{align=parleft,left=0pt..1em}
\newenvironment{zitemize}{
\begin{itemize} \itemsep 0pt \parskip 0pt \parsep 1pt}
{\end{itemize}\vspace{-.5em}}


%-----------------------------------------------------------

\begin{document}
\begin{textblock*}{5cm}(14.6cm,1cm) % {block width} (coords) 
\raggedleft\textcolor{MidnightBlue}{ekyi@hawaii.edu}\\
www.linkedin.com/in/eintkyi
\end{textblock*}
\raggedright
\begin{textblock*}{5cm}(2cm,1cm) % {block width} (coords) 
\textcolor{MidnightBlue}{440-935-5123}\\
   Albuquerque, NM
\end{textblock*}
\begin{textblock*}{10cm}(9.7cm,1cm) % {block width} (coords) 
\huge
\textbf{Eint Kyi}\\

\end{textblock*}
\begin{textblock*}{20cm}(9.8cm,1.8cm) % {block width}
\large
\textcolor{MidnightBlue}{Data Analyst}
\end{textblock*}
\noindent
{\color{MidnightBlue} \rule{\linewidth}{0.7mm} }
\vspace{-0.6cm}


\section{SKILLS}
\begin{description}
\item[Languages]
R, Python, SQL
\vspace{-0.3cm}
\item[Tools \& Frameworks] 
NumPy, Pandas
\vspace{-0.3cm}
\item[Technical Skills] Data Wrangling, Data Extraction/Manipulation, Data Visualization, Exploratory Data Analysis
\vspace{-0.3cm}
\item[Technologies]  LaTeX, PowerBI, IBM Cognos \& Maximo Softwares, JasperSoft, Power Automate
\vspace{-0.15cm}
\end{description}

\section{Work Experience}
\begin{itemize}
\item
    \ressubheading{Water Utility Authority (ABCWUA)}{Albuquerque, NM}{Data Analyst}{November 2022 - Present}
    \begin{itemize}
        \resitem{Maintained the Laboratory Management Information System (LIMS) application and database}
        \resitem{Led meetings with IT team on automating instruments' data onto the LIMS system}
        \resitem{Analyzed water quality data using statistical techniques and make recommendations to program managers based on current regulations, policies, and quality control}
        \resitem{Collected and organized laboratory data for customers, consultants, and external governmental agencies using IBM’s Cognos Business Information Software, IBM's Maximo Software, PowerBI, Jaspersoft Studio, Microsoft Power Automate, Python, Microsoft SQL Server, and R}
   \end{itemize}
\item
	\ressubheading{Spectra Analytical Lab}{Honolulu, HI}{Quality Manager}{July 2018 - October 2022}
	\begin{itemize}
		\resitem{Successfully executed residual solvent validation studies for Hawai'i Department of Health (HDOH) certification in 4 different matrices (topicals, edibles, concentrates and tinctures)}
		\resitem{Actively involved in policy decisions of Hawai'i cannabis laws \& regulations}
		\resitem{Managed annual maintenance of ISO 17025 certification for over 2 years}
	    \resitem{Managed 5 employees on daily laboratory maintenance and work-flow}
		\resitem{Managed quality assurance and control of lab instruments and samples processed under ISO 17025 compliance}
	\end{itemize}
\end{itemize}

\section{Projects}
\begin{itemize}
\item
    \ressubheading{University of Hawaii at Manoa}{Honolulu, HI}{Bioinformatics}{August 2015- May 2018}
    \begin{itemize}
        \resitem{Investigated microbial activity and diversity associated with sinking particles at Station ALOHA by analyzing DNA extracts of 16S rRNA gene using DADA2 v1.14 and SILVA v138 database}
        \resitem{Statistical analyses of the sequences were performed using R packages: vegan, DECIPHER, phangorn and phyloseq to determine diversity, richness and evenness}
    \end{itemize}
\end{itemize}

\section{Education}
\begin{itemize}
\item
    \ressubheading{University of Hawaii at Manoa}{Honolulu, HI}{Masters in Oceanography}{May 2018}
\item
    \ressubheading{Oberlin College}{Oberlin, OH}{Bachelors in Biochemistry \& Geology}{May 2015}
\end{itemize}

\section{Published Papers}
\begin{itemize}
\item
	{Church, M.J., Kyi, E., Hall, R.O., Karl, D.M., Lindh, M., Nelson, A., and E.K. Wear. 2021. Production and diversity of microorganisms associated with sinking particles in the subtropical North Pacific Ocean. Limnology and Oceanography 66: 3255-3270. https://doi.org/10.1002/lno.11877}
\end{itemize}


\end{document}


