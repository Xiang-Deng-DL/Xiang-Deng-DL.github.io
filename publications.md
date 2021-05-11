---
layout: page
permalink: /publications/index.html
title: Publications
pubs:
  - author: "**Xiang Deng**, Chaoran Cui, Huidi Fang, Xiushan Nie, Yilong Yin"
    title: "
	Personalized Image Aesthetics Assessment"
    booktitle: "CIKM'2017"
    url: https://dl.acm.org/doi/10.1145/3132847.3133052 

  - author: "**Xiang Deng**, Yuanjie Zheng, Yunlong Xu, XiaomingXi, NingLi, Yilong Yin"
    title: "
	Graph cut based automatic aorta segmentation with an adaptive smoothness constraint in 3D abdominal CT images"
    booktitle: "Neurocomputing, 2018"
    url: https://www.sciencedirect.com/science/article/abs/pii/S0925231218305502?via%3Dihub

  - author: "**Xiang Deng**, Chaoran Cui, Huihui Liu, Xiushan Nie, Yilong Yin"
    title: "
	Automatic image cropping with a single fully convolutional network"
    booktitle: "ICIMCS'2018"
    url: https://dl.acm.org/doi/10.1145/3240876.3240906

  - author: "Chaoran Cui, Huidi Fang, **Xiang Deng**, Xiushan Nie, Hongshuai Dai, Yilong Yin"
    title: "
	Distribution-oriented Aesthetics Assessment for Image Search"
    booktitle: "SIGIR'2017"
    url: https://dl.acm.org/doi/10.1145/3077136.3080704  
    
  - author: "Huidi Fang, Chaoran Cui, **Xiang Deng**, Xiushan Nie, Muwei Jian, Yilong Yin"
    title: "
	Image Aesthetic Distribution Prediction with Fully Convolutional Network"
    booktitle: "MMM'2017"
    url: https://link.springer.com/chapter/10.1007%2F978-3-319-73603-7_22 

---

# Publications
________________________________________________________________________________

{% for pub in page.pubs %}
{% unless pub.hidden %}
  - {% if pub.url %} [{{pub.title}}]({{pub.url}}).
    {% else %} {{pub.title}}.
    {% endif %}{% if pub.type %}({{pub.type}})
    {% endif %}<br>
    {{pub.author}}.<br>
    {% if pub.type == 'Technical Report' %}{{pub.number}}
    {% endif %}{{pub.booktitle}}{{pub.school}}{{pub.journal}}.<br>
    {% endif %}
{% endunless %}
{% endfor %}
