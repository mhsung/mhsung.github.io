---
title:  "Learning Fuzzy Set Representations of Partial Shapes on Dual Embedding Spaces"

author: <a href="http://mhsung.github.io/" target="_blank">Minhyuk Sung</a>, <a href="http://web.stanford.edu/~adkarni/" target="_blank">Anastasia Dubrovina</a>, <a href="http://www.vovakim.com/" target="_blank">Vladimir G. Kim</a>, and <a href="https://geometry.stanford.edu/member/guibas/" target="_blank:">Leonidas Guibas</a>

journal: Conditionally accepted to SGP 2018

slug: fuzzy-set-dual

date: 2018-05-25

arxiv-link: https://arxiv.org/abs/????

paper-link: https://www.dropbox.com/s/kz06kob99iwwdg7/fuzzy-set-dual.pdf?dl=1

slides-link: https://www.dropbox.com/s/x161i48rcwrbc28/fuzzy-set-dual-presentation.pptx?dl=1

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
>Modeling relations between components of 3D objects is essential for many geometry editing tasks. Existing techniques commonly rely on labeled components, which requires substantial annotation effort and limits components to a dictionary of pre-defined semantic parts. We propose a novel framework based on neural networks that analyzes an uncurated collection of 3D models from the same category and learns two important types of semantic relations among full and partial shapes: complementarity and interchangeability.  The former helps to identify which two partial shapes make a complete plausible object, and the latter indicates that interchanging two partial shapes from different objects preserves the object plausibility. Our key idea is to jointly encode both relations by embedding partial shapes as fuzzy sets in dual embedding spaces. We model these two relations as fuzzy set operations performed across the dual embedding spaces, and within each space, respectively. We demonstrate the utility of our method for various retrieval tasks that are commonly needed in geometric modeling interfaces.
<br />

*{{page.author}}<br>
**{{page.title}}**<br>
{{page.journal}}*<br>
arXiv: TBA  |  [Code]({{page.code-link}}){:target="_blank"}

### Bibtex
```
@article{Sung:2018,
  author = {Sung, Minhyuk and Dubrovina, Anastasia, and Kim, Vladimir G. and Guibas, Leonidas},
  title = {Learning Fuzzy Set Representations of Partial Shapes on Dual Embedding Spaces},
  Journal = {Computer Graphics Forum (Proc. of Symposium on Geometry Processing (SGP))}, 
  year = {2018}
}
```

<!---
#### Acknowledgements
This project was supported by NSF grants IIS-1528025 and DMS-1521608, MURI award N00014-13-1-0341, a Google focused research award, the Korea Foundation for Advanced Studies, and gifts from the Adobe systems and Autodesk corporations.
-->

<br />
