---
title: "Nifti Format"
teaching: 10
exercises: 0
questions:
- "Consectetur adipiscing elit"
objectives:
- "First learning objective. (FIXME)"
keypoints:
- "First key point. Brief Answer to questions. (FIXME)"
---

## Format / Extension 

* Typically assocated with .nii, .hdr/.img pair
* Probably one of the most popular format

You can read more about the technical details of [Nifti-1](https://brainder.org/2012/09/23/the-nifti-file-format/) format and its contrast with [NIFI-2](https://brainder.org/2015/04/03/the-nifti-2-file-format/). 

It is typically used to store 3D volumetric data. It can store [4D volumetric data] as well but outside of SPM/FSLEye and a few others, 4D data visualization can be more cumbersome.  
 

## Visualize NII format:

### SPM 3D Data Visualization


See relevant chapter at [SPM12 menu](https://www.fil.ion.ucl.ac.uk/spm/doc/spm12_manual.pdf) 

* Display Image Function Module (Chapter 17)

   * Fairly straight forward to use, click on the display button and then choose the image file to display and now you get an interactive way to explore the 3D data.  

* Registry Function (Chapter 18)
   * Mainly used to compare images to check for image alignments    
   * A hidden jewel within the Registry function is its ability to visualize 4D data as animation.
   * ![](https://www.researchgate.net/profile/Tamoor_Malik3/post/Failed_Model_Estimation---There_is_no_significant_Voxels/attachment/5d48d12bcfe4a7968dbd433c/AS%3A788704553607168%401565053227507/image/11.png)
 
* Results View
   * More in the statical module. 
   * Keep in mind without a .SPM file, T map nii files and etc by themselves means very little. Also, multiple comparison corrects etc. 
   *  ![](https://neuroimage.usc.edu/forums/uploads/default/original/1X/0fe415c1a23d05f2e39186f3d1b083c89f467dc0.jpg)

{% include links.md %}

### MRIcron/N/GL  

* All these software are quite closely related. 
* Use File -> Open to load the image you want.  
* MRICon
   * Notice MRICon has a LOT more tools to play with?
   * ![](https://people.cas.sc.edu/rorden/mricro/mricro1.gif)
* MRICron
   * Great user interface improvement. Much greater ease of use. 
   * ![](https://images.idoimaging.com/images/83/mricron_1.jpg)
* MRICronGL
   * Glossy rendering. 
   * ![](https://i0.wp.com/www.linuxlinks.com/wp-content/uploads/2019/03/MRIcroGL.jpg?fit=700%2C399&ssl=1)

### FSL Eye: 
* One of its most powerful feature is the ability to actually visualize 4D data as a interactive 3D movie sets of images. 
* It also has one of the most polish software to control overlay/layers (probably one of the best, short of Slicer3D)
* Detailed instruction at [FSL tutorial on FSLEye](https://fsl.fmrib.ox.ac.uk/fslcourse/lectures/practicals/intro1/index.html). ![](https://www.fmrib.ox.ac.uk/primers/intro_primer/ExBox7/TBSS_stats.png)


### Slicer 3D: 
* Probably one of the most powerful GUI based app you can find. It provides a very powerful manual segmentation interface as well 
* Best place to start: https://www.slicer.org/wiki/New_users#Main_Application_GUI
