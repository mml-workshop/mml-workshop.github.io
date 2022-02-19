---
layout: default
title: "Workshop on Multilingual Multimodal Learning"
permalink: /shared_task
---


## MML 2022 Shared Task

The multilingual multimodal learning (MML) workshop, co-located at ACL 2022, is hosting a shared task on multilingual visually grounded reasoning. The task will be centred around the MaRVL dataset, introduced by [Liu & Bugliarello et al. (EMNLP 2021)](https://marvl-challenge.github.io). This dataset extends the NLVR2 task [(Suhr et al., ACL 2019)](https://lil.nlp.cornell.edu/nlvr/) to multicultural and multilingual (Indonesian, Mandarin, Swahili, Tamil, Turkish) inputs: Given two images and a textual description, a system needs to predict whether the description applies to both images (True/False).

The standard setup consists of fine-tuning a multilingual vision-and-language model in the English NLVR2 dataset and then evaluating on MaRVL. We consider two subtasks, as detailed below: zero-shot transfer and few-shot transfer. Both setups have been shown to be challenging [(Bugliarello et al., 2022)](https://iglue-benchmark.github.io), and we look forward to seeing your approaches to the tasks!

Participants will be invited to describe their system in a paper for the MML workshop proceedings. The task organisers will write an overview paper that describes the task and summarises the different approaches taken, and analyses their results.



### Important Links
Here are the links to quickly download the data for the shared task:
* NLVR2: [text](https://github.com/e-bug/iglue/tree/main/datasets/nlvr2/annotations) / [images](https://github.com/lil-lab/nlvr/tree/master/nlvr2#direct-image-download) / [features](https://sid.erda.dk/sharelink/FjJUsFbRWO)
* MaRVL zero-shot: [text](https://github.com/e-bug/iglue/tree/main/datasets/marvl/zero_shot) / [images](https://dataverse.scholarsportal.info/dataset.xhtml?persistentId=doi:10.5683/SP3/42VZ4P) / [features](https://sid.erda.dk/sharelink/fMNmRmJgQA)
* MaRVL few-shot: [text](https://github.com/e-bug/iglue/tree/main/datasets/marvl/few_shot/annotations) / [images](https://dataverse.scholarsportal.info/dataset.xhtml?persistentId=doi:10.5683/SP3/42VZ4P) / [features](https://sid.erda.dk/sharelink/fMNmRmJgQA)
* [IGLUE repository](https://github.com/e-bug/iglue)

Preprocessed image features are available for two visual encoders:
- `*boxes36`: 36 RoIs per image extracted with a Faster R-CNN with a ResNet-101
- `*X101`: 10-100 RoIs per image extracted with a Faster R-CNN with a ResNeXt-101

The IGLUE repository contains sample code and pretrained models to help you get started. Open issues on GitHub or reach out to us for any doubts.

### Important Dates
- Submission Due: April 30 2022 (11:59pm AoE)
- Notification: May 7 2022 (11:59pm AoE)
- Camera-ready Due: May 14 2022 (11:59pm AoE)
- Workshop: 27 May 2022

### Subtasks
The shared task will consist of two subtasks:
- ZS) Zero-shot transfer: Models are fine-tuned on the English NLVR2 data, and tested on MaRVL Indonesian, Mandarin, Swahili, Tamil, Turkish
- FS) few-shot transfer: Models are further fine-tuned on a few data points in the target language. This subtask corresponds to the most-shot setup of [Bugliarello et al. (2022)](https://iglue-benchmark.github.io/). In particular, performance is only reported in three languages: Indonesian, Mandarin and Turkish.

NB: we will *only* consider submissions that use pre-existing pre-trained models that are publicly available or new models that have been (pre)trained on publicly available data.

“Translate test” methods are accepted but will be ranked separately. 

#### The MaRVL Benchmark

We list existing baseline results for the subtasks below. The numbers are copied from the IGLUE benchmark [(Bugliarello et al., 2022)](https://iglue-benchmark.github.io) and is average of the five languages.


##### **_ZS results:_**

| Rank | Model   | Accuracy (%) |
|:------:|---------|:------------:|
|   1  | UC2 [(Zhou et al., 2021)](https://arxiv.org/abs/2104.00332)     |     57.28    |
|   2  | M3P [(Ni et al., 2021)](https://arxiv.org/pdf/2006.02635.pdf)    |     56.00    |
|   3  | xUNITER [(Liu & Bugliarello et al., 2021)](https://aclanthology.org/2021.emnlp-main.818.pdf) |     54.59    |
|   4  | mUNITER [(Liu & Bugliarello et al., 2021)](https://aclanthology.org/2021.emnlp-main.818.pdf) |     53.72    |

##### **_FS results:_**

| Rank | Model   | Accuracy (%) |
|:------:|---------|:--------------:|
|   1  | UC2 [(Zhou et al., 2021)](https://arxiv.org/abs/2104.00332)     |      58.32    |
|   2  | xUNITER [(Liu & Bugliarello et al., 2021)](https://aclanthology.org/2021.emnlp-main.818.pdf) |      57.46    |
|   3  | mUNITER [(Liu & Bugliarello et al., 2021)](https://aclanthology.org/2021.emnlp-main.818.pdf) |      53.41    |
|   4  | M3P [(Ni et al., 2021)](https://arxiv.org/pdf/2006.02635.pdf)     |      49.79    |

<br>

### Submission
Submissions should be emailed to the organisers by the end of April 30, anywhere on Earth.
Submissions need to follow the jsonlines format, where languages are in ISO 639-2 codes:
```
{"concept": "39-Panci", "language": "id", "chapter": "Basic actions and technology", "id": "id-0", "prediction": true}
```
Files should be named as `{team-name}_{zs/ms}_{xl/tt}_{lang}.jsonl` to indicate the subtask (zero-shot or few-shot), whether it’s cross-lingual or translate-test transfer, and the target language.

### Description Papers
Papers describing shared task submissions should consist of 4 to 8 pages of content plus additional pages of references, formatted according to the ARR format guidelines for ACL 2022. For shared task paper submission, it is not necessary to blind the team name and authors. Accepted papers will be published online in the ACL 2022 proceedings and will be presented at the MML workshop at ACL 2022. Writeups should be submitted through [OpenReview](https://openreview.net/group/edit?id=aclweb.org/ACL/2022/Workshop/MML), and are due by 30 April 2022 11:59pm [UTC-12h].


### Contact
Please contact [mml DOT wksp AT gmail DOT com](mailto:mml.wksp@gmail.com) if you have any questions.



