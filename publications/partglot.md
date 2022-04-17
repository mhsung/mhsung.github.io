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


### Language-guided 3D Part Segmentations via Neural Attention

The followings are *random* examples of our segmentation results. 
<a href="javascript:location.reload();">Refresh</a> the webpage to see new random examples.
Given **unsupervised 3D super-segments of shapes** (the first column) and the **referential language**, we learn a set of **attention maps** that corresponds to semantic shape parts, discovered solely by solving the language-reference problems of identifying the target shape.
At test time, we obtain part segments using the attention map of a **template expression**: *“a chair with {part name}”*  (the second to fifth columns). The color goes from blue to yellow for the attention weight zero to one.
The final part segmentation (the sixth column) is obtained by assigning the part label with the highest attention weight to each super-segment.

See the teaser image (Figure 1) and Section A.10. in the [arXiv]({{page.arxiv-link}}){:target="_blank"} version for more examples.

<p align="center">
<iframe src="{{site.baseurl}}/publications/partglot/chair_results.html"
onload='javascript:(function(o){o.style.height=o.contentWindow.document.body.scrollHeight+"px";}(this));'
width="100%" height="100px" 
frameborder="0" scrolling="no" overflow="hidden"></iframe>
</p>


### Out-of-Distribution Test

Tapping on the **zero-shot learning capacity** of natural language learners, and
the shared part composition of common objects, we find examples of zero-shot segmentations on other categories (Airplane, Car, Lamp, and Table), extracted from
learners and **language concerning only chairs**.
<a href="javascript:location.reload();">Refresh</a> the webpage to see new random examples.

See the teaser image (Figure 1) and Section A.10. in the [arXiv]({{page.arxiv-link}}){:target="_blank"} version for more examples.

<p align="center">
<iframe src="{{site.baseurl}}/publications/partglot/other_results.html"
onload='javascript:(function(o){o.style.height=o.contentWindow.document.body.scrollHeight+"px";}(this));'
width="100%" height="100px" 
frameborder="0" scrolling="no" overflow="hidden"></iframe>
</p>

#### Acknowledgements
This work was supported in part by NRF grant (2021R1F1A1045604) and NST grant (CRC 21011) funded by the Korea government(MSIT), Technology Innovation Program (20016615) funded by the Korea government(MOTIE), and grants from the Adobe and KT corporations. L. Guibas also acknowledges the support of ARL grant W911NF2120104, a Vannevar Bush faculty fellowship, and grants from the Adobe, Autodesk, and Snap corporations.

<br />
