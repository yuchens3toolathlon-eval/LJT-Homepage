---
permalink: /
title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a first-year PhD candidate at the [HKUST NLP Group](https://junxianhe.info/) under the supervision of [Professor Junxian He](https://junxianhe.info/). I graduated from Shanghai Jiao Tong University (SJTU) in June 2024 with a B.Eng. degree.

My research focuses on natural language processing and machine learning. I am particularly interested in:
- **LLM Reasoning and Reinforcement Learning**
- **Hallucination in Vision-Language Models (VLM)**
- **LLM Truthfulness and Interpretability**

Education
======
* **Ph.D. in Computer Science**, Hong Kong University of Science and Technology (2024 - Present)
* **B.Eng.**, Shanghai Jiao Tong University (2020 - 2024)

Research Experience
======
* **Research Intern** at MINIMAX (February 2025 - Present)
* **Research Intern** at Tencent WXG (June 2024 - September 2024)
  * Advisor: Zifei Shan
* **Research Intern** at Shanghai AI Lab (June 2023 - December 2023)
  * Advisor: Prof. Yu Cheng

Honors and Awards
======
* **Zhiyuan Honor Scholarship**, Shanghai Jiao Tong University

Publications
======
<!-- This handles the automatic display of publications from the _publications folder -->
{% include base_path %}
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

Skills
======
* **Research**: Natural Language Processing, Machine Learning, LLM Reasoning, VLM Hallucination
* **Programming**: Python, Deep Learning frameworks
* **Languages**: English, Chinese (Native)

Contact
======
* **Email**: [jliugi@connect.ust.hk](mailto:jliugi@connect.ust.hk)
* **GitHub**: [Vicent0205](https://github.com/Vicent0205)
* **Google Scholar**: [Profile](https://scholar.google.com/citations?hl=en&user=tbK9jl4AAAAJ&view_op=list_works&sortby=pubdate)
* **X (Twitter)**: [@junteng88716710](https://twitter.com/junteng88716710)
