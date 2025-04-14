---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* **Ph.D. in Semantic Audio Processing**, Friedrich Alexander University Erlangen-Nuremberg, Germany  
  * *Jan 2021 – Jun 2024*  
  * Thesis: *Source Separation of Piano Music Recordings*  
  * Advisor: Prof. Meinard Müller  
  * Focus: Audio source separation, music synchronization, and audio decomposition

* **M.S. in Communications Engineering**, Technical University of Munich, Germany  
  * *Sep 2013 – Nov 2015*  
  * Thesis: *Multimodal Deep Convolutional Neural Networks for Texture Classification*  
  * GPA: 1.9 / 1.0

* **B.S. in Electrical and Electronics Engineering**, Bilkent University, Turkey  
  * *Sep 2009 – Jun 2013*  
  * Graduated with College Honors  
  * GPA: 3.77 / 4.00

Work Experience
======
* **Postdoctoral Researcher**, National Institute of Informatics, Tokyo, Japan
  * *Yamagishi Lab* — April 2025 — present
  * Audio watermarking
  * Generative models for speech and music processing

* **Research Intern**, Sony AI, Tokyo, Japan  
  * *Music Foundation Model Team — Sep 2024 – Dec 2024*  
  * Audio watermarking with deep learning techniques

* **Research Assistant**, International Audio Laboratories Erlangen, Germany  
  * *Semantic Audio Processing Group — Jan 2021 – Aug 2024*  
  * Source separation, music synchronization, and decomposition

* **Research Associate**, Fraunhofer IIS, Erlangen, Germany  
  * *Spoken Language Processing Group — Jan 2019 – Dec 2020*  
  * Lead developer for TTS pipelines; music processing with NMF

* **Data Science Consultant**, Data Insights GmbH, Munich, Germany  
  * *Jun 2017 – Dec 2018*  
  * ML for word mining, computer vision, and time series  
  * Agile consulting with Scrum

* **Machine Learning Engineer**, Cape Analytics GmbH, Munich, Germany  
  * *Jan 2016 – May 2017*  
  * Deep learning for computer vision; supervised student team

Skills
======
* Python (Proficient)
* C++, MATLAB (Intermediate)
* PyTorch, TensorFlow, Apache Spark

Languages
======
* English (Fluent), German (Fluent), Turkish (Native)  
* Japanese (Intermediate), French (Intermediate)  
* Spanish (Basic), Russian (Basic), Persian (Basic)

Publications
======
<ul>{% for post in site.publications reversed %}
  {% include archive-single-cv.html %}
{% endfor %}</ul>

Talks
======
<ul>{% for post in site.talks reversed %}
  {% include archive-single-talk-cv.html %}
{% endfor %}</ul>
