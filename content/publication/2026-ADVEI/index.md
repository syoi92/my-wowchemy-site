---
title: "Rethinking Point Sampling for 3D Semantic Segmentation: An Incidence-Aware Approach to Construction LiDAR"
authors:
- Admin
- Jingdao Chen
- Yong Kwon Cho
date: 2026-08-01T17:07:57+09:00
doi: ""
draft: false

# Schedule page publish date (NOT publication's date).
publishDate: 2026-08-01T17:07:57+09:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: Advanced Engineering Informatics
# publication_short: In *STC*

abstract: "3D scene understanding is increasingly important for construction applications, yet curated datasets often underrepresent actual site sensing conditions. Partially observed scans exhibit acquisition-driven density variation and severe class imbalance, making point allocation critical to balancing geometric detail and spatial context under computational constraints. This study introduces incidence-aware sampling to normalize surface point allocation using incidence angle, reducing redundancy on densely observed surfaces while preserving sparse evidence at grazing angles. Experiments on the Site in Pieces benchmark using Point Transformer and PointNeXt show improved resolution-averaged performance and reduced sensitivity to sampling resolution. For Point Transformer, resolution-averaged mean intersection over union improves by 4.7 percentage points overall, with gains of 8.1 points for slender construction elements and 16.3 points for ladders. Among the evaluated geometry-aware sampling methods, the proposed pipeline achieves the highest mean intersection over union for these elements while reducing total inference time by 69–76% relative to the alternatives. It also achieves comparable overall mean intersection over union to Point Transformer V3 with approximately 83% fewer trainable parameters, with an additional inference cost of approximately 0.7 s/Mpts. Additional experiments on Rohbau3D and Semantic3D show segmentation improvements of varying magnitude. These results support incidence-aware sampling as a practical approach to preserving sparse construction evidence when the scanner origin is known, with potential benefits for local site assessment and incremental updates to digital representations."
# Summary. An optional shortened abstract.
summary: "Keywords: 3D semantic segmentation; Terrestrial laser scanning; Point cloud sampling; Construction monitoring  


*Advanced Engineering Informatics*, Under Review"

tags: []
categories: []
featured: true

links:
- name: arXiv
  url: https://arxiv.org/abs/2608.07757
- name: GitHub
  url: https://github.com/syoi92/Pointcept-SIP
# - name: pdf
#   url: 'media/2020-CPENG/(ASCE)CP.1943-5487.0000942.pdf'
# url_pdf: http://eprints.soton.ac.uk/352095/1/Cushen-IMV2013.pdf
# url_code: '#'
# url_dataset: '#'
# url_poster: '#'
# url_project: ''
# url_slides: ''
# url_source: '#'
# url_video: '#'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
# image:
#  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
#  focal_point: ""
#  preview_only: false

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
#   Otherwise, set `#slides: ""`.
# slides: example
---
