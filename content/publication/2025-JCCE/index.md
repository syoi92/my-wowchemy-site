---
title: "SIP: Site in Pieces-A Dataset of Disaggregated Construction-Phase 3D Scans for Semantic Segmentation and Scene Understanding"
authors:
- Admin
- Yong Kwon Cho
date: 2025-08-01T17:07:57+09:00
doi: ""
draft: false

# Schedule page publish date (NOT publication's date).
publishDate: 2025-08-01T17:07:57+09:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: Journal of Computing in Civil Engineering
# publication_short: In *STC*

abstract: "LiDAR has become a core sensing modality in construction due to its ability to reliably capture geometric information in cluttered and dynamic environments. However, most publicly available 3D perception datasets are derived from densely fused scans with near-complete visibility, which differs from practical construction data acquisition. On active construction sites, comprehensive scene reconstruction is often neither feasible nor necessary, and field data are therefore commonly collected as isolated single-station LiDAR scans exhibiting radial density decay and fragmented geometry. These conditions motivate perception methods that operate on partial observations without relying on full scene rescanning or global reconstruction. This paper presents SIP (Sites in Pieces), a dataset designed to preserve the realistic sensing characteristics of construction-phase LiDAR while organizing the data within a construction-specific semantic taxonomy. SIP includes indoor and outdoor LiDAR scenes annotated at the point level and categorized into Built Environment, Construction Operations, and Site Surroundings classes. The dataset covers both permanent structural components and temporary objects such as scaffolding, staged materials, and scissor lifts, which often appear sparse or fragmented and pose segmentation challenges. A standardized scanning protocol, annotation workflow, and quality control process ensure dataset consistency, and the dataset is released openly with a companion utility code repository to facilitate integration into modern 3D deep learning pipelines. By retaining real-world sensing artifacts, SIP enables realistic benchmarking for construction-oriented 3D vision and supports automated site understanding and digital-twin applications."
# Summary. An optional shortened abstract.
summary: "Keywords: Construction Lidar Dataset; 3D Point Cloud; Semantic Segmentation; Digital Twins


*Journal of Computing in Civil Engineering*, In Production"

tags: []
categories: []
featured: true

links:
- name: arXiv
  url: https://arxiv.org/abs/2512.09062
- name: GitHub
  url: https://github.com/syoi92/SIP_dataset/
- name: Zenodo
  url: https://doi.org/10.5281/zenodo.17667735
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
