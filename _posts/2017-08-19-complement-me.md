---
title:  "ComplementMe: Weakly-Supervised Component Suggestions for 3D Modeling"

author: <a href="http://mhsung.github.io/" target="_blank">Minhyuk Sung</a>, <a href="http://cseweb.ucsd.edu/~haosu/" target="_blank">Hao Su</a>, <a href="http://www.vovakim.com/" target="_blank">Vladimir G. Kim</a>, <a href="https://www.cse.iitb.ac.in/~sidch/" target="_blank">Siddhartha Chaudhuri</a>, and <a href="https://geometry.stanford.edu/member/guibas/" target="_blank:">Leonidas Guibas</a>

journal: SIGGRAPH Asia 2017

slug: complement-me

date: 2017-08-19

arxiv-link: https://arxiv.org/abs/1708.01841

code-link: https://github.com/mhsung/complement-me
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
[arXiv]({{page.arxiv-link}}){:target="_blank"}  | 
[Paper]({{site.baseurl}}/assets/files/{{page.slug}}.pdf){:target="_blank"}  | 
[Slides(PPTX)]({{site.baseurl}}/assets/files/{{page.slug}}-slides.pptx){:target="_blank"}  | 
[Code]({{page.code-link}}){:target="_blank"}

### Bibtex
```
@article{Sung:2017,
  author = {Sung, Minhyuk and Su, Hao and Kim, Vladimir G. and Chaudhuri, Siddhartha and Guibas, Leonidas},
  title = {Complement{Me}: Weakly-Supervised Component Suggestions for 3D Modeling},
  Journal = {ACM Transactions on Graphics (Proc. of SIGGRAPH Asia)}, 
  year = {2017}
}
```

