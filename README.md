# beamer-theme-uha

Beamer theme UHA is a modern Beamer suitable for the staff of the University of Haute Alsace. the core designed has been inspered by the metropolis theme. An LaTeX source example and the related PDF document are provided in the repository.

## Installation
The installation of this theme involves four easy steps :
1. **Download the source** with a git clone of the beamer-theme-uha repository or as a zip archive.
2. **Move .sty files and the logo directory** to the folder containing your presentation. 
3. **Use the theme** by declaring `\usetheme{uha}` in the preamble of your Beamer document. 
4. **For best results** set the font size at *9pt*.


## Usage 

The following code shows a minimal example of a Beamer presentation using the beamer-theme-uha.
``` latex
\documentclass[8pt]{beamer}

\usetheme{uha}

\title{Titre de la présentation}
\subtitle{Sous-titre}
\date{Date d'aujourd'hui}
\author{Auteur de la présentation}
\institute{Université de Haute Alsace}

\begin{document}

\begin{frame}[plain, noframenumbering]
	\titlepage
\end{frame}

\section{Introduction}

\begin{frame}[fragile]{beamer UHA}
	
	Le thème beamer uha s'inspire du thème Metropolis qui lui même s'inspire du thème HSRM de Benjamin Weiss.

	Le thème se charge de la manière suivante :

	\begin{verbatim}
	\documentclass[9pt]{beamer}
	\usetheme{uha}
	\end{verbatim}
\end{frame}

\begin{frame}[fragile]{Section}
	Chaque section permet de regrouper des diapositives d'un même sujet.
	\begin{verbatim}
	\section{Les éléments}
	\end{verbatim}
\end{frame}

\section{Les éléments}

\begin{frame}[fragile]{Typographie}
	\begin{verbatim}
	Le thème uha permet de mettre en \emph{valeur du texte}, 
	de mettre en \textbf{gras du texte} et même 
	\alert{d'alerter le lecteur}.
	\end{verbatim}
	Le thème uha permet de mettre en \emph{valeur du texte}, de mettre en \textbf{gras du texte} et même \alert{d'alerter le lecteur}.
\end{frame}

\begin{frame}{Les listes}
	Une liste
	\begin{itemize}
		\item Premier
		\item Second
		\item Troisième
	\end{itemize}

	Une énumération
	\begin{enumerate}
		\item Premier
		\item Second
		\item Troisième
	\end{enumerate}

	Une description
	\begin{description}
		\item [UHA] Université de Haute Alsace
	\end{description}
\end{frame}

\begin{frame}{Les blocks}
	\begin{exampleblock}{Exemple}
		Un exemple
	\end{exampleblock}
	\begin{alertblock}{Exemple}
		Une alerte
	\end{alertblock}
	\begin{block}{Exemple}
		Un block
	\end{block}
\end{frame}

\end{document}

```


