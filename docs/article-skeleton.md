---
title: "Article Template"
output:
  pdf_document: default
  word_document: default
  html_document:
    keep_md: true
geometry: margin= 1.0in
font-size: 11pt
header-includes: 
  - \usepackage{helvet}
  - \renewcommand*\familydefault{\sfdefault}
  - \usepackage{setspace}
  - \doublespacing
  - \usepackage[left]{lineno}
  - \linenumbers
  - \usepackage{colortbl}
editor_options: 
  chunk_output_type: console
knit: (function(input, ...) {
    rmarkdown::render(
      input,
      output_format = "html_document",
      output_dir = "docs"
    )
  })
---



# **Article Template** 

\vspace{10mm}

**Running Title:**

\vspace{10mm}

Author Name 1 ${^\dagger}$ , Author Name 2, ...

${\dagger}$ To whom correspondance should be addressed

\vspace{10mm}
 
Department of ...  
... University  
Address  

\vspace{10mm}

**Observation Format**

\newpage

## Abstract (... words)
Here goes an **Abstract** text.

## Importance (... words)
Here goes an **Importance** text.

* Importance I 
  * Importance-I-a
  * Importance-I-b
* Importance II
* Importance III

\newpage

## Introduction
Here goes an **Introduction** text.

\newpage

## Results
Here goes an **Results** text.

example results from {gtsummary} package named `trial`.

<table>
 <thead>
  <tr>
   <th style="text-align:left;"> trt </th>
   <th style="text-align:right;"> age </th>
   <th style="text-align:right;"> marker </th>
   <th style="text-align:left;"> stage </th>
   <th style="text-align:left;"> grade </th>
   <th style="text-align:right;"> response </th>
   <th style="text-align:right;"> death </th>
   <th style="text-align:right;"> ttdeath </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:left;"> Drug A </td>
   <td style="text-align:right;"> 23 </td>
   <td style="text-align:right;"> 0.160 </td>
   <td style="text-align:left;"> T1 </td>
   <td style="text-align:left;"> II </td>
   <td style="text-align:right;"> 0 </td>
   <td style="text-align:right;"> 0 </td>
   <td style="text-align:right;"> 24.00 </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Drug B </td>
   <td style="text-align:right;"> 9 </td>
   <td style="text-align:right;"> 1.107 </td>
   <td style="text-align:left;"> T2 </td>
   <td style="text-align:left;"> I </td>
   <td style="text-align:right;"> 1 </td>
   <td style="text-align:right;"> 0 </td>
   <td style="text-align:right;"> 24.00 </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Drug A </td>
   <td style="text-align:right;"> 31 </td>
   <td style="text-align:right;"> 0.277 </td>
   <td style="text-align:left;"> T1 </td>
   <td style="text-align:left;"> II </td>
   <td style="text-align:right;"> 0 </td>
   <td style="text-align:right;"> 0 </td>
   <td style="text-align:right;"> 24.00 </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Drug A </td>
   <td style="text-align:right;"> NA </td>
   <td style="text-align:right;"> 2.067 </td>
   <td style="text-align:left;"> T3 </td>
   <td style="text-align:left;"> III </td>
   <td style="text-align:right;"> 1 </td>
   <td style="text-align:right;"> 1 </td>
   <td style="text-align:right;"> 17.64 </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Drug A </td>
   <td style="text-align:right;"> 51 </td>
   <td style="text-align:right;"> 2.767 </td>
   <td style="text-align:left;"> T4 </td>
   <td style="text-align:left;"> III </td>
   <td style="text-align:right;"> 1 </td>
   <td style="text-align:right;"> 1 </td>
   <td style="text-align:right;"> 16.43 </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Drug B </td>
   <td style="text-align:right;"> 39 </td>
   <td style="text-align:right;"> 0.613 </td>
   <td style="text-align:left;"> T4 </td>
   <td style="text-align:left;"> I </td>
   <td style="text-align:right;"> 0 </td>
   <td style="text-align:right;"> 1 </td>
   <td style="text-align:right;"> 15.64 </td>
  </tr>
</tbody>
</table>


### Results-I
Here goes an **Results-I** text.

### Results-II
Here goes an **Results-II** text.

\newpage

## Conclusions
Here goes an **Conclusions** text.

* Conclusions-I
  * Conclusions-I-a
  * Conclusions-I-b
* Conclusions-II
* Conclusions-III

\newpage

## Materials & Methods
Here goes an **Materials & Methods** text.


\newpage

## Tables
Here  **Tables** text.

\vspace{2mm}
`table_1` using the {gtsummary} package

\setlength{\LTpost}{0mm}
\begin{longtable}{lccccc}
\toprule
 &  &  & \multicolumn{2}{c}{Treatment Received} &  \\ 
