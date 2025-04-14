---
layout: archive
title: "Selected Publications"
permalink: /publications/
author_profile: true
---

{% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}

{% include base_path %}

## 📕 Ph.D. Thesis

**Yigitcan Özer**  
*Source Separation of Piano Music Recordings*  
Ph.D. Thesis, Friedrich-Alexander-Universität Erlangen-Nürnberg (FAU), Erlangen, Germany, 2024

---

## 📘 Journal Papers

**Yigitcan Özer**, Meinard Müller  
*Source Separation of Piano Concertos Using Musically Motivated Augmentation Techniques*  
IEEE/ACM Transactions on Audio, Speech, and Language Processing (TASLP), vol. 32, pp. 1214–1225, 2024

**Yigitcan Özer**, Leo Brütting, Simon Schwär, Meinard Müller  
*libsoni: A Python Toolbox for Sonifying Music Annotations and Feature Representations*  
Journal of Open Source Software (JOSS), vol. 9, no. 98, 2024  

**Yigitcan Özer**, Simon Schwär, Vlora Arifi-Müller, Jeremy Lawrence, Emre Sen, Meinard Müller  
*Piano Concerto Dataset (PCD): A Multitrack Dataset of Piano Concertos*  
Transactions of the International Society for Music Information Retrieval (TISMIR), vol. 6, no. 1, pp. 75–88, 2023

Meinard Müller, **Yigitcan Özer**, Michael Krause, Thomas Prätzlich, and Jonathan Driedger

*Sync Toolbox: A Python Package for Efficient, Robust, and Accurate Music Synchronization*
Journal of Open Source Software (JOSS), 6(64): 1–4, 2021. 

---

## 📘 Conference Papers

**Yigitcan Özer**, Hans-Ulrich Berendes, Vlora Arifi-Müller, Fabian-Robert Stöter, Meinard Müller  
*Notewise Evaluation for Music Source Separation: A Case Study for Separated Piano Tracks*  
Proc. International Society for Music Information Retrieval Conference (ISMIR), San Francisco, USA, 2024

Nazif Can Tamer, **Yigitcan Özer**, Meinard Müller, Xavier Serra  
*TAPE: An End-to-End Timbre-Aware Pitch Estimator*  
Proc. IEEE International Conference on Acoustics, Speech, and Signal Processing (ICASSP), Rhodes Island, Greece, 2023

**Yigitcan Özer**, Meinard Müller  
*Source Separation of Piano Concertos with Test-Time Adaptation*  
Proc. International Society for Music Information Retrieval Conference (ISMIR), Bengaluru, India, 2022, pp. 493–500  

**Yigitcan Özer**, Matěj Ištvánek, Vlora Arifi-Müller, Meinard Müller  
*Using Activation Functions for Improving Measure-Level Audio Synchronization*  
Proc. International Society for Music Information Retrieval Conference (ISMIR), Bengaluru, India, 2022, pp. 749–756

**Yigitcan Özer**, Jonathan Hansen, Tim Zunner, Meinard Müller  
*Investigating Nonnegative Autoencoders for Efficient Audio Decomposition*  
Proc. European Signal Processing Conference (EUSIPCO), Belgrade, Serbia, 2022, pp. 254–258  

<!-- New style rendering if publication categories are defined -->
{% if site.publication_category %}
  {% for category in site.publication_category  %}
    {% assign title_shown = false %}
    {% for post in site.publications reversed %}
      {% if post.category != category[0] %}
        {% continue %}
      {% endif %}
      {% unless title_shown %}
        <h2>{{ category[1].title }}</h2><hr />
        {% assign title_shown = true %}
      {% endunless %}
      {% include archive-single.html %}
    {% endfor %}
  {% endfor %}
{% else %}
  {% for post in site.publications reversed %}
    {% include archive-single.html %}
  {% endfor %}
{% endif %}



