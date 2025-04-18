\documentclass{article}
\usepackage{amsmath, amssymb, hyperref}

\title{Interest Rate Modeling: Lognormal Spot Rate Models}
\author{
  Flavio Salvatore Boccia \\
  Ludovico Costa \\
  Alessandro Pigato \\
  Lorenzo Tolomelli
}
\date{}

\begin{document}

\maketitle

\section*{Overview}

This report presents a comprehensive study on lognormal spot rate models, with a particular focus on the \textbf{Black-Derman-Toy (BDT)} model and its extensions. It explores theoretical foundations, numerical methodologies, and empirical insights central to interest rate modeling.

\section*{Objectives}

\begin{itemize}
  \item Examine the properties and limitations of lognormal spot rate models.
  \item Develop a detailed calibration framework for the BDT model.
  \item Analyze the Zero Black-Derman-Toy (ZBDT) model in the context of Zero Interest Rate Policies (ZIRP).
  \item Investigate pricing challenges of Eurodollar futures under lognormal models.
  \item Present a correction approach based on the Sandmann-Sondermann methodology.
\end{itemize}

\section*{Contents}

\subsection*{Lognormal Spot Rate Models}
\begin{itemize}
  \item Importance in bond pricing.
  \item Properties and limitations of lognormal short-rate models.
  \item Discussion of related models: CIR, Hull-White, Dothan, and BDT.
\end{itemize}

\subsection*{The Black-Derman-Toy Model}
\begin{itemize}
  \item Mathematical formulation and discrete/continuous link.
  \item Calibration methodology via a binomial tree.
  \item Numerical results and implementation in Python.
\end{itemize}

\subsection*{The Zero Black-Derman-Toy Model}
\begin{itemize}
  \item Extension to ZIRP environments.
  \item Structural modifications and probabilistic framework.
  \item Calibration and empirical validation.
  \item Applications to bond and option pricing.
\end{itemize}

\subsection*{Pricing Eurodollar Futures}
\begin{itemize}
  \item Theoretical instability of lognormal models.
  \item Analytical insights into explosive accumulation factors.
  \item Arbitrage-free pricing issues.
  \item Correction by Sandmann and Sondermann.
\end{itemize}

\section*{Implementation}

This project includes Python implementations supporting:
\begin{itemize}
  \item Calibration of the BDT model using historical yield and volatility data.
  \item Pricing of zero-coupon bonds and interest rate derivatives.
  \item Simulation of short-rate dynamics under various assumptions.
  \item Application of the Sandmann-Sondermann correction for stable Eurodollar futures pricing.
\end{itemize}

\section*{Key Findings}

\begin{itemize}
  \item The BDT binomial short-rate tree was successfully calibrated to historical data.
  \item The ZBDT model effectively handles prolonged low interest rate periods.
  \item Lognormal models can lead to unstable Eurodollar futures pricing.
  \item The Sandmann-Sondermann correction ensures stability and finite accumulation factors.
\end{itemize}

\section*{Authors}

\begin{itemize}
  \item Flavio Salvatore Boccia
  \item Ludovico Costa
  \item Alessandro Pigato
  \item Lorenzo Tolomelli
\end{itemize}

\section*{References}

\begin{itemize}
  \item Black, F., Derman, E., \& Toy, W. (1990). \textit{A One-Factor Model of Interest Rates and Its Application to Treasury Bond Options}. The Journal of Fixed Income, 1(1), 2–8.
  \item Black, F., \& Karasinski, P. (1991). \textit{Bond and Option Pricing when Short Rates are Lognormal}. Financial Analysts Journal, 47(4), 52–59.
  \item Sandmann, K., \& Sondermann, D. (1993). \textit{Log-Normal Interest Rate Models: Stability and Methodology}. Mathematical Finance, 3(1), 1–15.
  \item Hogan, S., \& Weintraub, D. (1993). \textit{Singularity and Explosive Behaviour in the Black-Derman-Toy Model}. Journal of Financial Economics, 36(2), 123–140.
  \item Krzyżanowski, G., Mordecki, E., \& Sosa, A. (2020). \textit{Zero Black-Derman-Toy Interest Rate Model}. Risk Management, 22(4), 89–106.
  \item Hull, J. C. (2017). \textit{Options, Futures, and Other Derivatives} (10th ed.). Pearson. ISBN: 978-0134472089.
\end{itemize}

\end{document}
