---
title: "Digital Imaging and Communications in Medicine (DICOM)"

teaching: 10

exercises: 0

questions:
- "What is a DICOM file?"
- "What can you do with DICOM files?"
- "What are the limitation of DICOM file?"

objectives:
- "Be able to identify DICOM files"

keypoints:
- "First key point. Brief Answer to questions. (FIXME)"
---

## Overview: 
DICOM file format was initially designed to facilitate medical diagnostic imaging information exchange between modalities. It is prefixed with a header and has numerous text fields (tags) to describe its properties. The tags typically exist in the format of ```(XXXX, XXXX)```. You can easily find a full lilst of all commonly used tags at: <https://www.dicomlibrary.com/dicom/dicom-tags/>
 
## Some Import Notes:

* Each DICOM files have **sets of tags in its header**. Therefore, adjacent 2D slides in a 3D volumes can have most tags duplicated almost.
* Individual DICOM files represent **a single 2D matrix "slice"** ((3002,0011)	DS	Image Plane Pixel Spacing) with a predefined "thickness" ((0018,0050)	DS	Slice Thickness and (0018,0088)	DS	Spacing Between Slices). The DICOM tags respectively determine both the real world dimension of the DICOM files, as well as the thickness.   
* ```StudyUID```, ```SeriesUID``` and other UID fields are a globally unique 128 bits [**Universally Unique Identifier**](https://en.wikipedia.org/wiki/Universally_unique_identifier) fields. They are commonly 
* DICOM format is **not determined by its file extension**. In fact, depending on modalities, some DICOM files may not even have file extensions. 
 
## How to work with DICOM files. 

Typically work flow involving DICOM files invovle two streams: 

1. You can visualize and inspect the DICOM files by directly open and accessing it.
This is most useful to either obtain tag related information (which are commonly shared with other slices from the same acquisition series)

1. You can convert (usually a stack of) DICOMs to 3D or 4D volumetric data format to other more native neuroimaging format for subsequent analyses. In this stream, DICOM is merely a transitory format. 


### Visualization of DICOM format

There are many effective and simple tools to directly visualize DICOM data, mostly targetted towards clinicians. They serve as a great first step towards quality control process. 

Example apps are: [RadiAnt(Windows only)](https://www.radiantviewer.com/), [Imaios web app](https://www.imaios.com/en/Imaios-Dicom-Viewer), [MicroDICOM](http://www.microdicom.com/). 

### Conversion of DICOM format 

To Nii Format: 

* SPM conversion: Under SPM batch manager -> Util -> DICOM Import: https://en.wikibooks.org/wiki/SPM/DICOM

* MRIcro/N/GL include [dcm2nii]=(https://people.cas.sc.edu/rorden/mricron/dcm2nii.html) or [dcm2niiN](http://www.mccauslandcenter.sc.edu/mricro/mricron/dcm2nii.html) which contain files:  

To MINC Format

* dcm2mnc converter would be necessary to convert the DICOM format to MINC format to conduct further analyses. 
  
## How to identify DICOM files: 

The only sure way to identify a DICOM file is by checking its header. 

This typically involves a DICOMHeader inspector. 

A few good examples are:

* DCMTK, DICOM dump utility, as part of the well known offis DICOM toolkit available across all platforms <https://support.dcmtk.org/docs/dcmdump.html>
* DICOMBrowser on Windows: <https://www.nitrc.org/projects/dicom_browser/>* 


{% include links.md %}
