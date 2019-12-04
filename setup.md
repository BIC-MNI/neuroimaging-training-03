---
layout: page
title: "Visualization Softare Setup"
---


## SPM visualizer setup: 

Source: https://neurometrika.org/CoursePreparation

All OS: 

Instructions for installing SPM:
1. Install MATLAB 7.4 (R2007a) or later.
1. Download and unpack the core SPM12 distribution
1. Do not install the SPM12 files in the MATLAB directory structure. Instead, put the SPM12 directory in a /applications folder if possible.
1. Start MATLAB
1. Add the SPM12 top-level directory to the beginning of the MATLAB search path. In doing so, use "Add Folder..." rather than "Add with Subfolder..."
1. Save the new MATLAB search path and close the window.
1. Type "spm" at the MATLAB prompt
1. The SPM12 top-level dialog box should appear on the screen.

Also check the helpful youtube video online below: 
[![IMAGE ALT TEXT HERE](https://i.ytimg.com/vi/sbDi_HU8__Y/maxresdefault.jpg)](https://www.youtube.com/watch?v=f4CIcLyNTSw)


## xjView toolbox for SPM: 

All OS: 

1. Download XJView from here: https://www.alivelearn.net/xjview/download/
2. Unizp the XJView by copying it to the ```toolbox``` subfolder for the ```SPM``` root folder such that the path is like ```/spm/toolbox/xjview```

## FSLeye visualizer: 

Check the official guide from the FSL https://fsl.fmrib.ox.ac.uk/fsl/fslwiki/FSLeyes. 

Basicly, you can install it as part of FSL or separately and independently. I recommend to install part of the FSLEyes. 

## MRICron, MRICronGL: 

Note that MRICro, MRICroN, MRICronGL are THREE separately distinct and only tangentially related software by the same author. 

MRICro is the oldest but had the most extensive functionalities: https://www.mccauslandcenter.sc.edu/crnl/mricro 
MRICroN is the most common version used, with substantially simplified user interface, however its pixel value extraction is buggy: https://www.nitrc.org/projects/mricron 
MRICronGL further reduced functionalities while produce excellent image rendering: https://www.nitrc.org/projects/mricrogl

All MRICro/N/GL do not require any dependencies and once the binaries are downloaded from the website sources, you can directly execute them run. 

## ITKSnap: 

ITK Snap offers very friendly installer packages as well as binaries across platform.  
http://www.itksnap.org/pmwiki/pmwiki.php?n=Downloads.SNAP3

## MNI Display: 

Look for 1.9.17: https://bic-mni.github.io/#v2-version-1917

Make sure it is V2 Minc Tool Kit and version 1.9.17. Ignore everything else. 
The .deb and .rpm files for each platform can be found there. 

For most linux, you can use either ```sudo dpkg –install PACKAGE.deb``` or ```sudo rpm –install PACKAGE.rpm``` respectively. Make sure to replace ```package``` with the respective filename. 
 
## 3D Slicer: 

You can download respective 3DSlicer installer from the official website, https://download.slicer.org

{% include links.md %}
