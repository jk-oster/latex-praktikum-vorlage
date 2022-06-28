# latex-praktikum-bsp

## LaTex Befehle
```latex
\include{folder/filename} % File einfügen (Kapitel in eigenem File)
\chapter{...} \label{cha:...} % Kapitel
\section{...} % Überschrift 1   
\subsection{...} % Überschrift 2 
\subsubsection{...} % Überschrift 3
\paragraph{...} % Absatz   
\texttt{...} % code   
\emph{...} % kurisv   
\textbf{...} % fett   
\label{key}  % Sprungmarken,   jedes Bild, Tabelle, Abschnitt
\ref{key} % Referenzieren / Verweisen   
\pageref{key} % Seite mit Sprungmarke Verweisen   
\footnote{...} % Fußnote   
\begin{itemize} \item ... \item ... \end{itemize} % Aufzählung Bullets   
\begin{enumerate} \item ... \item ... \end{enumerate} % Aufzählung Nummeriert   
\begin{center} ... \end{center} % Zentrierter Text   
\begin{JsCode} ... \end{JsCode} % JavaScript Code highlighten
\begin{algorithm} ... \end{algorithm} % Pseudo code
... $(a+b)$ ... % Mathematische Formeln inline
$$(a+b)$$ ... % Mathematische Formeln freigestellt
\begin{equation} \label{mat:...} ... \end{equation} % Referenzierbare Formel
~ % Geschütztes Leerzeichen
-- % Längerer Bindestrich   
--- % Englischer Gedankenstrich   
"..." % Anführungszeichen, wenn smartquotes eingeschaltet
\- % Überlänge von Wörtern z.B. bei Code      wird bei Bedarf hier geteilt   erst ganz zum Schluss
```

## Bilder
```latex
\begin{figure}[htbp] 
    \centering
    \includegraphics[width=.2\textwidth]{logo}
    \caption{Das ist eine Abbildung}
    \label{fig:pic1}
\end{figure}
% !h   Bild hier im Text erzwingen
% !b   Bild am Ende der Seite erzwingen
% !t   Bild am Anfang der Seite erzwingen
% htbp   Versuche Bild hier einzufügen, wenn nicht möglich am Anfang der Seite, wenn nicht möglich am Ende der Seite, wenn nicht möglich eigene Seite
```

% Bilder inline im Text
```latex
\begin{wrapfigure}{R}{0.5\textwidth}
    \centering
    \includegraphics[width=.4\textwidth]{logo}
    \caption{Das ist eine Abbildung}
    \label{fig:pic1}
\end{wrapfigure}
```

## Table
```latex
% Tabelle in Excel erstellen und als .pdf exportieren
\begin{table}
    \centering
    \caption{Das ist eine Tabelle}
    \includegraphics[width=.4\textwidth]{logo.pdf}
    \label{tab:tab1}
\end{table}
```

## Zitieren
```latex
% Bei fehlern immer BibTex kontrollieren
\cite{key} % Zitat hne klammer   
\parencite{key} % Ztat mit Klammer   
\parencite[Seite 3]{key} % Zitat mit Klammer und Seite   
\textcite{key} % Tetzitat (Jahr in klammer)   
\citeauthor{key} % ur Autor zitieren   
\citeyear{key} % Nur Jhr zitieren   
\begin{quote} "..." \citeauhtor{key} \end{quote} % hervorgehobenes Zitat
```
