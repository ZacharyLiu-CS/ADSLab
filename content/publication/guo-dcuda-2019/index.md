---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: 'DCUDA: Dynamic GPU Scheduling with Live Migration Support'
subtitle: ''
summary: ''
authors:
- Fan Guo
- Yongkun Li
- John C. S. Lui
- Yinlong Xu
tags:
- '"GPU scheduling"'
- '"live migration"'
categories: []
date: '2019-11-01'
lastmod: 2020-09-16T19:06:56+08:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ''
  focal_point: ''
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
publishDate: '2020-09-16T11:06:55.839082Z'
publication_types:
- 1
abstract: In clouds and data centers, GPU servers which consist of multiple GPUs are
  widely deployed. Current state-of-the-art GPU scheduling algorithm are \"static\"
  in assigning applications to different GPUs. These algorithms usually ignore the
  dynamics of the GPU utilization and are often inaccurate in estimating resource
  demand before assigning/running applications, so there is a large opportunity to
  further load balance and to improve GPU utilization. Based on CUDA (Compute Unified
  Device Architecture), we develop a runtime system called DCUDA which supports \"dynamic\"
  scheduling of running applications between multiple GPUs. In particular, DCUDA provides
  a realtime and lightweight method to accurately monitor the resource demand of applications
  and GPU utilization. Furthermore, it provides a universal migration facility to
  migrate \"running applications\" between GPUs with negligible overhead. More importantly,
  DCUDA transparently supports all CUDA applications without changing their source
  codes. Experiments with our prototype system show that DCUDA can reduce 78.3% of
  overloaded time of GPUs on average. As a result, for different workloads consisting
  of a wide range applications we studied, DCUDA can reduce the average execution
  time of applications by up to 42.1%. Furthermore, DCUDA also reduces 13.3% energy
  in the light load scenario.
publication: '*Proceedings of the ACM Symposium on Cloud Computing*'
url_pdf: https://doi.org/10.1145/3357223.3362714
doi: 10.1145/3357223.3362714
---