### Data download
We provide ShapeNet model component and semantic part data used in the paper. You can directly download the *point cloud* and *contact graph* data in the following links:
- [Components (877M)](https://shapenet.cs.stanford.edu/media/minhyuk/ComplementMe/data/components.tgz)<br>
  Point cloud and contact graph data of components (generated as described in Sec 4. of the paper). Refer to the included README file for the details of the data structure.
- [Semantic parts (220M)](https://shapenet.cs.stanford.edu/media/minhyuk/ComplementMe/data/parts.tgz)<br>
  Point cloud data of semantic parts. This is a *subset* of ShapeNet semantic part dataset created by [[Yi et al. 2016]](https://cs.stanford.edu/~ericyi/project_page/part_annotation/index.html){:target="_blank"}. Refer to the included README file for the details of the data structure.

The *mesh* data is only provided to people who have already signed up for [ShapeNet](https://www.shapenet.org/){:target="_blank"} and have agreed to the Terms of Use. To download the mesh data, please fill out an agreement to the [ShapeNet Terms of Use]({{site.baseurl}}/assets/misc/ShapeNet_Terms_of_Use.pdf){:target="_blank"} with the ShapeNet account email address, and send it to <a href="mailto:mhsung@cs.stanford.edu">mhsung@cs.stanford.edu</a>.

Please cite [our paper](#bibtex) and [all related papers](#acknowledgements) if you use this dataset in your research.

### Video
<p align="center">
  <video width="640" height="360" controls preload>
    <source src="{{site.baseurl}}/assets/videos/{{page.slug}}/{{page.slug}}.webm"></source> 
  </video>
</p>

### Overview & Results

![]({{site.baseurl}}/assets/images/{{page.slug}}/figure_2.png)
<p class="caption">
<b>Fig. 2.</b> Overview of the retrieval process at test time. From the given partial assembly, the retrieval network predicts a probability distribution (modeled as a mixture of Gaussians) over the component embedding space. Suggested complementary components are sampled from the predicted distribution, and then the placement network predicts their positions with respect to the query assembly.
</p><br>

![]({{site.baseurl}}/assets/images/{{page.slug}}/figure_7.png)
<p class="caption">
<b>Fig. 7.</b> Automatic iterative assembly results from a single component. Small component not typically labeled with semantics in the shape database (e.g. as slats between chair/table legs, pillows on sofas, cords in lamps/watercrafts) are appropriately retrieved and placed.
</p><br>

![]({{site.baseurl}}/assets/images/{{page.slug}}/figure_8.png)
<p class="caption">
<b>Fig. 8.</b> Automatic iterative assembly with two different random choices at every time. From the initial component at the bottom, various objects are synthesized
by assembling different components.
</p>

### More Results
Automatic shape synthesis with maximal probability components (More examples of <b>Fig.7.</b>) <br>

| <a href="https://shapenet.cs.stanford.edu/media/minhyuk/ComplementMe/images/assembly_max_prob/Airplane/index.html" target="_blank">Airplane</a> | <a href="https://shapenet.cs.stanford.edu/media/minhyuk/ComplementMe/images/assembly_max_prob/Car/index.html" target="_blank">Car</a> | <a href="https://shapenet.cs.stanford.edu/media/minhyuk/ComplementMe/images/assembly_max_prob/Chair/index.html" target="_blank">Chair</a> | <a href="https://shapenet.cs.stanford.edu/media/minhyuk/ComplementMe/images/assembly_max_prob/Guitar/index.html" target="_blank">Guitar</a> | <a href="https://shapenet.cs.stanford.edu/media/minhyuk/ComplementMe/images/assembly_max_prob/Lamp/index.html" target="_blank">Lamp</a> | <a href="https://shapenet.cs.stanford.edu/media/minhyuk/ComplementMe/images/assembly_max_prob/Rifle/index.html" target="_blank">Rifle</a> | <a href="https://shapenet.cs.stanford.edu/media/minhyuk/ComplementMe/images/assembly_max_prob/Sofa/index.html" target="_blank">Sofa</a> | <a href="https://shapenet.cs.stanford.edu/media/minhyuk/ComplementMe/images/assembly_max_prob/Table/index.html" target="_blank">Table</a> | <a href="https://shapenet.cs.stanford.edu/media/minhyuk/ComplementMe/images/assembly_max_prob/Watercraft/index.html" target="_blank">Watercraft</a> |

<br>

Automatic shape synthesis with two different random choices each time (More examples of <b>Fig.8.</b>) <br>

| <a href="https://shapenet.cs.stanford.edu/media/minhyuk/ComplementMe/images/assembly_bin_tree/Airplane/index.html" target="_blank">Airplane</a> | <a href="https://shapenet.cs.stanford.edu/media/minhyuk/ComplementMe/images/assembly_bin_tree/Car/index.html" target="_blank">Car</a> | <a href="https://shapenet.cs.stanford.edu/media/minhyuk/ComplementMe/images/assembly_bin_tree/Chair/index.html" target="_blank">Chair</a> |<a href="https://shapenet.cs.stanford.edu/media/minhyuk/ComplementMe/images/assembly_bin_tree/Guitar/index.html" target="_blank">Guitar</a> | <a href="https://shapenet.cs.stanford.edu/media/minhyuk/ComplementMe/images/assembly_bin_tree/Lamp/index.html" target="_blank">Lamp</a> | <a href="https://shapenet.cs.stanford.edu/media/minhyuk/ComplementMe/images/assembly_bin_tree/Rifle/index.html" target="_blank">Rifle</a> | <a href="https://shapenet.cs.stanford.edu/media/minhyuk/ComplementMe/images/assembly_bin_tree/Sofa/index.html" target="_blank">Sofa</a> | <a href="https://shapenet.cs.stanford.edu/media/minhyuk/ComplementMe/images/assembly_bin_tree/Table/index.html" target="_blank">Table</a> | <a href="https://shapenet.cs.stanford.edu/media/minhyuk/ComplementMe/images/assembly_bin_tree/Watercraft/index.html" target="_blank">Watercraft</a> |

#### Acknowledgements
This project was supported by NSF grants IIS-1528025 and DMS-1521608, MURI award N00014-13-1-0341, a Google focused research award, the Korea Foundation for Advanced Studies, and gifts from the Adobe systems and Autodesk corporations.

<br />
<sub>
**[Yi et al.2016]** Li Yi, Vladimir G. Kim, Duygu Ceylan, I-Chao Shen, Mengyan Yan, Hao Su, Cewu Lu, Qixing Huang, Alla Sheffer, and Leonidas Guibas, "A Scalable Active Framework 
for Region Annotation in 3D Shape Collections", SIGGRAPH Asia 2016.<br>
**[ShapeNet]** [http://shapenet.cs.stanford.edu/](http://shapenet.cs.stanford.edu/){:target="_blank"}<br>
</sub>

<br />
