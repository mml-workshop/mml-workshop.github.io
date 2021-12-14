---
layout: default
title: "The 1st Multilingual Multimodal Learning Workshop"
permalink: /

speakers:
  - name: Preethi Jyothi
    url: https://www.cse.iitb.ac.in/~pjyothi/
    topic: TBA
    aff: IIT Bombay
    interest: TBA
    image: /assets/images/preethi.png

  - name: Lei Ji
    url: https://www.microsoft.com/en-us/research/people/leiji/
    topic: TBA
    aff: Microsoft Research Asia
    interest: TBA
    image: /assets/images/lei.jpg
  - name: Lisa-Anne Hendricks
    url: https://scholar.google.com/citations?user=pvyI8GkAAAAJ
    topic: TBA
    aff: DeepMind
    interest: TBA
    image: /assets/images/lisa.jpg


Organizers:
  - name: Emanuele Bugliarello (University of Copenhagen)
    url: https://e-bug.github.io
    image: assets/images/test.jpeg

  - name: Kai-Wei Chang (UCLA)
    url: http://web.cs.ucla.edu/~kwchang/
    image: assets/images/test.jpeg

  - name: Desmond Elliott (University of Copenhagen)
    url: https://elliottd.github.io
    image: assets/images/test.jpeg

  - name: Spandana Gella (Amazon Alexa AI)
    url: https://scholar.google.com/citations?user=fChTW6MAAAAJ
    image: assets/images/test.jpeg

  - name: Aishwarya Kamath (NYU)
    url: https://ashkamath.github.io
    image: assets/images/test.jpeg

  - name: Liunian Harold Li (UCLA)
    url: https://liunian-harold-li.github.io
    image: assets/images/test.jpeg

  - name: Fangyu Liu (Cambridge)
    url: http://fangyuliu.me/about
    image: assets/images/test.jpeg
  
  - name: Jonas Pfeiffer (TU Darmstadt)
    url: https://pfeiffer.ai
    image: assets/images/test.jpeg

  - name: Edoardo M. Ponti (MILA Montreal)
    url: https://ducdauge.github.io
    image: assets/images/test.jpeg

  - name: Krishna Srinivasan (Google Research)
    url: https://krishna2.com/
    image: assets/images/test.jpeg

  - name: Ivan Vulić (Cambridge)
    url: https://sites.google.com/site/ivanvulic/
    image: assets/images/test.jpeg

  - name: Yinfei Yang (Google Research)
    url: https://scholar.google.com/citations?user=kvDbu90AAAAJ
    image: assets/images/test.jpeg

  - name: Da Yin (UCLA)
    url: http://wadeyin9712.github.io
    image: assets/images/test.jpeg


---

# About

Multilingual multimodal research focuses on collecting resources, developing models, and evaluating systems that need to jointly reason over multilingual text and multimodal inputs, including images, videos, texts, and knowledge bases. Multilingual multimodal NLP presents new and unique challenges. First, it is one of the areas that suffer the most from language imbalance issues. Texts in most multimodal datasets are usually only available in high-resource languages. Second, multilingual multimodal research provides opportunities to investigate culture-related phenomena. On top of the language imbalance issue in text-based corpora and models, the data of additional modalities (e.g. images or videos) are mostly collected from North American and Western European sources (and their worldviews). As a result, multimodal models do not capture our world's multicultural diversity and do not generalise to out-of-distribution data from minority cultures. The interplay of the two issues leads to extremely poor performance of multilingual multimodal systems in real-life scenarios. This workshop encourages and promotes research efforts towards more inclusive multimodal technologies and tools to assess them. We invite papers which focus on the topics of interest include (but are not limited to):

- Datasets for multilingual multimodal learning
- Modeling multilingual multimodal Data
- Approaches to improving the inclusion of multilingual multimodal models
- Evaluation and analysis for multilingual multimodal learning
- Future challenges of multilingual multimodal research

## Submission Policy 

The paper submission will be done via [OpenReivew](https://openreview.net/group?id=aclweb.org/ACL/2022/Workshop/MML).

Submitted manuscripts must be 8 pages long for full papers, and 4 pages long for short papers. Both full and short papers can have unlimited pages for references and appendices.  We follow ARR submission guidelines. For more information about templates, guidelines, and instructions, see the [ARR CFP guidelines](https://aclrollingreview.org/cfp). We encourage authors to include a broader impact and ethical concerns statement, following [ARR Ethics Policy](https://aclrollingreview.org/cfp) from the main conference.

All submissions will be double-blind peer-reviewed (with author names and affiliations removed) by the program committee and judged by their relevance to the workshop themes.  

Please note that at least one of the authors of each accepted paper must register for the workshop and present the paper.


## Non-Archival option
ACL workshops are traditionally archival. To allow dual submission of work, we are also including a non-archival track. If accepted, these submissions will still participate and present their work in the workshop. A reference to the paper will be hosted on the workshop website (if desired), but will not be included in the official proceedings. Please submit through OpenReview but indicate that this is a cross-submission at the bottom of the submission form. You can also skip this step and inform us of your non-archival preference after the reviews.

## Shared Task Submission

We will organize a shared task. Papers describing systems that participate in the shared task are welcome to submit to this workshop. Please see the details in a separate call later. 


## Follow Us

TBA

# Invited Talks (In alphabetical order)

{% include team.html id="speakers" %}


# Important Dates 

Important Dates:
- February 28, 2022: Submission Date
- March 26, 2022: Notification of Acceptance
- April 10, 2022: Camera-ready papers due (hard deadline)
- May 26-27, 2022: Workshop on Multimodal Multilingual Learning (M3L2)


# Organizers and Contact

Organizers are in the alphabetical order. For any question, please contact [email address TBA].


<ul>
{% for p in page.Organizers %}
<li>
<a{% if p.url %} href="{{ p.url }}"{% endif %}>{{ p.name }}</a>
</li>
{% endfor %}
</ul>


