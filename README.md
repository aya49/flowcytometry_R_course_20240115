# Flow cytometry analysis on R/bioconductor

This course is a 4 day x 4 hour course instructed by Alice Yue, hosted on Physalia: https://www.physalia-courses.org/courses-workshops/flow-cytometry/

- **Date and time**: 2024-01-15 - 2024-01-18 @ 16:00-18:00 CEST (7:00-11:00 PST) (11:00-3:00 BJT)
- **Instructor**: Alice Yue (Metafora-biosystems)
- **Level**: Beginner-Intermediate

**Overview**: Flow cytometry is a gold standard in the analysis of immune cells for clinical diagnosis and research. This course introduces what flow cytometry is and why we use it to analyze cell population composition in biological samples. We will learn about best practices for how to analyze flow cytometry data using R/Bioconductor. Said practices include: preprocessing of the data (compensation, transformation, and quality control), multi-dimensional cell population identification via clustering, and visualizing the results in 2D. These tools can be applied to all types of cytometry including flow, mass, and spectral.

**Target audience**: This course is created for anyone interested in analyzing biological samples with single-cell flow cytometry. Background in flow cytometry and R/Bioconductor is not necessary as we will go over a short introduction to them. However, experience with programming will help greatly.

## Learning outcomes

- Understand the flow cytometry machinery and its analytical purpose.
- Be able to set up the infrastructure for and write basic data analytic scripts in R.
- Describe and execute each step in the flow cytometry data analytics pipeline in R/Bioconductor.
- Be comfortable with interpreting and eliciting conclusions from the results of the flow cytometry data analytics pipeline.

## Pre-requisites

Before starting,

- Install [R](https://www.r-project.org/) and [Rstudio](https://www.rstudio.com/categories/rstudio-ide/): https://learnr-examples.shinyapps.io/ex-setup-r/
- Install required R packages using script: [02_packages](02_packages.R)

## Schedule

Support over Slack will be available throughout the course: http://physaliaflowcytometry.slack.com/

- Day 1
    - [01] [Background on flow cytometry](https://docs.google.com/presentation/d/1qkEWJLE6fFMY-fGJ1V7cxGwj2TlhV8ybRnwtupt3O7o/edit?usp=sharing): This session focuses on the purpose of flow cytometry, a brief overview of its machinery, and its data analysis pipeline.
    - Download [sangerP2.fcs](https://drive.google.com/file/d/1PpSM93GTj9zejVDZzD89_k3sx7Lc-TQl/view?usp=sharing), it will be used for sessions 4\&5| 
    - [01.2] [Beginner's guide to R](https://docs.google.com/presentation/d/1oPUWVpwM1-60sFgXknvmElf8yqwHsxnLGJIOeUEWtVs/edit?usp=sharing): Users will learn the basics of R and we will set up the computational infrastructure required for the next sessions. For those who do not have R, for this session, please use https://posit.cloud/.
    - **Scripts**: [01_intro_to_R.R](./01_intro_to_R.R), [02_packages.R](./02_packages.R)
- Day 2
    - [02] [Preprocessing flow cytometry data](https://docs.google.com/presentation/d/18mVxUs6g5fCtY68M-S_wVcV2qqm4dsp9yMjiaqLHOe0/edit?usp=sharing): We will learn about the theory behind preprocessing of flow cytometry samples.
    - **Scripts**: [03_preprocess.R](./03_preprocess.R), [03.1_more_intro_to_R_ifelse_loop_func_plot.R](./03.1_more_intro_to_R_ifelse_loop_func_plot.R), [03.2_intro_to_R_fileIO_loop.R](./03.2_intro_to_R_fileIO_loop.R) (example solution: [03.3_preprocess_loop.R](./03.3_preprocess_loop.R))
- Day 3
    - [04] [Cell population identification using 2D gating](https://docs.google.com/presentation/d/14UsDaiAsvemXUoEh5pP47G5NU8TVcMrGVS39grAP1X0/edit?usp=sharing): Participants will learn about how flow cytometrists traditionally identify cell populations in preprocessed samples using 2D gating. We will go over an example of an existing manual 2D gating from flowJo and how it is used to compare cell population abundances across samples.
    - **Scripts**: [04_gating.R](./04_gating.R) (example solution: [04_gating_full.R](./04_gating_full.R)), [05_gating_stats.R](./05_gating_stats.R), (optional: [04.5_intro_to_R_truefalse.R](./04.5_intro_to_R_truefalse.R))
- Day 4
    - [05] [Cell population identification using clustering](https://docs.google.com/presentation/d/1Hc1-azirEF6bsODBX_G3uehJ7hWcHmaAv68hUMtIn_Y/edit?usp=sharing): We will analyze the same samples using clustering in R and learn how to interpret the results.
    - **Scripts**: [06_gating_clustering.R](./06_gating_clustering.R), [07_clustering.R](./07_clustering.R)
