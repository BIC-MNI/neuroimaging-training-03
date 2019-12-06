---
title: "Introduction"
teaching: 10
exercises: 0
questions:
- "Why look at your data?"
- "When to look at your data?"
- "What to look for in your data?"
- "How to look at your data?"
objectives:
- "Understand the importance of visualization"
- "Know why, when, what and how to look at your data"
keypoints:
- "Garbage in, Garbage Out"
- "After major processing steps, especially spatial manipulation"
- "Motion artefacts, signal dropout, distortion, more motion" 
- "Open data and notice any abnormal patterns."
---

# Data visualization


## Why? 

### Because of GIGO...
> GIGO: Garbage in garbage out. 
> - George Fueschsel, IBM Programmer and Instructor
{: .callout}

Neuroimaging data science is about processing data: localisation (data discovery), accession (local or remote, permissions), cleaning (artifact removal), and transformation before putting them through an analysis pipeline. If at any step the data are bad, your entire analysis can be meaningless and misguided at best, and at worst lead to the wrong conclusions. Visualising your data helps detect potential sources of problem and 
It is one of the most important steps before any kind of data analysis but it is also one of, if not the most commonly ignored.
Quality check of data is fundamental, and this applies across all neuroimaging modalities (e.g. different imaging acquisitions such as structural and functional neuroimaging), and all analysis types (e.g. univariate / multivariate statistics, connectivity analysis). 

> Fig 
> Source: "Echo time dependence of BOLD fMRI studies of the piriform cortex" https://www.ncbi.nlm.nih.gov/pubmed/19936572
> Just imagine what you can do with awesome orbitofrontal cortex fMRI data like these when... there are massive holes in your data. I am sure the group comparisons would look nice.  /s
{: .challenge}

### Because it will help you create figures.

The other solution for a less intuitive representation would be to create a table. 
Ever tried to make figures but not sure how to start? Familiarity with these tools will help you get nice figures, QUICKER, EASIER, and less painful.
 
### Because it will help with your analyses, regardless of the type of data. 

* functional MRI: task or resting state 
* Structural MRI: T1, T2, PD, etc.
* Diffusion weighted MRI
* PET: metabolism, in vivo receptor
* M/EEG

{: . } 

{% include links.md %}

