---
title: "LibAM: An Area Matching Framework for Detecting Third-party Libraries in
  Binaries"
publication_types:
  - "2"
authors:
  - Siyuan Li
  - Yongpan Wang
  - admin
  - Shouguo Yang
  - Hong Li
  - Hao Sun
  - Zhe Lang
  - Zuxin Chen
  - Weijie Wang
  - Hongsong Zhu
  - Limin Sun
author_notes:
  - ""
publication: ACM Transactions on Software Engineering and Methodology
publication_short: ToSEM (CCF-A)
abstract: >-
  Third-party libraries (TPLs) are extensively utilized by developers to
  expedite the software development process and incorporate

  external functionalities. Nevertheless, insecure TPL reuse can lead to significant security risks. Existing methods, which involve

  extracting strings or conducting function matching, are employed to determine the presence of TPL code in the target binary. However,

  these methods often yield unsatisfactory results due to the recurrence of strings and the presence of numerous similar non-homologous

  functions. Furthermore, the variation in C/C++ binaries across different optimization options and architectures exacerbates the problem.

  Additionally, existing approaches struggle to identify specific pieces of reused code in the target binary, complicating the detection of

  complex reuse relationships and impeding downstream tasks. And we call this issue the poor interpretability of TPL detection results.

  In this paper, we observe that TPL reuse typically involves not just isolated functions but also areas encompassing several adjacent

  functions on the Function Call Graph (FCG). We introduce LibAM, a novel Area Matching framework that connects isolated functions

  into function areas on FCG and detects TPLs by comparing the similarity of these function areas, significantly mitigating the impact of

  different optimization options and architectures. Furthermore, LibAM is the first approach capable of detecting the exact reuse areas

  on FCG and offering substantial benefits for downstream tasks. To validate our approach, we compile the first TPL detection dataset

  for C/C++ binaries across various optimization options and architectures. Experimental results demonstrate that LibAM outperforms

  all existing TPL detection methods and provides interpretable evidence for TPL detection results by identifying exact reuse areas. We

  also evaluate LibAM’s scalability on large-scale, real-world binaries in IoT firmware and generate a list of potential vulnerabilities for

  these devices. Our experiments indicate that Area Matching framework performs exceptionally well in the TPL detection task and

  holds promise for other binary similarity analysis tasks. Last but not least, by analyzing the detection results of IoT firmware, we make

  several interesting findings, for instance, different target binaries always tend to reuse the same code area of TPL. The datasets and

  source code used in this paper are available at https://github.com/Siyuan-Li201/LibAM
draft: false
featured: false
image:
  filename: ""
  focal_point: Smart
  preview_only: false
  caption: "Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)"
date: 2023-08-24T05:50:11.869Z
---

{{% callout note %}}
Click the _Cite_ button above to demo the feature to enable visitors to import publication metadata into their reference management software.
{{% /callout %}}

{{% callout note %}}
Create your slides in Markdown - click the _Slides_ button to check out the example.
{{% /callout %}}

Supplementary notes can be added here, including [code, math, and images](https://wowchemy.com/docs/writing-markdown-latex/).
