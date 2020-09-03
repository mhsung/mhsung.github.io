---
title:  "DeformSyncNet: Deformation Transfer via Synchronized Shape Deformation Spaces"

author: <a href="http://mhsung.github.io/" target="_blank">Minhyuk Sung*</a>, <a href="http://jiangzhenyu.xyz/" target="_blank">Zhenyu Jiang*</a>, <a href="http://ai.stanford.edu/~optas/" target="_blank">Panos Achlioptas</a>, <a href="http://www0.cs.ucl.ac.uk/staff/n.mitra/" target="_blank">Niloy J. Mitra</a>, and <a href="https://geometry.stanford.edu/member/guibas/" target="_blank:">Leonidas J. Guibas</a>

journal: SIGGRAPH Asia 2020

slug: deform-sync-net

date: 2020-09-03

arxiv-link: https://arxiv.org/abs/1807.01519

code-link: https://github.com/mhsung/fuzzy-set-dual
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
[Slides(PPTX)]({{site.baseurl}}/assets/files/{{page.slug}}-slides.pptx){:target="_blank"}  | 
[Code]({{page.code-link}}){:target="_blank"}

### Bibtex
```
@article{Sung:2018,
  author = {Sung, Minhyuk and Jiang, Zhenyu and Achlioptas, Panos and Mitra, Niloy J. and Guibas, Leonidas J.},
  title = {Learning Fuzzy Set Representations of Partial Shapes on Dual Embedding Spaces},
  Journal = {ACM Transactions on Graphics (Proc. of SIGGRAPH Asia)}, 
  year = {2020}
}
```

<!---
#### Acknowledgements
N. J. Mitra acknowledges the support of ERC PoC Grant, Google Faculty Award, Royal Society Advanced Newton Fellowship, and gifts from Adobe. L. J. Guibas acknowledges the support of a Vannevar Bush Faculty Fellowship, a Samsung GRO grant, a Google Daydream Research Award, and gifts from the Adobe, Autodesk, and Snap corporations.
-->

<br />
