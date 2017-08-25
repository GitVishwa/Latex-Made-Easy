LATEX BASIC INTRODUCTION
  A Document preparation system which can be used for technical or scientific documents forms of publishing.
 
SYNTAX

  \documentclass{article}             -------------> This document is an article  
  \usepackage{package Name}           -------------> Use the required package.
   \title{Technical paper Name}       -------------> Title of the article
   \author{Author Name}               -------------> Author Name
   \date{Written date}                -------------> Written Date
   \begin{document}		      -------------> Beginning of document
	
     Hi Latex Folks!		      -------------> Start Latext Content here.
	
  \end{document}		      -------------> End of document.

	Latex is mainly used for preparing technical papers or scientifi documents.But these papers or documents may
	involve equations, tables, graphs etc. So, let's consider one by one.
 	
  A) Equations: 
	The following syntax defines various equations to use in latex.
	
       		\documentclass{article}
	        \usepackage{amsmath}
	       	\begin{document}
	 	        \begin{align}
   			  f(x) &= x^2\\
		          (a+b)^2 &= a^2+2ab+b^2\\
			  F(x) &= \int^a_b \frac{1}{3}x^3\\
			  (x+y)^2 + \sin(x+y)^2+(x+\frac{\frac{A}{B}}{C}+y)^2
 		        \end{align}
             	\end{document}
     
	When you run the above syntax, you will get the following result.

   B) Tables:
	Some technical papers requires usage of tables.So, following is the syntax for table creation 

		\documentclass{article}
		 \begin{document}

		   \begin{table}[h]            
			\caption{Table Name}                                      %title of the table
			\centering					          %centering table	
			\begin{tabular}{c rr}			                  %creating three colums
			\hline\hline						  %inserting double-line
			Algorithms &\multicolumn{2}{c}{Time and space complexities} \\ [0.5ex]
			\hline                                                    %inserting single line
			Bubble Sort  & O(n^2)  & O(1)\\                           %Row Contents
			Selection Sort & O(n^2) & O(1)\\      
			Quick Sort & O(n\log{}n) & O(n\log{}n)\\
			Merge Sort & O(n\log{}n) & O(n)\\
		    \end{tabular}
		    \label{tab:hresult}
		\end{table}
		\end{document}
             
           The above code displays the following result in TexMaker.

    C) Graphs:
	  Syntax for usage of graphs inside the latex.

		\documentclass{article}
		\usepackage{graphicx}                                             %package to include the graph/image.
		 \begin{document}

	         \begin{figure}
		 \centering
                  \includegraphics[totalheight=8cm]{/home/vishwanath/Desktop/png/PNG-Gradient_hex.png}   %Path of the image 
		   \label{fig:verticalcell}
		\end{figure}
		\end{document}