\cmidrule(lr){4-5}
Variable & \textbf{N} & \textbf{Overall}, N = 200\textsuperscript{1} & \textbf{Drug A}, N = 98\textsuperscript{1} & \textbf{Drug B}, N = 102\textsuperscript{1} & \textbf{p-value}\textsuperscript{2} \\ 
\midrule
Age & 189 & 47 (38, 57) & 46 (37, 59) & 48 (39, 56) & 0.72 \\ 
    Unknown &  & 11 & 7 & 4 &  \\ 
Grade & 200 &  &  &  & 0.87 \\ 
    I &  & 68 (34\%) & 35 (36\%) & 33 (32\%) &  \\ 
    II &  & 68 (34\%) & 32 (33\%) & 36 (35\%) &  \\ 
    III &  & 64 (32\%) & 31 (32\%) & 33 (32\%) &  \\ 
\bottomrule
\end{longtable}
\begin{minipage}{\linewidth}
\textsuperscript{1}Median (IQR) or Frequency (\%)\\
\textsuperscript{2}Wilcoxon rank sum test; Pearson\textquotesingle{}s Chi-squared test\\
\end{minipage}

**Table 1: with gtsummary package**

\newpage

`table_2` using the {gt} package

\vspace{2mm}

\begin{longtable}{lrc}
\caption*{
{\large \texttt{trial} Data from \{gtsummary\} package} \\ 
{\small \texttt{trial} is an \{gtsummary\} dataset}
} \\ 
\toprule
trt & age & grade \\ 
\midrule
Drug A & 23 & II \\ 
Drug B & 9 & I \\ 
Drug A & 31 & II \\ 
Drug A & NA & III \\ 
Drug A & 51 & III \\ 
\bottomrule
\end{longtable}

**Table 2: with {gt} package (needs manipulation in gt)**

\vspace{2mm}

\newpage

`table_3` using the {gtsummary} & {kableExtra} package 
{kableExtra} add caption of table within code give number of table by code.

\arrayrulecolor{white}

<table style="NAborder-bottom: 0; font-size: 10px; width: auto !important; margin-left: auto; margin-right: auto;" class="table">
<caption style="font-size: initial !important;">Table 3 with {gtsummary} and {kableExtra} packages</caption>
 <thead>
<tr>
<th style="empty-cells: hide;border-bottom:hidden;" colspan="3"></th>
<th style="border-bottom:hidden;padding-bottom:0; padding-left:3px;padding-right:3px;text-align: center; " colspan="2"><div style="border-bottom: 1px solid #ddd; padding-bottom: 5px; ">Treatment Received</div></th>
<th style="empty-cells: hide;border-bottom:hidden;" colspan="1"></th>
</tr>
  <tr>
   <th style="text-align:left;"> Variable </th>
   <th style="text-align:center;"> N </th>
   <th style="text-align:center;"> Overall, N = 200 </th>
   <th style="text-align:center;"> Drug A, N = 98 </th>
   <th style="text-align:center;"> Drug B, N = 102 </th>
   <th style="text-align:center;"> p-value </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:left;"> Age </td>
   <td style="text-align:center;"> 189 </td>
   <td style="text-align:center;"> 47 (38, 57) </td>
   <td style="text-align:center;"> 46 (37, 59) </td>
   <td style="text-align:center;"> 48 (39, 56) </td>
   <td style="text-align:center;"> 0.72 </td>
  </tr>
  <tr>
   <td style="text-align:left;padding-left: 2em;" indentlevel="1"> Unknown </td>
   <td style="text-align:center;">  </td>
   <td style="text-align:center;"> 11 </td>
   <td style="text-align:center;"> 7 </td>
   <td style="text-align:center;"> 4 </td>
   <td style="text-align:center;">  </td>
  </tr>
  <tr>
   <td style="text-align:left;"> Grade </td>
   <td style="text-align:center;"> 200 </td>
   <td style="text-align:center;">  </td>
   <td style="text-align:center;">  </td>
   <td style="text-align:center;">  </td>
   <td style="text-align:center;"> 0.87 </td>
  </tr>
  <tr>
   <td style="text-align:left;padding-left: 2em;" indentlevel="1"> I </td>
   <td style="text-align:center;">  </td>
   <td style="text-align:center;"> 68 (34%) </td>
   <td style="text-align:center;"> 35 (36%) </td>
   <td style="text-align:center;"> 33 (32%) </td>
   <td style="text-align:center;">  </td>
  </tr>
  <tr>
   <td style="text-align:left;padding-left: 2em;" indentlevel="1"> II </td>
   <td style="text-align:center;">  </td>
   <td style="text-align:center;"> 68 (34%) </td>
   <td style="text-align:center;"> 32 (33%) </td>
   <td style="text-align:center;"> 36 (35%) </td>
   <td style="text-align:center;">  </td>
  </tr>
  <tr>
   <td style="text-align:left;padding-left: 2em;" indentlevel="1"> III </td>
   <td style="text-align:center;">  </td>
   <td style="text-align:center;"> 64 (32%) </td>
   <td style="text-align:center;"> 31 (32%) </td>
   <td style="text-align:center;"> 33 (32%) </td>
   <td style="text-align:center;">  </td>
  </tr>
