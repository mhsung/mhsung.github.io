---
title: "CS492(H): Machine Learning for 3D Data"

topic: "Project Submission Guidelines"

class_info: <a href="http://mhsung.github.io/" target="_blank">Minhyuk Sung</a>, <a href="https://www.kaist.ac.kr/" target="_blank">KAIST</a>, Spring 2021

slug: project-submission-guidelines

date: 2021-05-20
---


## <a href="{{site.baseurl}}/{{page.path}}/../../" target="_blank">{{ page.title }}</a>
{:.title}
## {{ page.topic }}
{:.title}
#### {{ page.class_info }}
{:.title}
<br />


<style>
em { font-style: normal; font-weight: bold; color: #C62828 }
h { background-color:#FFC107 }
</style>


### Table of Contents
1. [Submission Deadline](#submission-deadline')
2. [Submission Guidelines](#submission-guidelines)
3. [Poster Sessions](#poster-sessions)
4. [Review Guidelines](#review-guidelines)
5. [Review Questions](#review-questions)


<br>

---

<div id='submission-deadline'/>
### 1. Submission Deadline

<h>Jun 06 (Sun), 23:59 KST</h>


<br>

---

<div id='submission-guidelines'/>
### 2. Submission Guidelines

*TBA.*<br>

- Must include a *report*, a *poster*, and a *code repository link*.<br>
- *Supplementary materials* are optional.
- Submission with the *wrong format* or any *missing items* may receive a *zero* score.


#### Report Guidelines

<b>Format</b>
- A *single PDF* file (maximum 20MB). Supplementary materials are allowed.
- Must be in *CVPR* format:<br>
[LaTeX/Word Templates Zip file (CVPR 2021 format)](http://cvpr2021.thecvf.com/sites/default/files/2020-09/cvpr2021AuthorKit_2.zip){:target="_blank"}<br>
[Overleaf template (CVPR 2018 format)](https://www.overleaf.com/latex/templates/cvpr-2018-template/qgmrfntfbqns){:target="_blank"}
- Must be up to *four* pages long, including figures, tables, and acknowledgments, but not references. Additional pages containing only cited references are allowed.

<h><b>Structure</b></h>
Please use the *same section names* below to facilitate the review process.<br>
Additional sections/subsections are allowed. Also, the detailed instructions in each section are *recommendations*, and you do need to exactly follow them.

<h><b>[Development Track]</b></h><br>

<h><em>DO NOT COPY the texts or figures in the original paper — it will be considered as Plagiarism</em>. Write the report in your own words.</h><br>

- <b>Abstract</b>
    - one-sentence *TL;DR*,
    - 2-3 sentences for the *motivation* and *key ideas* of the original work,
    - a few sentences summary of the *implementation challenges* and *your approaches*, and
    - 1-2 sentences summary of the *experimental results*.
    - In the end, add *“Code is available at: {link}.”*

- <b>Introduction</b>
    - What is the *motivation* of the (original) work? Why is it important to solve the problem? What would be the potential impacts of this work in the research field, or what would be the potential applications?
    - What is the *problem setup* the original work introduce? (Add a citation of the original work.)  What are the input and desired output? What are the given information in the training time and the given assumptions? What are the *main ideas* of the original work to solve the problem?
    - What are the *key challenges* in implementing the proposed method? Does the framework include some components that are not implemented in public libraries (e.g., PyTorch, PyTorch3D)? Are you implementing some components from scratch without the public libraries? (Using CUDA?) Are there lots of components to implement? Are there lots of technical details hidden in the paper/code? Doesn't the authors provide their code or datasets? Does the authors' code even not reproduce the results in the paper? Is the network training tricky or unstable? Or, do you improve the original work?
    - Summarize the *implementation details*. *Clearly differentiate* the parts you implemented and the parts you borrowed existing code or got some help from the external collaborators. How did you implement each part, and how did you handle the challenges? A *teaser* figure that illustrates the parts you focused on in the implementation would be great.
    - Briefly describe the *experimental setups*. Which datasets/benchmarks did you use? How did you evaluate the results? Did you need to make any changes in the experimental setups of the original work? If yes, why? How good are your results compared with the results reported in the original paper (or the results of the authors' code)? Did you conduct more experiments than the original work?
    - A *summary of contributions* (in terms of providing your code) at the end is also recommended (in a bullet point list). You can start the summary with (for example) ‘In summary, our contributions are:’.

- <b>Method Summary</b>
    - Describe the *problem setup* again, but in detail and also in a formal way. Introduce essential math notations for the following formulations. <h><em>DO NOT COPY the texts or figures in the original paper</em></h>, but use the *same math notations* in the original work.
    - Briefly *summarize* the method proposed in the original work, while focusing on the parts that you implemented (if you used existing codes for some parts). The report needs to be *self-contained*; the readers must be able to understand the main ideas without reading the original paper.


- <b> Implementation Details</b>
    - First, clearly state *which parts you implemented*. If you used some existing codes, describe *how you adopted the existing codes* as well in detail. Add *references* for the existing codes. <h><em>Hiding the use of existing codes will be considered as plagiarism</em></h>.
    - *Data generation/preprocessing* and *evaluations* are also parts of the implementation. If you implemented these yourself, illustrate the details.
    - Consider as you explain the implementation details in a way that the readers can reproduce the results (like providing a *recipe in cooking*). Make the exposition *easy to follow*, but also *clear* and *specific* as much as possible.
    - Use visual aids in your exposition. More would be better. But <h><em>DO NOT COPY figures in the original paper.</em></h> Formulations are fine (but do not copy and paste an image but write them yourself).

- <b>Experimental Results</b>
    - Clearly describe the *experiment setups*, including *benchmarks/datasets* and *evaluation metrics*. If you change or simplify the experimental setups of the original work, explain why.
    - Provide *comparisons* with the original work. Use the *exact results* reported in the original paper for comparison. If you test the authors' code in new datasets, explain why. Provide both *quantitative results (tables)* and *qualitative results (figures)*. Explain in which aspects the results of your method is better or comparable.
    - Try to reproduce *all the results* in the original paper. Any *lack of experiments, evaluations, or comparisons* (without any appropriate reasons) will be penalized in the evaluation.
    - Make *fair*, *apple-to-apple* comparisons. Unfair benefits to your implementation in the experiments will also be penalized.
    - If you achieve *better performance* than the original work, if you *improve* the proposed algorithm, or if you conduct some *additional experiments* that were not performed in the original paper, *emphasize* the results.
    - In here or in the conclusion, consider showing some *remarkable failure cases* explaining the limitation of the proposed method or your implementation, or motivating some future works.

- <b>Conclusion</b>
    - Briefly *summarize* the project, particularly the main parts you implemented and the experimental results.
    - Describe the *limitation* of the proposed work or your implementation and *potential future research directions* (if you have space in the report).

- <b>Acknowledgments</b>
    - Make it as a subsection (without a section number) or a paragraph.
    - Describe the *role* of each team member and the *external collaborators* and their contributions.
    - <h><em>Hiding the external collaborators will be considered committing academic dishonesty.</em></h>


<br>


<h><b>[Research Track]</b></h><br>

- <b>Abstract</b><br>
    - one-sentence *TL;DR*,
    - 1-2 sentences for the *motivation* of the work,
    - a few sentences summary of the *problem statement and key contributions*, and
    - 1-2 sentences summary of the *experimental results*.
    - In the end, add *"Code is available at: {link}."*
- <b>Introduction</b>
    - What is the *motivation* of the work? Why is it important to solve the problem? What would be the potential impacts of this work in the research field, or what would be the potential applications?
    - What are the *challenges* in the problem? How has previous work approached this problem, and what are the limitations (add citations)? Or, why hasn't the problem been addressed while it is important?
    - What is the *problem statement*? What are the input and desired output? What are the given information in the training time and the given assumptions? A *teaser figure* that effectively illustrates the problem setup or the desired output would be great. (E.g., show the best result with the input.)
    - What are your *key ideas* for solving the challenges? It would be also great if your teaser image also describes the key ideas. (E.g. how do your key ideas make differences in the results?)
    - Briefly describe the *experimental setups*. Which datasets/benchmarks did you use? How did you evaluate the results? What is the conclusion? (E.g. our method outperformed SotA methods by huge margins.)
    - *A summary of contributions* at the end is also recommended (in a bullet point list). You can start the summary with (for example) 'In summary, our contributions are:'.
- <b>Related Work</b>:
    - Consider making *two or three* groups of related papers and writing a short paragraph for each of them, which a *paragraph title*. Also, an intro sentence briefly describing the groups is recommended (but not necessary). E.g., if your project is about '3D GAN', you can consider groups of 'Deep Learning for 3D Data' and 'Deep Generative Models'.
    - Summarize each work with 1-2 sentences while focusing on describing in which aspects your work is *different* or *overcoming the limitations*.

- <b>Method</b>
    - Describe the *problem setup* again, but in detail and also in a formal way. Introduce *essential math notations* for the following formulations. A *figure* describing the overall method is recommended.
    - The report needs to be *self-contained*; the readers must be able to understand the ideas without reading the other papers. Provide *background knowledge* if needed (not necessary). If needed, provided the 'minimal' background to understand your work.
    - Think about the most effective way of explaining the *key ideas*. One option would be *prioritizing* components in your method not based on the order in the method but based on the *importance*. Less important details can go to the end or to the supplementary.
    - Use *visual aids* in your exposition. More would be better.
    - Make the exposition as *clear* and *specific* as possible. *Formulations* can make the exposition clearer and more concise.
- <b>Experimental Results</b>:
    - Clearly describe the *experiment setups*, including *benchmarks/datasets*, *evaluation metrics*, and *baseline methods*.
    - Provide both *quantitative results (tables)* and *qualitative results (figures)*. Provide *comparisons* with the baseline methods. Explain in which aspects your method is better. Think about the best way to demonstrate the advantages of your method over the baseline methods.
    - Conduct the *ablation study* and show the results. If you have multiple technical contributions, demonstrate how each component affects the results.
    - *Do not miss* any well-known benchmarks/datasets, standard evaluation metrics, or previous methods. Any *lack of experiments, evaluations, or comparisons* will be penalized in the evaluation.
    - Make *fair*, *apple-to-apple* comparisons. (Or, if the baseline methods take some advantages such as stronger supervision, describe clearly.) Unfair benefits to the proposed method in the experiments will also be penalized.
    - In here or in the conclusion, consider showing some *remarkable failure cases* explaining the limitation of the proposed method or motivating some future works.

- <b>Conclusion</b>
    - Briefly *summarize* the project, particularly the *key ideas* and the *experimental results*.
    - Describe the *limitation* of the proposed work and *potential future research* directions (if you have space in the report).

- <b>Acknowledgments</b>
    - Make it as a subsection (without a section number) or a paragraph.
    - Describe the *role* of each team member and the *external collaborators* and their contributions.
    - <h><em>Hiding the external collaborators will be considered committing academic dishonesty.</em></h>


#### Poster Guidelines

<b>Format</b>
- A *single PNG* file (maximum 3MB).
- Must have *2560x1280* resolution.
- Poster template: [<b>Link</b>](https://kaistackr-my.sharepoint.com/:p:/g/personal/mhsung_kaist_ac_kr/EQz68whVxahPoGdcBExRSqIBhcbldxFCXE9p-otheEmCTg?e=VF2sNi){:target="_blank"} (Design adapted from [Zoya Bylinskii](https://web.mit.edu/zoya/www/docs.html){:target="_blank"})<br>
Do not need to use this template.
- Must include *project title*, *project track*, *team member names*, and *acknowledgments*.


<b>Resources</b>
- [<b>How to Make a More Effiective Research Poster (Zoya Bylinskii)</b>](https://web.mit.edu/zoya/www/posterRecommendations.pdf){:target="_blank"}


#### Code Submission
- Create a *public code repository* in GitHub or Bitbucket and submit the link.
- Also, add the link in the *abstract* of the report (see [Report Guidelines](#report-guidelines)).


#### Supplementary Materials

- Supplementary materials are optional.
- Any formats (PDF document, video, web page) are allowed (maximum 100MB).
- Submit as a *ZIP* file.

#### <h>Plagiarism / Academic Dishonesty</h>
If plagiarism or academic dishonesty is found in your report, poster, or code, you will receive an F grade, and also it will be reported to the university.


[Back to top](#)
<br>

---

<div id='poster-sessions'/>
### 3. Poster Sessions (Virtual)

*TBA.*<br>

We'll use [Gather.town](https://gather.town/){:target="_blank"}.


[Back to top](#)
<br>

---

<div id='review-guidelines'/>
### 4. Review Guidelines

*TBA.*<br>

- Each project will be reviewed by *four* peer reviewers.
- The review will be *single-blind* and will be performed in *OpenReview*.<br>
(Both the submissions and reviews will NOT be open to the public.)
- Reviews can be *rejected* based on the assessment of the review quality.
- Each *unsubmitted* or *rejected* review will be *penalized by 20%* in the project evaluation.


[Back to top](#)
<br>

---

<div id='review-questions'/>
### 5. Review Questions

#### <h>Project Summary</h>

<b>Please summarize the project idea in your own words (3+ sentences).</b><br>
*Please read the report thoroughly. Your review can be rejected based on the assessment of the review quality. Each unsubmitted or rejected review will be penalized by 20% in the project evaluation.*<br>


#### <h>Report Evaluation</h>

<b>[All] (Introduction) Are the motivation and problem statement clearly described?</b><br>
- Yes.
- No. (Please describe the details in the detailed comments.)


<b>[All] (Introduction) Are the implementation challenges (Development) or the technical contributions/novelties (Research) clearly described?</b><br>
- Yes.
- No. (Please describe the details in the detailed comments.)


<b>[Development] (Method Summary) Is the method summary clearly described (including input, desired output, supervision provided in the network training, representation of the data, etc)?</b><br>
- Yes.
- No. (Please describe the details in the detailed comments.)
- Research track.


<b>[Development] (Implementation Details) Are the implementation details clearly described (including the parts where the existing codes are used)?</b><br>
- Yes.
- No. (Please describe the details in the detailed comments.)
- Research track.


<b>[Research] (Related Work) Is the related work adequate, and Is relation to prior work well-explained? (If not, is there any missing prior work?)</b><br>
- Yes.
- No. (Please describe the details in the detailed comments.)
- Development track.


<b>[Research] (Method) Is the method clearly described (including input, desired output, supervision provided in the network training, representation of the data, main technical ideas, etc)?</b><br>
- Yes.
- No. (Please describe the details in the detailed comments.)
- Development track.


<b>[All] (Experimental Results) Are the experiment setups clearly described (including benchmarks/datasets, evaluation metrics, baseline methods, quantitative/qualitative results, comparisons, failure cases)?</b><br>
- Yes.
- No. (Please describe the details in the detailed comments.)


<b> [All] (Acknowledgments) Are the 1) the role of each team member and 2) the external collaborators and their contributions clearly described?</b><br>
- Yes.
- No. (Please describe the details in the detailed comments.)


<b> [All] Overall, is the report well-organized and clearly written? If not, should there be additional explanations or illustrations?</b><br>
- Clear, only minor flaws. 
- Mostly clear, but improvements needed. (Please describe the details in the detailed comments.) 
- Difficult to understand in places. (Please describe the details in the detailed comments.) 
- Very hard to understand. (Please describe the details in the detailed comments.) 


#### <h>Overall Evaluation</h>

<b>[Development] (Degree of Challenges) How do you assess the difficulty of the implementation (when considering the number of team members, external collaborators, the parts where the submitters used the existing codes)?</b><br>
- Very hard, requires extraordinary efforts and/or skills.
- Challenging.
- Moderate. Doable.
- Easy.


<b>[Research] (Novelty) Does it present a new concept or idea?</b><br>
- Proposes novel and interesting views, ideas, or problems .
- Worthy contributions with some novel (but small) ideas. 
- Minor variations to existing techniques .
- Does not advance the state of knowledge , or closely duplicates existing work.


<b>[Research] (Technical quality) Is the approach technically sound?</b><br>
- Technically very strong and solid.
- Technically adequate.
- A few minor flaws.
- Claims not completely supported, assumptions or simplifications unrealistic, fatal mistakes.


<b>[All] (Experimental Results) Are the experiments well designed, sufficient, clearly described?</b><br>
- Extensive, detailed, and informative evaluations without any missing benchmarks/datasets, evaluation metric, and comparison.
- Solid and sufficient to convince the merits of the proposed method (Research) or the performance of the implementation (Development) (although lacking some minor experiments or simplifying the experiment setup a bit.)
- Lacking some important experiments (in terms of benchmarks/datasets, evaluation metrics, comparisons, quantitative/qualitative results, etc).
- Insufficient, unfair, inadequate, or uninformative comparisons with related work  (Research) or the original work (Development).


<b>[Development] (Reproduction) Did the implementation reproduce the results in the original work?</b><br>
- Yes, and even improved/outperformed the original work, or showed more results in different applications.
- Almost, the results are similar.
- A bit worse but comparable.
- Significantly worse, or couldn’t reproduce the results at all.


<b>[All] (Strengths) Describe the strengths of the work in bullet points (with 2-3 bullets).</b><br>


<b>[All] (Weaknesses) Describe the weaknesses of the work in bullet points (with 2-3 bullets).</b><br>


<b>[All] (Detailed Comments) Describe the detailed comments here and how you decided the ‘Overall Score’.</b><br>
*Please be constructive, respectful, and detailed in your comments.*<br>


<b>[All] (Feedback) Provide questions or comments to the submitters if you have.</b><br>


<b>[All] (Overall Score) Please provide an "overall score" for this submission (in [1-5] range).</b><br>
<br>


#### <h>Scoring Criteria</h>

*Criteria of score 4 (‘Great!’) (AND conditions)*<br>
- [All] <b>(Report Writing)</b> The report is well-organized and clearly written.
- [All] <b>(Experiment Designs)</b> The experiments are well-designed and convincing.
- [Development] <b>(Experimental Results)</b> Achieved similar results in a challenging development task with the original or improved/outperformed the original work in a doable task.
- [Research] <b>(Experimental Results)</b> Achieved promising results. Worth pursuing the direction for future paper publication (although not ready for now).
- [All] <b>(Etc)</b> No significant flaws in the report writing, experimental result demonstration, and poster presentation.

*Criteria of score 5 (‘Outstanding!’)*<br>
- Better than ‘Great!’. Probably the best project in the class.

*Criteria of score 3 (‘Good!’)*<br>
- Has one significant reason not to be ‘Great!’.

*Criteria of score 2 (‘Not Good’) (OR conditions)*<br>
- Has two significant reasons not to be ‘Great!’.
- Shows poor experimenal designs or experimental results or technical contributions (while everything else is ok).

*Criteria of score 1 (‘Poor’) (OR conditions)*<br>
- Has three or more significant reasons not to be ‘Great!’.
- Shows poor experimental designs or experimental results or technical contributions, and has one more significant reason not to be ‘Great!’.

[Back to top](#)

<br/>

