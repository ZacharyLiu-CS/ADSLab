---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: 'HP-Mapper: A High Performance Storage Driver for Docker Containers'
subtitle: ''
summary: ''
authors:
- Fan Guo
- Yongkun Li
- Min Lv
- Yinlong Xu
- John C. S. Lui
tags:
- '"Docker containers"'
- '"I/O performance"'
- '"storage drivers"'
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
publishDate: '2020-09-16T11:06:56.167232Z'
publication_types:
- 1
abstract: Docker containers are widely deployed to provide lightweight virtualization,
  and they have many desirable features such as ease of deployment and near bare-metal
  performance. However, both the performance and cache efficiency of containers are
  still limited by their storage drivers due to the coarse-grained copy-on-write operations,
  and the large amount of redundancy in both I/O requests and page cache. To improve
  I/O performance and cache efficiency of containers, we develop HP-Mapper, a high
  performance storage driver for Docker containers. HP-Mapper provides a two-level
  mapping strategy to support fine-grained copy-on-write with low overhead, and an
  efficient interception method to reduce redundant I/Os. Furthermore, it uses a novel
  cache management mechanism to reduce duplicate cached data. Experiment results with
  our prototype system show that HP-Mapper significantly reduces copy-on-write latency
  due to its finer-grained copy-on-write scheme. Moreover, HP-Mapper can also reduce
  65.4% cache usage on average due to elimination of duplicated data. As a result,
  HP-Mapper improves the throughput of real-world workloads by up to 39.4%, and improves
  the startup speed of containers by 2.0x.
publication: '*Proceedings of the ACM Symposium on Cloud Computing*'
url_pdf: https://doi.org/10.1145/3357223.3362718
doi: 10.1145/3357223.3362718
---