</tbody>
<tfoot>
<tr><td style="padding: 0; " colspan="100%">
<sup>1</sup> Median (IQR) or Frequency (%)</td></tr>
<tr><td style="padding: 0; " colspan="100%">
<sup>2</sup> Wilcoxon rank sum test; Pearson's Chi-squared test</td></tr>
</tfoot>
</table>

\vspace{2mm}

\newpage

`table_4` using the {gtsummary} & {kableExtra} package

\vspace{2mm}

<table style="NAborder-bottom: 0; font-size: 10px; width: auto !important; margin-left: auto; margin-right: auto;" class="table">
<caption style="font-size: initial !important;">**Patient Characteristics**</caption>
 <thead>
<tr>
<th style="empty-cells: hide;border-bottom:hidden;" colspan="3"></th>
<th style="border-bottom:hidden;padding-bottom:0; padding-left:3px;padding-right:3px;text-align: center; " colspan="2"><div style="border-bottom: 1px solid #ddd; padding-bottom: 5px; ">Treatment Received</div></th>
<th style="empty-cells: hide;border-bottom:hidden;" colspan="1"></th>
</tr>
  <tr>
   <th style="text-align:left;"> Variable </th>
   <th style="text-align:center;"> N </th>
   <th style="text-align:center;"> Overall, N = 200 </th>
   <th style="text-align:center;"> Drug A, N = 98 </th>
   <th style="text-align:center;"> Drug B, N = 102 </th>
   <th style="text-align:center;"> p-value </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:left;"> <span style=" font-weight: bold;    ">Age</span> </td>
   <td style="text-align:center;"> 189 </td>
   <td style="text-align:center;"> 47 (38, 57) </td>
   <td style="text-align:center;"> 46 (37, 59) </td>
   <td style="text-align:center;"> 48 (39, 56) </td>
   <td style="text-align:center;"> 0.72 </td>
  </tr>
  <tr>
   <td style="text-align:left;padding-left: 2em;" indentlevel="1"> Unknown </td>
   <td style="text-align:center;">  </td>
   <td style="text-align:center;"> 11 </td>
   <td style="text-align:center;"> 7 </td>
   <td style="text-align:center;"> 4 </td>
   <td style="text-align:center;">  </td>
  </tr>
  <tr>
   <td style="text-align:left;"> <span style=" font-weight: bold;    ">Grade</span> </td>
   <td style="text-align:center;"> 200 </td>
   <td style="text-align:center;">  </td>
   <td style="text-align:center;">  </td>
   <td style="text-align:center;">  </td>
   <td style="text-align:center;"> 0.87 </td>
  </tr>
  <tr>
   <td style="text-align:left;padding-left: 2em;" indentlevel="1"> I </td>
   <td style="text-align:center;">  </td>
   <td style="text-align:center;"> 68 (34%) </td>
   <td style="text-align:center;"> 35 (36%) </td>
   <td style="text-align:center;"> 33 (32%) </td>
   <td style="text-align:center;">  </td>
  </tr>
  <tr>
   <td style="text-align:left;padding-left: 2em;" indentlevel="1"> II </td>
   <td style="text-align:center;">  </td>
   <td style="text-align:center;"> 68 (34%) </td>
   <td style="text-align:center;"> 32 (33%) </td>
   <td style="text-align:center;"> 36 (35%) </td>
   <td style="text-align:center;">  </td>
  </tr>
  <tr>
   <td style="text-align:left;padding-left: 2em;" indentlevel="1"> III </td>
   <td style="text-align:center;">  </td>
   <td style="text-align:center;"> 64 (32%) </td>
   <td style="text-align:center;"> 31 (32%) </td>
   <td style="text-align:center;"> 33 (32%) </td>
   <td style="text-align:center;">  </td>
  </tr>
</tbody>
<tfoot>
<tr><td style="padding: 0; " colspan="100%">
<sup>1</sup> Median (IQR) or Frequency (%)</td></tr>
<tr><td style="padding: 0; " colspan="100%">
<sup>2</sup> Wilcoxon rank sum test; Pearson's Chi-squared test</td></tr>
</tfoot>
</table>

\newpage

## Figures

Here goes a **Figures** text.

\vspace{2mm}

\includegraphics{figures/trial_plot.pdf}

**Figure 1. trial plot with ggplot2**

\newpage



![Sample figure for trial data with ggplot2](figures/trial_plot.pdf)

\newpage

## Acknowledgements
Here goes an **Acknowledgements** text.

\newpage

## References

