---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: 'UniKV: Toward High-Performance and Scalable KV Storage in Mixed Workloads
  via Unified Indexing'
subtitle: ''
summary: ''
authors:
- Qiang Zhang
- Yongkun Li
- Patrick P. C. Lee
- Yinlong Xu
- Qiu Cui
- Liu Tang
tags:
- '"Compaction"'
- '"data locality"'
- '"design optimizations"'
- '"hash indexing"'
- '"high-performance storage"'
- '"indexing"'
- '"Indexing"'
- '"indexing management"'
- '"key-value stores"'
- '"KV stores"'
- '"Log-Structured Merge-tree"'
- '"LSM-tree"'
- '"merging"'
- '"Merging"'
- '"optimisation"'
- '"read-write mixed workloads"'
- '"Scalability"'
- '"scalable KV storage"'
- '"Sorting"'
- '"storage management"'
- '"Throughput"'
- '"tree data structures"'
- '"unified indexing"'
- '"UniKV design"'
categories: []
date: '2020-04-01'
lastmod: 2020-09-16T19:06:55+08:00
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
publishDate: '2020-09-16T11:06:54.169547Z'
publication_types:
- 1
abstract: Persistent key-value (KV) stores are mainly designed based on the Log-Structured
  Merge-tree (LSM-tree), which suffer from large read and write amplifications, especially
  when KV stores grow in size. Existing design optimizations for LSM-tree-based KV
  stores often make certain trade-offs and fail to simultaneously improve both the
  read and write performance on large KV stores without sacrificing scan performance.
  We design UniKV, which unifies the key design ideas of hash indexing and the LSM-tree
  in a single system. Specifically, UniKV leverages data locality to differentiate
  the indexing management of KV pairs. It also develops multiple techniques to tackle
  the issues caused by unifying the indexing techniques, so as to simultaneously improve
  the performance in reads, writes, and scans. Experiments show that UniKV significantly
  outperforms several state-of-the-art KV stores (e.g., LevelDB, RocksDB, HyperLevelDB,
  and PebblesDB) in overall throughput under read-write mixed workloads.
publication: '*2020 IEEE 36th International Conference on Data Engineering (ICDE)*'
doi: 10.1109/ICDE48307.2020.00034
---
