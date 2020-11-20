---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Updating Land Category in Cadastral Map Using Hyperspectral UAV"
summary: "Cadastral Map; Discrepancy Analysis; Land Update; Hyperspectral UAV; Land Classificaion; 3D-CNN; Integration Analysis"
authors: []
tags: ["selected", "research"]
categories: ["GIS"]
date: 2020-11-19T14:21:25+09:00

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: "Discrepancy analysis for updating the land category in parcel maps"
  focal_point: ""
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---
***With the perspective of automation, we perform discrepancy analysis for detecting parcels that should be updated using hyperspectral UAV images.***

#
1. An up-to-date land cover map is generated from hyperspectral unmanned aerial vehicle (UAV) images. These images are effectively classified by a hybrid two- and three-dimensional convolutional neural network.
2. A discrepancy map, which contains the ratio of the area that is being used differently from the registered land use in each parcel, is constructed through a three-stage inconsistency comparison. 


The method automatically reveals the inconsistent parcels requiring updates of their land category. Although the performance of the proposed method depends on the classification results obtained from UAV imagery, the method allows a flexible modification of the matching criteria between the land categories and land coverage. Therefore, it is generalizable to various cadastral systems and the discrepancy ratios will provide practical information and significantly reduce the time and effort for land monitoring and field surveying.