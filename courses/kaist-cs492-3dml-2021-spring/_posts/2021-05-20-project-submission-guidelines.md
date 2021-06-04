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
1. [Submission Deadline & Website](#submission-deadline-website)
2. [Corrections and Clarifications](#corrections-and-clarifications)
3. [Submission Guidelines](#submission-guidelines)
4. [Review Guidelines](#review-guidelines)
5. [Review Questions](#review-questions)


<br>


---

<div id='submission-deadline-website'/>
### 1. Submission Deadline & Website

*Submission deadline*: <h><b>Jun 06 (Sun), 23:59 KST</b></h><br>
*OpenReview* submission website:<br>
[https://openreview.net/group?id=kaist.ac.kr/KAIST/Spring2021/CS492H](https://openreview.net/group?id=kaist.ac.kr/KAIST/Spring2021/CS492H){:target="_blank"}<br>


<br>

---

<div id='corrections-and-clarifications'/>
### 2. Corrections and Clarifications
- <b>[Report Guidelines]</b> The review will be *single-blind*. Add *author names* in the report (*uncomment* `\cvprfinalcopy` in the CVPR template).
- <b>[Report Guidelines]</b> Add the *project type* (Development Track / Research Track) in the *second line* of the report title. Using LaTex, you can add like this: `\title{Project Title \\ {Development/Research} Track}`.
- <b>[Report Guidelines]</b> <em>Acknowledgments section is required</em>, even when you do not have the other team member, external collaborators, or any data/codes you borrowed from the other places (state the fact).
- <b>[Report Guidelines]</b> For development track, it is allowed to *use qualitative result figures* in the original paper for comparisons (actually *highly recommended*), but *clearly mention* that the figures are from the original paper.
- <b>[Code Submission]</b> In the code repository, provide *links of the pretrained models* (stored in Google Drive or any other places) and also *datasets you created*, so that anyone can easily check the replicability.
- <b>[Review Guideline]</b> Guidelines about "<a href="{{site.baseurl}}/{{page.path}}/../../project-submission-guidelines.html#infeasible-experiments">Infeasible Experiments</a>" are added. The review question about experimental results is also revised to refer to the guidelines about "Infeasible Experiments".


<br>
[Back to top](#)
<br>

---

<div id='submission-guidelines'/>
### 3. Submission Guidelines

<h><em>OpenReview</em> submission website:</h>
[https://openreview.net/group?id=kaist.ac.kr/KAIST/Spring2021/CS492H](https://openreview.net/group?id=kaist.ac.kr/KAIST/Spring2021/CS492H){:target="_blank"}<br>

If you don't have an account at OpenReview, sign up here:<br>
[https://openreview.net/signup](https://openreview.net/signup){:target="_blank"}<br>
*Please use your KAIST email address.*

- A submission must include a *report*, a *poster*, and a *code repository link*. (Supplementary materials are optional.)
- Submission with the *wrong format* or any *missing items* may receive a *zero* score.
- Make a submission for each *team* (not for each person). Add all the team members' names in the submission.
- *Development Track:* Make the *title* to be the *same* as the original paper.
- In the OpenReview webpage, the deadline ie written as `Jun 06 2021 02:59PM UTC-0)`, which is the same as *Jun 06 (Sun), 23:59 KST*.
- Even in the case when OpenReview does not block the submission after the deadline (due to some system errors), *any submissions after the deadline will be rejected*.


#### Report Guidelines

<b>Format</b>
- A *single PDF* file (maximum 20MB). Supplementary materials are allowed.
- Must be in *CVPR* format:<br>
[LaTeX/Word Templates Zip file (CVPR 2021 format)](http://cvpr2021.thecvf.com/sites/default/files/2020-09/cvpr2021AuthorKit_2.zip){:target="_blank"}<br>
[Overleaf template (CVPR 2018 format)](https://www.overleaf.com/latex/templates/cvpr-2018-template/qgmrfntfbqns){:target="_blank"}
- Add the *project type* (Development Track / Research Track) in the *second line* of the report title. Using LaTex, you can add like this: `\title{Project Title \\ {Development/Research} Track}`.
- Must be up to *four* pages long, including figures, tables, and acknowledgments, but not references. Additional pages containing only cited references are allowed.

<h><b>Structure</b></h>
Please use the *same section names* below to facilitate the review process.<br>
Additional sections/subsections are allowed. Also, the detailed instructions in each section are *recommendations*, and *you do NOT need to exactly follow them*, except for the <h>highlighted</h> parts.<br>
The review will be *single-blind*. Add *author names* in the report (*uncomment* `\cvprfinalcopy` in the CVPR template).

<h><b>[Development Track]</b></h><br>

- <h><em>DO NOT COPY the texts or figures in the original paper (except for qualitative result figures) — it will be considered plagiarism.</em></h> Write the report in your own words. It is allowed to *use qualitative result figures* in the original paper for comparisons (actually *highly recommended*), but *clearly mention* that the figures are from the original paper.
- <h><em>Make the title to be the same as the original paper.</em></h><br>

- <b>Abstract</b>
    - one-sentence *TL;DR*,
    - 2-3 sentences for the *motivation* and *key ideas* of the *original work* <h><em>(add a citation)</em></h>,
    - a few sentences summary of the *implementation challenges* and *your approaches*, and
    - 1-2 sentences summary of the *experimental results*.
    - In the end, add *“Code is available at: {link}.”*

- <b>Introduction</b>
    - What is the *motivation* of the (original) work? Why is it important to solve the problem? What would be the potential impacts of this work in the research field, or what would be the potential applications?
    - What is the *problem setup* the original work introduce? (Add a citation of the original work.)  What are the input and desired output? What are the given information in the training time and the given assumptions? What are the *main ideas* of the original work to solve the problem?
    - What are the *key challenges* in implementing the proposed method? Does the framework include some components that are not implemented in public libraries (e.g., PyTorch, PyTorch3D)? Do you implement some components from scratch without the public libraries? (Using CUDA?) Is the framework complicated with lots of components? Are there technical details hidden in the paper/code? Doesn't the authors provide their code or datasets? Does the authors' code even not reproduce the results in the paper? Is the network training tricky or unstable? Or, do you improve the original work?
    - Summarize the *implementation details*. *Clearly differentiate* the parts you implemented and the parts you borrowed existing code or got some help from the external collaborators. How do you implement each part, and how do you handle the challenges? A *teaser* figure that illustrates the parts you focused on in the implementation would be great.
    - Briefly describe the *experimental setups*. Which datasets/benchmarks do you use? How do you evaluate the results? Do you make any changes in the experimental setups of the original work? If yes, why? How good are your results compared with the results reported in the original paper (or the results of the authors' code)? Do you improve the original method, or do you conduct additional experiments not shown in the original work?
    - A *summary of achievements* at the end is also recommended (in a bullet point list). You can start the summary with (for example) ‘In summary, our achievements are:’.

- <b>Method Summary</b>
    - Describe the *problem setup* again, but in detail and also in a formal way. Introduce essential math notations for the following formulations. <h><em>DO NOT COPY the texts or figures in the original paper</em></h>, but use the *same math notations* in the original work.
    - Briefly *summarize* the method proposed in the original work, while focusing on the parts that you implemented (if you used existing codes for some parts). The report needs to be *self-contained*; the readers must be able to understand the main ideas of the original work without reading the paper.


- <b> Implementation Details</b>
    - First, briefly but clearly state *which parts you implemented* in the framework. If you used some existing codes, describe in detail *how you also adopted the existing codes*. Add *references* for the existing codes. <h><em>Hiding the use of existing codes will be considered plagiarism</em></h>.
    - *Data generation/preprocessing* and *evaluations* are also parts of the implementation. If you implemented these yourself, illustrate the details.
    - Consider as you explain the implementation details to help readers reproduce the results (like providing a *recipe in cooking*). Make the exposition *easy to follow*, but also *clear* and *specific* as much as possible.
    - Use *visual aids* in your exposition. More would be better. But <h><em>DO NOT COPY figures in the original paper.</em></h> Formulations are fine (but do not copy and paste an image but write them yourself).

- <b>Experimental Results</b>
    - Clearly describe the *experiment setups*, including *benchmarks/datasets* and *evaluation metrics*. If you change or simplify the experimental setups of the original work, explain why.
    - Provide *comparisons* with the original work. Use the *exact results* reported in the original paper for comparison. If you test the authors' code in new datasets, explain why. Provide both *quantitative results (tables)* and *qualitative results (figures)*. Explain in which aspects the results of your method is better or comparable.
    - Try to reproduce *all the results* in the original paper. Any *lack of experiments, evaluations, or comparisons* (without any appropriate reasons) will be penalized in the evaluation.
    - Make *fair and reasonable* (apples-to-apples) comparisons. Unfair benefits to your implementation in the experiments will also be penalized.
    - If you achieve *better performance* than the original work, if you *improve* the proposed algorithm, or if you conduct some *additional experiments* not performed in the original paper, *emphasize* the results.
    - In here or in the conclusion, consider showing some *remarkable failure cases* explaining the limitation of the proposed method or your implementation, or motivating some future works.

- <b>Conclusion</b>
    - Briefly *summarize* the project, particularly the main parts you implemented and the experimental results.
    - Describe the *limitation* of the proposed work or your implementation and *potential future research directions* (if you have space in the report).

- <b>Acknowledgments</b>
    - Make acknowledgments as a subsection without a section number or as a paragraph.
    - <h>Describe the <em>role</em> of each team member and the <em>external collaborators</em> and their contributions.</h>
    - <h><em>Hiding the external collaborators will be considered academic misconduct.</em></h>
    - <h><em>Acknowledgments section is required</em>, even when you do not have the other team member, external collaborators, or any data/codes you borrowed from the other places (state the fact).</h>


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
    - Briefly describe the *experimental setups*. Which datasets/benchmarks do you use? How do you evaluate the results? What is the conclusion? (E.g. our method outperformed SotA methods by huge margins.)
    - *A summary of contributions* at the end is also recommended (in a bullet point list). You can start the summary with (for example) 'In summary, our contributions are:'.
- <b>Related Work</b>:
    - Consider making *two or three* groups of related papers and writing a short paragraph for each of them, which a *paragraph title*. E.g., if your project is about '3D GAN', you can consider groups of 'Deep Learning for 3D Data' and 'Deep Generative Models'. Also, an intro sentence briefly describing the groups is recommended (but not necessary).
    - Summarize each work with 1-2 sentences while focusing on describing in which aspects your work is *different* or *overcoming the limitations*.

- <b>Method</b>
    - Describe the *problem setup* again, but in detail and also in a formal way. Introduce *essential math notations* for the following formulations. A *figure* describing the overall method is recommended.
    - The report needs to be *self-contained*; the readers must be able to understand the ideas without reading the other papers. If needed, provide *background knowledge* (the 'minimal' background to understand your work).
    - Think about the most effective way to explain the *key ideas*. One option would be *prioritizing* components in your method not based on the order in the method but based on the *importance*. Less important details can go to the end or to the supplementary.
    - Use *visual aids* in your exposition. More would be better.
    - Make the exposition as *clear* and *specific* as possible. *Formulations* can make the exposition clearer and more concise.
- <b>Experimental Results</b>:
    - Clearly describe the *experiment setups*, including *benchmarks/datasets*, *evaluation metrics*, and *baseline methods*.
    - Provide both *quantitative results (tables)* and *qualitative results (figures)*. Provide *comparisons* with the baseline methods. Explain in which aspects your method is better. Think about the best way to demonstrate the advantages of your method over the baseline methods.
    - Conduct the *ablation study* and show the results. If you have multiple technical contributions, demonstrate how each component affects the results.
    - *Do not miss* any well-known benchmarks/datasets, standard evaluation metrics, or previous methods. Any *lack of experiments, evaluations, or comparisons* will be penalized in the evaluation.
    - Make *fair and reasonable* (apples-to-apples) comparisons. (Or, if the baseline methods take some advantages such as stronger supervision, describe clearly.) Unfair benefits to the proposed method in the experiments will also be penalized.
    - In here or in the conclusion, consider showing some *remarkable failure cases* explaining the limitation of the proposed method or motivating some future works.

- <b>Conclusion</b>
    - Briefly *summarize* the project, particularly the *key ideas* and the *experimental results*.
    - Describe the *limitation* of the proposed work and *potential future research* directions (if you have space in the report).

- <b>Acknowledgments</b>
    - Make acknowledgments as a subsection without a section number or as a paragraph.
    - <h>Describe the <em>role</em> of each team member and the <em>external collaborators</em> and their contributions.</h>
    - <h><em>Hiding the external collaborators will be considered academic misconduct.</em></h>
    - <h><em>Acknowledgments section is required</em>, even when you do not have the other team member, external collaborators, or any data/codes you borrowed from the other places (state the fact).</h>


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
- <h>All the results shown in the report must be replicable with your code.</h> In the code repository, provide *links of the pretrained models* (stored in Google Drive or any other places) and also *datasets you created*, so that anyone can easily check the replicability.


#### Supplementary Materials

- Supplementary materials are optional.
- Any formats (PDF document, video, web page) are allowed (maximum 100MB).
- Submit as a *ZIP* file.

#### <h>Plagiarism / Academic Misconduct</h>
*Plagiarism consists of appropriating someone else's ideas or any texts, figures, or results of the other work, without sharing credit or correctly citing or mentioning the work.
If plagiarism or other academic misconduct is discovered in your submission (in any of your report, poster, code, or supplementary), you will receive an F grade, and also it will be reported to the university.*


<br>
[Back to top](#)
<br>

---

<div id='review-guidelines'/>
### 4. Review Guidelines

- You will be asked to review *four* projects, and each project will be reviewed by *at least four* peer reviewers.
- The review will be *single-blind* and will be performed in *OpenReview*.<br>
(Both the submissions and reviews will NOT be open to the public.)
- Reviews can be *rejected* based on the assessment of the review quality.
- Each *unsubmitted* or *rejected* review will be *penalized by 20%* in the project evaluation.


<div id='infeasible-experiments'/>
#### Infeasible Experiments

In the report, you can argue the *infeasibility* of experiments that are expected to be shown in the results.
For example,
- Some experiments in the original work (Development Track) may not be reproducible if the experiments require multiple GPUs or too large disk/memory spaces *(note that only one GPU is provided to each student)* or some important details in the experiment are missing.
- An exact comparison with the original work (Development Track) or previous work (Research Track) may not be possible when the data used in the experiment is not released.

For such infeasible experiments, the authors must consider *substituting* them with similar but feasible experiments (or, also argue why it is even not possible to substitute them).
For example,
- If an experiment is computationally infeasible, try to simplify the experiment (use a smaller dataset, use a simplified neural network, reduce the batch size, etc).
- If data for replication is not provided, consider using the other similar data.
- If some experiment details for replication are not provided, use any common parameters or approaches.

As a *reviewer*, you need to judge whether the argument about infeasibility is valid or not and whether the authors tried to substitute the infeasible experiments.

For the experiments considered infeasible, do not take them into account in the evaluation.


<br>
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
*(Refer to the guidelines about "<a href="{{site.baseurl}}/{{page.path}}/../../project-submission-guidelines.html#infeasible-experiments">Infeasible Experiments</a>" before answering this question.)*<br>
- Extensive, detailed, and informative evaluations without any missing benchmarks/datasets, evaluation metric, and comparison.
- Solid and sufficient to convince the merits of the proposed method (Research) or the performance of the implementation (Development) (although lacking some minor experiments or simplifying the experiment setup a bit.)
- Lacking some important experiments (in terms of benchmarks/datasets, evaluation metrics, comparisons, quantitative/qualitative results, etc).
- Insufficient, unfair, inadequate, or uninformative comparisons with related work  (Research) or the original work (Development).


<b>[Development] (Reproduction) Do the implementation reproduce the results in the original work?</b><br>
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

<br>
[Back to top](#)

<br/>

