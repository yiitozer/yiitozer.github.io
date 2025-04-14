---
layout: archive
title: "Publications"
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
[Demo](https://www.audiolabs-erlangen.de/resources/MIR/PCD_AudioLabs) ·  
[FAU Repository](https://open.fau.de/handle/openfau/31319)

---

## 📘 Journal Papers

**Yigitcan Özer**, Meinard Müller  
*Source Separation of Piano Concertos Using Musically Motivated Augmentation Techniques*  
*IEEE/ACM Transactions on Audio, Speech, and Language Processing (TASLP)*, vol. 32, pp. 1214–1225, 2024  
[Demo](https://www.audiolabs-erlangen.de/resources/MIR/2024-TASLP-PianoConcertoSeparation) ·  
[DOI](https://doi.org/10.1109/TASLP.2024.3356980)


<!-- Add more journal papers below as needed -->





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



