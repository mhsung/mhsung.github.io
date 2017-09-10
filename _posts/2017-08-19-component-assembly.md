---
title:  "ComplementMe: Weakly-Supervised Component Suggestions for 3D Modeling"

author: <a href="http://cs.stanford.edu/~mhsung" target="_blank">Minhyuk Sung</a>, <a href="http://ai.stanford.edu/~haosu/" target="_blank">Hao Su</a>, <a href="http://vova.kim" target="_blank">Vladimir G. Kim</a>, <a href="https://www.cse.iitb.ac.in/~sidch/" target="_blank">Siddhartha Chaudhuri</a>, and <a href="https://geometry.stanford.edu/member/guibas/" target="_blank:">Leonidas Guibas</a>

journal: SIGGRAPH Asia 2017

slug: component-assembly

date: 2017-08-19

arxiv-link: https://arxiv.org/abs/1708.01841

paper-link: TBA

supplementary-link: TBA

slides-link: TBA

code-link: TBA
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
>Assembly-based tools provide a powerful modeling paradigm for non-expert shape designers. However, choosing a component from a large shape repository and aligning it to a partial assembly can become a daunting task. In this paper we describe novel neural network architectures for suggesting complementary components and their placement for an incomplete 3D part assembly. Unlike most existing techniques, our networks are trained on unlabeled data obtained from public online repositories, and do not rely on consistent part segmentations or labels. Absence of labels poses a challenge in indexing the database of parts for the retrieval. We address it by jointly training embedding and retrieval networks, where the first indexes parts by mapping them to a low-dimensional feature space, and the second maps partial assemblies to appropriate complements. The combinatorial nature of part arrangements poses another challenge, since the retrieval network is not a function: several complements can be appropriate for the same input. Thus, instead of predicting a single output, we train our network to predict a probability distribution over the space of part embeddings. This allows our method to deal with ambiguities and naturally enables a UI that seamlessly integrates user preferences into the design process. We demonstrate that our method can be used to design complex shapes with minimal or no user input. To evaluate our approach we develop a novel benchmark for component suggestion systems demonstrating significant improvement over state-of-the-art techniques.
<br />

*{{page.author}}<br>
**{{page.title}}**<br>
{{page.journal}}*<br>
[arXiv]({{page.arxiv-link}}){:target="_blank"}  |  Paper (TBA)  |  Slides (TBA)  |  Code (TBA)

### Bibtex
```
@article{Sung:2017,
  author = {Sung, Minhyuk and Su, Hao, and Kim, Vladimir G. and Chaudhuri, Siddhartha and Guibas, Leonidas},
  title = {ComplementMe: Weakly-Supervised Component Suggestions for 3D Modeling},
  Journal = {ACM Transactions on Graphics (Proc. of SIGGRAPH Asia)}, 
  year = {2017}
}
```

### Video
TBA

### Benchmark Results
TBA

#### Acknowledgements
This project was supported by NSF grants IIS-1528025 and DMS-1521608, MURI award N00014-13-1-0341, a Google focused research award, the Korea Foundation for Advanced Studies, and gifts from the Adobe systems and Autodesk corporations.

<br />
