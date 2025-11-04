# GPT vs human legal texts annotations: A comparative study with privacy policies

This repository provides all the files and elements required for experiments reproducibility of the research project: "GPT vs human legal texts annotations: A comparative study with privacy policies".

This research is part of the project "PRIVIA: Identificación Automatizada de Brechas de Privacidad en Ecuador usando Inteligencia Artificial Generativa y LLMs" conducted by Escuela Politécnica Nacional.

## Research information

- **Main project:** "PRIVIA: Identificación Automatizada de Brechas de Privacidad en Ecuador usando Inteligencia Artificial Generativa y LLMs" conducted by Escuela Politécnica Nacional.
- **Main project reference:** PIGR-24-06.
- **Date:** 2025-10-17.

## How to use this repository?

The repository contains 3 folders with a set of files that detail the results of the research. For experiments reproducibility, just open the file and execute it.

### Folder AnnotationMethod

This folder contains all the files for reproducing our proposed annotation method using GPT. The files are the following:

- SegmentsAnnotations.ipynb: This file contains the Python code to connect to the Chat Completions API and annotate all the segments of the 115 privacy policies of the OPP-115 corpus (segment-level annotation).
- WholeTextAnnotations.ipynb: This file contains the Python code to connect to the Chat Completions API and annotate all the 115 privacy policies of the OPP-115 corpus (full-text annotation).

Do not forget to set your OpenAI's API key before running the code.

### Folder Analysis

This folder contains the code to compare GPT-4o performance with human annotators. The files are the following:

- Analysis.ipynb: This file obtains the F1-score distributions of humans annotators and GPT-4o considering the ten categories of privacy policies.
- Analysis_061.ipynb: This file obtains the F1-score distributions of humans annotators and GPT-4o considering the categories of privacy policies with Fleiss' Kappa values greater than 0.61.
- Analysis_075:ipynb: This file obtains the F1-score distributions of humans annotators and GPT-4o considering the categories of privacy policies with Fleiss' Kappa values greater than 0.75.


### Folder Statistics

This folder contains the R files with the statistical analysis of the research. The files are the following:

- Statistics_segmentsLevel.Rmd: Statistics for segment-level annotations performed by humans and GPT-4o considering the ten categories of privacy policies.
- Statistics_segmentsLevel_061.Rmd: Statistics for segment-level annotations performed by humans and GPT-4o considering the categories of privacy policies with Fleiss' Kappa values greater than 0.61.
- Statistics_segmentsLevel_075.Rmd: Statistics for segment-level annotations performed by humans and GPT-4o considering the categories of privacy policies with Fleiss' Kappa values greater than 0.75.
- Statistics_wholeTextLevel.Rmd: Statistics for full-text level annotations performed by humans and GPT-4o considering the ten categories of privacy policies.
- Statistics_wholeTextLevel_061.Rmd: Statistics for full-text level annotations performed by humans and  GPT-4o considering the categories of privacy policies with Fleiss' Kappa values greater than 0.61.
- Statistics_wholeTextLevel_075.Rmd: Statistics for full-text level annotations performed by humans and  GPT-4o considering the categories of privacy policies with Fleiss' Kappa values greater than 0.75.

The R files use the results obtained through the files of the Analysis folder. For convenience, we replicate these results in the following folders:

- results: GPT-4o and humans' F1-score distributions for the ten categories of privacy practices (resulting files from Analysis.ipynb).
- results061: GPT-4o and humans' F1-score distributions for the categories of privacy practices with Fleiss' Kappa values greater than 0.61 (resulting files from Analysis_061 ipynb).
- results075: GPT-4o and humans' F1-score distributions for the categories of privacy practices with Fleiss' Kappa values greater than 0.75 (resulting files from Analysis_075 ipynb).
