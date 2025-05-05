---
title: "Fourier Position Embedding: Enhancing Attention's Periodic Extension for Length Generalization"
authors:
  - Ermo Hua
  - Che Jiang
  - Xingtai Lv
  - Kaiyan Zhang
  - Ning Ding
  - Youbang Sun
  - Biqing Qi
  - Yuchen Fan
  - Xuekai Zhu
  - Bowen Zhou
author_notes:
  - 
  - 
  - 
  - 
  - 
  - 
  - 
  - 
  - 
  - Corresponding Author
date: '2024-12-01T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2024-12-01T00:00:00Z'

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ['3']

# Publication name and optional abbreviated publication name.
publication: '*arXiv* preprint'
publication_short: 

abstract: "Extending the context length of Language Models (LMs) by improving Rotary Position Embedding (RoPE) has become a trend. While existing works mainly address RoPE’s limitations within attention mechanism, this paper provides an analysis across nearly all parts of LMs, uncovering their adverse effects on length generalization for RoPE-based attention. Using Discrete Signal Processing theory, we show that RoPE enables periodic attention by implicitly achieving Non-Uniform Discrete Fourier Transform. However, this periodicity is undermined by the spectral damage caused by: 1) linear layers and activation functions outside of attention; 2) insufficiently trained frequency components brought by time-domain truncation. Building on our observations, we propose Fourier Position Embedding (FoPE), which enhances attention’s frequency-domain properties to improve both its periodic extension and length generalization. FoPE constructs Fourier Series and zero-outs the destructive frequency components, increasing model robustness against the spectrum damage. Experiments across various model scales show that, within varying context windows, FoPE can maintain a more stable perplexity and a more consistent accuracy in a needle-in-haystack task compared to RoPE and ALiBi. Several analyses and ablations bring further support to our method and theoretical modeling."

# Summary. An optional shortened abstract.
summary: 

tags:
  - Position Embedding
  - Length Generalization
  - Large Language Model
featured: false

links:
  # - name: Custom Link
  #   url: http://example.org
url_pdf: https://arxiv.org/pdf/2412.17739.pdf
url_code: https://github.com/TsinghuaC3I/Fourier-Position-Embedding
url_dataset: 
url_poster: 
url_project: 
url_slides: 
url_source: 
url_video: 

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  caption: 'Image credit: [**Original Paper**](https://arxiv.org/pdf/2412.17739.pdf)'
  focal_point: ''
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
slides:
---
