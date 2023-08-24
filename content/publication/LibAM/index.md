---
title: "LibAM: An Area Matching Framework for Detecting Third-party Libraries in Binaries"
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
date: "2023-09-20T00:00:00.000Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2023-08-24T00:00:00.000Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: "ACM Transactions on Software Engineering and Methodology"
publication_short: "ToSEM (CCF-A)"

abstract: "Third-party libraries (TPLs) are extensively utilized by developers to expedite the software development process and incorporate external functionalities. Nevertheless, insecure TPL reuse can lead to significant security risks. Existing methods, which involve extracting strings or conducting function matching, are employed to determine the presence of TPL code in the target binary. However, these methods often yield unsatisfactory results due to the recurrence of strings and the presence of numerous similar non-homologous functions. Furthermore, the variation in C/C++ binaries across different optimization options and architectures exacerbates the problem. Additionally, existing approaches struggle to identify specific pieces of reused code in the target binary, complicating the detection of complex reuse relationships and impeding downstream tasks. And we call this issue the poor interpretability of TPL detection results.

In this paper, we observe that TPL reuse typically involves not just isolated functions but also areas encompassing several adjacent functions on the Function Call Graph (FCG). We introduce LibAM, a novel Area Matching framework that connects isolated functions into function areas on FCG and detects TPLs by comparing the similarity of these function areas, significantly mitigating the impact of different optimization options and architectures. Furthermore, LibAM is the first approach capable of detecting the exact reuse areas on FCG and offering substantial benefits for downstream tasks. To validate our approach, we compile the first TPL detection dataset for C/C++ binaries across various optimization options and architectures. Experimental results demonstrate that LibAM outperforms all existing TPL detection methods and provides interpretable evidence for TPL detection results by identifying exact reuse areas. We also evaluate LibAM’s scalability on large-scale, real-world binaries in IoT firmware and generate a list of potential vulnerabilities for these devices. Our experiments indicate that Area Matching framework performs exceptionally well in the TPL detection task and holds promise for other binary similarity analysis tasks. Last but not least, by analyzing the detection results of IoT firmware, we make several interesting findings, for instance, different target binaries always tend to reuse the same code area of TPL."


# Summary. An optional shortened abstract.
summary: LibAM is the first approach capable of detecting the exact reuse areas on FCG and offering substantial benefits for downstream tasks, as well as evaluating LibAM's accuracy on large-scale, real-world binaries in IoT firmware and generating a list of potential vulnerabilities for these devices.

tags: []
featured: false

# links:
# - name: ""
#   url: ""
url_pdf: "https://gentlecp.com/publication/LibAM/2305.04026v2.pdf"
url_code: 'https://github.com/Siyuan-Li201/LibAM'
url_dataset: 'https://github.com/Siyuan-Li201/LibAM/tree/main/dataset'
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'The workflow of LibAM'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
---

