---
title:  "DeformSyncNet: Deformation Transfer via Synchronized Shape Deformation Spaces"

author: <a href="http://mhsung.github.io/" target="_blank">Minhyuk Sung</a>&#42;, <a href="http://jiangzhenyu.xyz/" target="_blank">Zhenyu Jiang</a>&#42;, <a href="http://ai.stanford.edu/~optas/" target="_blank">Panos Achlioptas</a>, <a href="http://www0.cs.ucl.ac.uk/staff/n.mitra/" target="_blank">Niloy J. Mitra</a>, and <a href="https://geometry.stanford.edu/member/guibas/" target="_blank:">Leonidas J. Guibas</a> <br>(&#42; equal contribution)

journal: SIGGRAPH Asia 2020 (To appear)

slug: deform-sync-net

date: 2020-09-03

arxiv-link: http://arxiv.org/abs/2009.01456

code-link: https://github.com/Steve-Tod/DeformSyncNet
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
>Shape deformation is an important component in any geometry processing toolbox. The goal is to enable intuitive deformations of single or multiple shapes or to transfer example deformations to new shapes while preserving the plausibility of the deformed shape(s). Existing approaches assume access to point-level or part-level correspondence or establish them in a preprocessing phase, thus limiting the scope and generality of such approaches. We propose DeformSyncNet, a new approach that allows consistent and synchronized shape deformations without requiring explicit correspondence information. Technically, we achieve this by encoding deformations into a class-specific idealized latent space while decoding them into an individual, model-specific linear deformation action space, operating directly in 3D. The underlying encoding and decoding are performed by specialized (jointly trained) neural networks. By design, the inductive bias of our networks results in a deformation space with several desirable properties, such as path invariance across different deformation pathways, which are then also approximately preserved in real space. We qualitatively and quantitatively evaluate our framework against multiple alternative approaches and demonstrate improved performance.
<br />

*{{page.author}}<br>
**{{page.title}}**<br>
{{page.journal}}*<br>
[arXiv]({{page.arxiv-link}}){:target="_blank"}  | 
[Paper]({{site.baseurl}}/assets/files/{{page.slug}}.pdf){:target="_blank"}  | 
[Code]({{page.code-link}}){:target="_blank"}

### Bibtex
```
@article{Sung:2020,
  author = {Sung, Minhyuk and Jiang, Zhenyu and Achlioptas, Panos and Mitra, Niloy J. and Guibas, Leonidas J.},
  title = {DeformSyncNet: Deformation Transfer via Synchronized Shape Deformation Spaces},
  Journal = {ACM Transactions on Graphics (Proc. of SIGGRAPH Asia)}, 
  year = {2020}
}
```

### Supplementary Video
<p align="center">
  <video width="640" height="360" controls preload>
    <source src="{{site.baseurl}}/assets/videos/{{page.slug}}/{{page.slug}}.webm"></source> 
  </video>
</p>

### Overview & Results

![]({{site.baseurl}}/assets/images/{{page.slug}}/figure_5.png)
<p class="caption">
<b>Fig. 5.</b> Elements in the learned deformation dictionary. The columns are deformations along some elements in the dictionary. Each element shows a natural <i>mode</i> of shape variations changing local parts, and the variations of each element are also <i>consistent</i> across the shapes despite the difference in styles of the shapes. The second column of chairs shows scaling of swivel leg (red circle), and the element does not affect the shapes not including the swivel leg. Also, the second column of tables lifts up the shelf in the middle (blue circle) and makes no change if the part does not exist. Refer to the supplemental video for animated visualizations.
</p><br>

![]({{site.baseurl}}/assets/images/{{page.slug}}/figure_6.png)
<p class="caption">
<b>Fig. 6.</b> Shape editing projection and transfer results. The first column is the source shape, the second column is the user edit (blue and red arrows mean translation and scaling along the direction, respectively), the third and fourth columns are the results of projection (with and without the part bounding boxes), the fifth column is the new source shape, and the sixth and seventh columns are the results of transferring the projected deformation to the new source shape (with and without the part bounding boxes). The projection adjusts the rest of the deformation handles while preserving part connectivity (red circles) and symmetry (green circles). Also, the projected deformations are naturally transferred to the new shape despite the different part structures  (blue circles). See the supplemental video for more examples.
</p><br>

#### Acknowledgements
N. J. Mitra acknowledges the support of ERC PoC Grant, Google Faculty Award, Royal Society Advanced Newton Fellowship, and gifts from Adobe. L. J. Guibas acknowledges the support of a Vannevar Bush Faculty Fellowship, a Samsung GRO grant, a Google Daydream Research Award, and gifts from the Adobe, Autodesk, and Snap corporations.

<br />
