---
layout: post
title:  "Skills: Bioinformatics vs Datascience"
date:   2022-02-09 18:45:00 -0000
categories: bioinformatics datascience job skills programming
---

Noticing several overlaps between bioinformatics and data science skill, I decided to visualize the similarities and differences. I randomly selected and compared 20 job postings on LinkedIn for each of them. I have limited my analysis to just the software skills required, including programming languages, frameworks, databases, etc. Comparing other skills would result in an unfair comparison since bioinformatics jobs often require specialized biological knowledge. Since it was random, the only filter I applied during selection was that the job title should reflect an entry or mid-level position, with hands-on work and not managerial roles.

This is how the plot looks!
![Bioinfo datascience tools comparison](/assets/images/combined_job_skills_counts.svg "Bioinformatics vs Datascience skills")

## Analysis
Summarizing few things that stand out or are surprising.

1. **The universality of Python:** Reqired in nearly all bioinformatics and data science jobs.
2. **R is important in bioinformatics:** Only 50% of the data science jobs require R. Also a reflection on R's academic origins and use.
3. **Low SQL and ML usage in bioinformatics:** This was a bit surprising because I know that almost all trained bioinformaticians learn it. Similarly not much machine learning is used in bioinformatics in general despite the recent successes in [structure prediction](https://www.nature.com/articles/s41586-021-03819-2)!
4. **Data science and the could:** Cloud technologies seem to be more important for data science jobs, with AWS and Spark being in high demand.
5. **Data scientists use commercial software:** Comparatively, bioinformaticians use more free software. I really don't know why, but it could be because of low commercial adoption of open-source tools.
6. **Bioinformatics requires more skills:** The variety of companies offering data science jobs is much higher than those offering bioinformatics jobs. Yet the number of skills required in bioinformatics is higher. This is mostly because of the requirement for specific tools or workflow management systems like Samtools and Snakemake.
7. **35 – 40% overlap in skills:** Other than the core of Python, R, and SQL, there are many non-overlapping skills required for either group.


## So?
So there are two take-home messages.

1. **To get into data science, you need to know Python and SQL! If you can combine it with AWS or Spark skills, you have a better chance of landing a job.**
2. **To be a bioinformatician, you need to know Python and R, along with knowledge of some other tools like Git, and also genome analysis tools like BWA.**

## Data
Data and code for this analysis can be found [here](https://github.com/gogothegreen/bioinfor_datsci_job_stats_analysis).