---
title:  "Data-driven Structural Priors for Shape Completion"

author: <a href="http://mhsung.github.io/" target="_blank">Minhyuk Sung</a>, <a href="http://www.vovakim.com/" target="_blank">Vladimir G. Kim</a>, <a href="http://rangst.github.io" target="_blank">Roland Angst</a>, and <a href="http://geometry.stanford.edu/member/guibas/" target="_blank">Leonidas Guibas</a>

journal: SIGGRAPH Asia 2015

slug: structure-completion

date: 2015-09-18

code-link: https://github.com/mhsung/structure-completion
---

## {{ page.title }}
{:.title}
#### {{ page.author }}
{:.title}
#### {{ page.journal }}
{:.title}

<br />
![]({{site.baseurl}}/assets/images/{{page.slug}}/teaser.png)

### Abstract
>Acquiring 3D geometry of an object is a tedious and time-consuming task, typically requiring scanning the surface from multiple viewpoints.  In this work we focus on reconstructing complete geometry from a single scan acquired with a low-quality consumer-level scanning device.  Our method uses a collection of example 3D shapes to build structural part-based priors that are necessary to complete the shape. In our representation, we associate a local coordinate system to each part and learn the distribution of positions and orientations of all the other parts from the database, which implicitly also defines positions of symmetry planes and symmetry axes. At the inference stage, this knowledge enables us to analyze incomplete point clouds with substantial occlusions, because observing only a few regions is still sufficient to infer the global structure. Once the parts and the symmetries are estimated, both data sources, symmetry and database, are fused to complete the point cloud. We evaluate our technique on a synthetic dataset containing 481 shapes, and on real scans acquired with a Kinect scanner. Our method demonstrates high accuracy for the estimated part structure and detected symmetries, enabling higher quality shape completions in comparison to alternative techniques.
<br />

*{{page.author}}<br>
**{{page.title}}**<br>
{{page.journal}}*<br>
[Paper]({{site.baseurl}}/assets/files/{{page.slug}}.pdf){:target="_blank"}  | 
[Supplementary material]({{site.baseurl}}/assets/files/{{page.slug}}-supplementary.pdf){:target="_blank"}  | 
[Slides(PPTX)]({{site.baseurl}}/assets/files/{{page.slug}}-slides.pptx){:target="_blank"}  | 
[Code]({{page.code-link}}){:target="_blank"}

### Bibtex
```
@article{Sung:2015,
  author = {Sung, Minhyuk and Kim, Vladimir G. and Angst, Roland and Guibas, Leonidas},
  title = {Data-driven Structural Priors for Shape Completion},
  Journal = {ACM Transactions on Graphics (Proc. of SIGGRAPH Asia)}, 
  year = {2015}
}
```

