---
title: "Statistical Maps"
teaching: 10
exercises: 0

questions:
- "What are statistical maps?"

objectives:
- "Understand what can be done at statistical maps?"

keypoints:
- "Statistical maps are different."

---
T/F/Z statistical maps are represented as a special version of NII/MINC format files. Instead of having voxels representing individual MRI signal intensities, the value of each voxel would represent the statical value from the test. 

These are best overlaid on the anatomical maps for spatial interpretation.

## Interpretation

Statistical maps should not be inspected without some kind of statical thresholding. They usually needs to be interpreted in the context applying proper thresholding and statistical correction.  

## Software:
- SPM: statistical/results module
- XJView: enhanced threshold view of statistical maps.


{% include links.md %}
