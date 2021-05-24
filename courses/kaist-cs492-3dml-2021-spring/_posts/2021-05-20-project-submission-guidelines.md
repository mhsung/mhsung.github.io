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

<em>TBA.</em><br>

- Must include a <em>report</em>, a <em>poster</em>, and a <em>code repository link</em>.<br>
- Supplementary materials are optional.
- Submission with the wrong format or any missing items may receive a zero score.


#### Report Guidelines

<b>Format</b>
- A <em>single PDF</em> file (maximum 20MB). Supplementary materials are allowed.
- Must be in <em>CVPR</em> format:<br>
[LaTeX/Word Templates Zip file (CVPR 2021 format)](http://cvpr2021.thecvf.com/sites/default/files/2020-09/cvpr2021AuthorKit_2.zip){:target="_blank"}<br>
[Overleaf template (CVPR 2018 format)](https://www.overleaf.com/latex/templates/cvpr-2018-template/qgmrfntfbqns){:target="_blank"}
- Must be up to <em>four</em> pages long, including figures, tables, and acknowledgments, but not references. Additional pages containing only cited references are allowed.

<h><b>Structure</b></h>
Please use the <em>same section names</em> below to facilitate the review process.<br>
Additional sections/subsections are allowed. Also, the detailed instructions in each section are <em>recommendations</em>, and you do need to exactly follow them.

<em>[Development Track]</em>

<em>TBD.</em><br>


<em>[Research Track]</em>

- <b>Abstract</b><br>
    - one-sentence <em>TL;DR</em>,
    - 1-2 sentences for the <em>motivation</em>,
    - a few sentences summary of the <em>problem statement and key contributions</em>, and
    - 1-2 sentences summary of the <em>experimental results</em>.
    - At the end, add <em>"Code is available at: {link}."</em>
- <b>Introduction</b>
    - What is the <em>motivation</em> of the work? Why is it important to solve the problem? What would be the potential impacts of this work in the research field, or what would be the potential applications?
    - What are the <em>challenges</em> in the problem? How has previous work approached this problem, and what are the limitations (add citations)? Or, why hasn't the problem been addressed while it is important?
    - What is the <em>problem statement</em>? What are the input and desired output? What are the given information in the training time and the given assumptions? A <em>teaser figure</em> that effectively illustrates the problem setup or the desired output would be great. (E.g., show the best result with the input.)
    - What are your <em>key ideas</em> for solving the challenges? It would be also great if your teaser image also describes the key ideas. (E.g. how do your key ideas make differences in the results?)
    - Briefly describe the <em>experimental setups</em>. Which datasets/benchmarks did you use? How did you evaluate the results? What is the conclusion? (E.g. our method outperformed SotA methods by huge margins.)
    - <em>A summary of contributions</em> at the end is also recommended (in a bullet point list). You can start the summary with (for example) 'In summary, our contributions are:'.
- <b>Related Work</b>:
    - Consider making <em>two or three</em> groups of related papers and writing a short paragraph for each of them, which a <em>paragraph title</em>. Also, an intro sentence briefly describing the groups is recommended (but not necessary). E.g., if your project is about '3D GAN', you can consider groups of 'Deep Learning for 3D Data' and 'Deep Generative Models'.
    - Summarize each work with 1-2 sentences while focusing on describing in which aspects your work is <em>different</em> or <em>overcoming the limitations</em>.

- <b>Method</b>
    - First describe the <em>problem setup</em> again, but in detail and also in a formal way. Introduce <em>essential math notations</em> for the following formulations. A <em>figure</em> describing the overall method is recommended.
    - The report needs to be <em>self-contained</em>; the readers must be able to understand the ideas without reading the other papers. Provide <em>background knowledge</em> if needed (not necessary). If needed, provided the 'minimal' background to understand your work.
    - Think about the most effective way of explaining the <em>key ideas</em>. One option would be <em>prioritizing</em> components in your method not based on the order in the method but based on the <em>importance</em>. Less important details can go to the end or to the supplementary.
    - Use <em>visual aids</em> in your exposition. More would be better.
    - Make the exposition as <em>clear</em> and <em>specific</em> as possible. <em>Formulations</em> can make the exposition clearer and more concise.
- <b>Experimental Results</b>:
    - Clearly describe the <em>experiment setups</em>, including <em>benchmarks/datasets</em>, <em>evaluation metrics</em>, and <em>baseline methods</em>.
    - Provide both <em>quantitative results (tables)</em> and <em>qualitative results (figures)</em>. Provide <em>comparisons</em> with the baseline methods. Explain in which aspects your method is better. Think about the best way to demonstrate the advantages of your method over the baseline methods.
    - <em>Do not miss</em> any well-known benchmarks/datasets, standard evaluation metrics, or previous methods. Any <em>lack of experiments, evaluations, or comparisons will be penalized</em> in the evaluation.
    - In here or in the conclusion, consider showing some 'meaningful' <em>failure cases</em> that can explain the limitation of the proposed method and can motivate some future works.

- <b>Conclusion</b>
    - Briefly summarize the project, particularly the key ideas and the experimental results.
    - Describe the limitation of the proposed work and potential future research directions (if you have space in the report).

- <b>Acknowledgments</b>
    - Make it as a subsection (without a section number) or a paragraph.
    - Describe the role of each team member and the external collaborators and their contributions.


#### Poster Guidelines

<b>Format</b>
- A <em>single PNG</em> file (maximum 3MB).
- Must have <em>2560x1280</em> resolution.
- Poster template: [<b>Link</b>](https://kaistackr-my.sharepoint.com/:p:/g/personal/mhsung_kaist_ac_kr/EQz68whVxahPoGdcBExRSqIBhcbldxFCXE9p-otheEmCTg?e=VF2sNi){:target="_blank"} (Design adapted from [Zoya Bylinskii](https://web.mit.edu/zoya/www/docs.html){:target="_blank"})<br>
Do not need to use this template.
- Must include <em>project title</em>, <em>project track</em>, <em>team member names</em>, and <em>acknowledgments</em>.


<b>Resources</b>
- [<b>How to Make a More Effiective Research Poster (Zoya Bylinskii)</b>](https://web.mit.edu/zoya/www/posterRecommendations.pdf){:target="_blank"}


#### Code Submission
- Create a <em>public code repository</em> in GitHub or Bitbucket and submit the link.
- Also, add the link in the <em>abstract</em> of the report (see [Report Guidelines](#report-guidelines)).


#### Supplementary Materials

- Supplementary materials are optional.
- Any formats (PDF document, video, web page) are allowed (maximum 100MB).
- Submit as a <em>ZIP</em> file.

#### Plagiarism
Plagiarism consists of appropriating the words or results of another, without credit. if plagiarism is found in your report, poster, or code, you will receive an F grade, and also it will be reported to the university.


[Back to top](#)
<br>

---

<div id='poster-sessions'/>
### 3. Poster Sessions (Virtual)

<em>TBA.</em><br>

We'll use [Gather.town](https://gather.town/){:target="_blank"}.


[Back to top](#)
<br>

---

<div id='review-guidelines'/>
### 4. Review Guidelines

<em>TBA.</em><br>

- Each project will be reviewed by <em>four</em> peer reviewers.
- The review will be <em>single-blind</em> and will be performed in <em>OpenReview</em>.<br>
(Both the submissions and reviews will NOT be open to the public.)
- Reviews can be <em>rejected</em> based on the assessment of the review quality.
- Each <em>unsubmitted</em> or <em>rejected</em> review will be <em>penalized by 20%</em> in the project evaluation.


[Back to top](#)
<br>

---

<div id='review-questions'/>
### 5. Review Questions

#### <h>Project Summary</h>

<b>Please summarize the project idea in your own words (3+ sentences).</b><br>
<em>Please read the report thoroughly. Your review can be rejected based on the assessment of the review quality. Each unsubmitted or rejected review will be penalized by 20% in the project evaluation.</em><br>


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
<em>Please be constructive, respectful, and detailed in your comments.</em><br>


<b>[All] (Feedback) Provide questions or comments to the submitters if you have.</b><br>


<b>[All] (Overall Score) Please provide an "overall score" for this submission (in [1-5] range).</b><br>
<br>


#### <h>Scoring Criteria</h>

<em>Criteria of score 4 (‘Great!’) (AND conditions)</em><br>
- [All] <b>(Report Writing)</b> The report is well-organized and clearly written.
- [All] <b>(Experiment Designs)</b> The experiments are well-designed and convincing.
- [Development] <b>(Experimental Results)</b> Achieved similar results in a challenging development task with the original or improved/outperformed the original work in a doable task.
- [Research] <b>(Experimental Results)</b> Achieved promising results. Worth pursuing the direction for future paper publication (although not ready for now).
- [All] <b>(Etc)</b> No significant flaws in the report writing, experimental result demonstration, and poster presentation.

<em>Criteria of score 5 (‘Outstanding!’)</em><br>
- Better than ‘Great!’. Probably the best project in the class.

<em>Criteria of score 3 (‘Good!’)</em><br>
- Has one significant reason not to be ‘Great!’.

<em>Criteria of score 2 (‘Not Good’) (OR conditions)</em><br>
- Has two significant reasons not to be ‘Great!’.
- Shows poor experimenal designs or experimental results or technical contributions (while everything else is ok).

<em>Criteria of score 1 (‘Poor’) (OR conditions)</em><br>
- Has three or more significant reasons not to be ‘Great!’.
- Shows poor experimental designs or experimental results or technical contributions, and has one more significant reason not to be ‘Great!’.

[Back to top](#)

<br/>

