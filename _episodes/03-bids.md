---
title: "Brain Imaging Data Structure (BIDS)"
teaching: 10
exercises: 0

questions:
- "What is BIDS?"
- "Why BIDS exist?"
- "How to use BIDS format?"

objectives:
- "Understand "

keypoints:
- ""
---

## Brain Imaging Data Structure

BIDS is really a meta organization architecture of organizing NII files along with useful meta data surrounding an imaging study. A good place to start is the official here: https://bids.neuroimaging.io/

## Why?

BIDS is needed because NII format by itself contain insufficient information about the project, group design, architecture.  


## How 
All BIDS compliant software are listed at: http://bids-apps.neuroimaging.io/apps/

To convert from DICOM files to BIDS, a solid list of software are indicated at the bottom of the dcm2niix page:
https://github.com/rordenlab/dcm2niix

Namely,[Bidsify](https://github.com/spinoza-rec/bidsify), [BIDSKit](https://github.com/jmtyszka/bidskit), [DAC2BIDS](https://github.com/dangom/dac2bids), [DCM2BIDS](https://github.com/cbedetti/Dcm2Bids), [HEUDICONV](https://github.com/nipy/heudiconv)

There currently do not exist any super polished commercial solution to convert to BIDS. 


> In the end, BIDS datasets are still grounded in basic format of NII, but organized in specific folder structures with the proper meta information stored and organized. In short, you still need software to open NII format.
{: .callout} 


{% include links.md %}