### Data Download
[Ground truth datasets (41.8MB)](https://shapenet.cs.stanford.edu/media/minhyuk/structure-completion/ground_truth_datasets.tgz)<br>
[Benchmark results (2.2GB)](https://shapenet.cs.stanford.edu/media/minhyuk/structure-completion/benchmark_results.tgz)<br>
[Kinect scan data (27.7MB)](https://shapenet.cs.stanford.edu/media/minhyuk/structure-completion/kinect_scan_data.tgz)

### Benchmark Results
On the following linked webpages, we present several experimental results organized as tables, where each row corresponds to a model.
The columns are as follows:

| Column Name  | Content |
|:------------ |:------- |
| View         |The image viewed from the scanner. |
| Input        |The acquired point cloud from a canonical view. |
| Structure    | Estimated structure (using our method, [Shen et al. 2012], or [Podolak 2006]) |
| Accuracy     | Completed shape where each point is colored according to the distance to the ground truth surface. Non-blue points indicate errors in completed point cloud. |
| Completeness | True shape where each point is colored according to the distance to the completed shape. Non-blue points indicate that occluded points were not added. |

<br />
We present results on the following datasets:

<table>
<thead>
<tr>
<th align="left">Dataset</th>
<th align="center">Ours</th>
<th align="center">Shen et al. 2012</th>
<th align="center">Podolak et al. 2006</th>
<th align="center">Plot (Fig. 11 in paper)</th>
</tr>
</thead>

<tbody>
<tr>
<td align="left">Chairs (Shen et al.)</td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/final3_assembly_chairs/index.html" target="_blank">Ours</a></td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/assembly_final3_assembly_chairs/index.html" target="_blank">Shen et al.</a></td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/symm_detection_final3_assembly_chairs/index.html" target="_blank">Podolak et al.</a></td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/box_plots/box_assembly_chair.png" target="_blank">Plot</a></td>
</tr>

<tr>
<td align="left">Airplanes (Shen et al.)</td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/final3_assembly_airplanes/index.html" target="_blank">Ours</a></td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/assembly_final3_assembly_airplanes/index.html" target="_blank">Shen et al.</a></td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/symm_detection_final3_assembly_airplanes/index.html" target="_blank">Podolak et al.</a></td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/box_plots/box_assembly_airplane.png" target="_blank">Plot</a></td>
</tr>

<tr>
<td align="left">Bicycles (Shen et al.)</td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/final3_assembly_bicycles/index.html" target="_blank">Ours</a></td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/assembly_final3_assembly_bicycles/index.html" target="_blank">Shen et al.</a></td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/symm_detection_final3_assembly_bicycles/index.html" target="_blank">Podolak et al.</a></td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/box_plots/box_assembly_bicycle.png" target="_blank">Plot</a></td>
</tr>

<tr>
<td align="left">Chairs (COSEG)</td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/final3_coseg_chairs/index.html" target="_blank">Ours</a></td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/assembly_final3_coseg_chairs/index.html" target="_blank">Shen et al.</a></td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/symm_detection_final3_coseg_chairs/index.html" target="_blank">Podolak et al.</a></td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/box_plots/box_coseg_chair.png" target="_blank">Plot</a></td>
</tr>

<tr>
<td align="left">Tables (ShapeNet)</td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/final3_shapenet_tables/index.html" target="_blank">Ours</a></td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/assembly_final3_shapenet_tables/index.html" target="_blank">Shen et al.</a></td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/symm_detection_final3_shapenet_tables/index.html" target="_blank">Podolak et al.</a></td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/box_plots/box_shapenet_table.png" target="_blank">Plot</a></td>
</tr>
</tbody>

</table>


<br />
We also present results in the presence of stronger occlusions simulated by a rectangle between the surface and the viewpoint (Fig. 12 in paper):

<table>
<thead>
<tr>
<th align="left">Dataset</th>
<th align="center">Ours</th>
<th align="center">Shen et al. 2012</th>
<th align="center">Podolak et al. 2006</th>
<th align="center">Plot (Fig. 12 in paper)</th>
</tr>
</thead>

<tbody>
<tr><td align="left">Chairs (Shen et al.)</td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/view_mask_assembly_chairs/index.html" target="_blank">Ours</a></td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/assembly_view_mask_assembly_chairs/index.html" target="_blank">Shen et al.</a></td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/symm_detection_view_mask_assembly_chairs/index.html" target="_blank">Podolak et al.</a></td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/box_plots/view_mask_box_assembly_chair.png" target="_blank">Plot</a></td>
</tr>

<tr>
<td align="left">Airplanes (Shen et al.)</td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/view_mask_assembly_airplanes/index.html" target="_blank">Ours</a></td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/assembly_view_mask_assembly_airplanes/index.html" target="_blank">Shen et al.</a></td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/symm_detection_view_mask_assembly_airplanes/index.html" target="_blank">Podolak et al.</a></td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/box_plots/view_mask_box_assembly_airplane.png" target="_blank">Plot</a></td>
</tr>

<tr>
<td align="left">Bicycles (Shen et al.)</td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/view_mask_assembly_bicycles/index.html" target="_blank">Ours</a></td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/assembly_view_mask_assembly_bicycles/index.html" target="_blank">Shen et al.</a></td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/symm_detection_view_mask_assembly_bicycles/index.html" target="_blank">Podolak et al.</a></td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/box_plots/view_mask_box_assembly_bicycle.png" target="_blank">Plot</a></td>
</tr>

<tr>
<td align="left">Chairs (COSEG)</td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/view_mask_coseg_chairs/index.html" target="_blank">Ours</a></td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/assembly_view_mask_coseg_chairs/index.html" target="_blank">Shen et al.</a></td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/symm_detection_view_mask_coseg_chairs/index.html" target="_blank">Podolak et al.</a></td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/box_plots/view_mask_box_coseg_chair.png" target="_blank">Plot</a></td>
</tr>

<tr>
<td align="left">Tables (ShapeNet)</td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/view_mask_shapenet_tables/index.html" target="_blank">Ours</a></td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/assembly_view_mask_shapenet_tables/index.html" target="_blank">Shen et al.</a></td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/symm_detection_view_mask_shapenet_tables/index.html" target="_blank">Podolak et al.</a></td>
<td align="center"><a href="http://web.stanford.edu/~mhsung/structure-completion/box_plots/view_mask_box_shapenet_table.png" target="_blank">Plot</a></td>
</tr>
</tbody>

</table>


#### Acknowledgements
This project was supported by NSF grants CCF 1011228, DMS 1228304, AFOSR grant FA9550-12-1-0372, ONR MURI grant N00014-13-1-0341, a Google Focused Research Award, the Korea Foundation for Advanced Studies, and the Max Planck Center for Visual Computing and Communications.

<br />
<sub>
**[Shen et al.2012]** Chao-Hui Shen, Hongbo Fu, Kang Chen, and Shi-Min Hu, "Structure Recovery by Part Assembly", SIGGRAPH Asia 2012.<br>
**[Podolak et al.2006]** Joshua Podolak, Philip Shilane, Aleksey Golovinskiy, Szymon Rusinkiewicz, Thomas Funkhouser, "A Planar-Reflective Symmetry Transform for 3D Shapes", SIGGRAPH 2006.<br>
**[COSEG]** Oana Sidi, Oliver van Kaick, Yanir Kleiman, Hao Zhang, Daniel Cohen-Or, "Unsupervised Co-Segmentation of a Set of Shapes via Descriptor-Space Spectral Clustering", SIGGRAPH Asia 2011.<br>
**[ShapeNet]** [http://shapenet.cs.stanford.edu/](http://shapenet.cs.stanford.edu/){:target="_blank"}<br>
</sub>

<br />
