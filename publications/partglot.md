---
layout: page

title:  "PartGlot: Learning Shape Part Segmentation from Language Reference Games"

author: <a href="https://github.com/63days" target="_blank">Juil Koo</a>, <a href="https://ianhuang0630.github.io/" target="_blank">Ian Huang</a>, <a href="http://ai.stanford.edu/~optas/" target="_blank">Panos Achlioptas</a>, <a href="https://geometry.stanford.edu/member/guibas/" target="_blank">Leonidas Guibas</a>, <a href="http://mhsung.github.io/" target="_blank">Minhyuk Sung</a>

journal: CVPR 2022

slug: partglot

date: 2022-03-14

arxiv-link: https://arxiv.org/abs/2112.06390

code-link: https://github.com/63days/PartGlot
---


## {{ page.title }}
{:.title}
#### {{ page.author }}
{:.title}
#### {{ page.journal }}
{:.title}

<br />
![]({{site.baseurl}}/assets/images/{{page.slug}}-teaser.png)

### Abstract
>We introduce PartGlot, a neural framework and associated architectures for learning semantic part segmentation of 3D shape geometry, based solely on part referential language. We exploit the fact that linguistic descriptions of a shape can provide priors on the shape's parts -- as natural language has evolved to reflect human perception of the compositional structure of objects, essential to their recognition and use. For training, we use the paired geometry / language data collected in the ShapeGlot work for their reference game, where a speaker creates an utterance to differentiate a target shape from two distractors and the listener has to find the target based on this utterance. Our network is designed to solve this target discrimination problem, carefully incorporating a Transformer-based attention module so that the output attention can precisely highlight the semantic part or parts described in the language. Furthermore, the network operates without any direct supervision on the 3D geometry itself. Surprisingly, we further demonstrate that the learned part information is generalizable to shape classes unseen during training. Our approach opens the possibility of learning 3D shape parts from language alone, without the need for large-scale part geometry annotations, thus facilitating annotation acquisition.
<br />

*{{page.author}}<br>
**{{page.title}}**<br>
{{page.journal}}*<br>
[arXiv]({{page.arxiv-link}}){:target="_blank"}  | 
[Code]({{page.code-link}}){:target="_blank"}

### Bibtex
```
@proceedings{PartGlot:2022,
  author = {Koo, Juil and Huang, Ian and Achlioptas, Panos and Guibas, Leonidas and Sung, Minhyuk},
  title = {PartGlot: Learning Shape Part Segmentation from Language Reference Games},
  booktitle = {CVPR}, 
  year = {2022}
}
```


#### Acknowledgements
This work was supported in part by NRF grant (2021R1F1A1045604) and NST grant (CRC 21011) funded by the Korea government(MSIT), Technology Innovation Program (20016615) funded by the Korea government(MOTIE), and grants from the Adobe and KT corporations. L. Guibas also acknowledges the support of ARL grant W911NF2120104, a Vannevar Bush faculty fellowship, and grants from the Adobe, Autodesk, and Snap corporations.

<br />