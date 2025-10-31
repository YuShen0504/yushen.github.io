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
* 2019-2024  PhD.
  - Geospatial Science and Engineering, GSCE, South Dakota State University, USA    
* 2017-2019  Master
  - Cartography and GIS, Institute of Remote Sensing and Digital Earth, CAS, China 
* 2012-2016  Bachelor
  - Cartography and GIS, China University of Mining and Technology, China 


Work experience
======
* 2025-2026  Postdoctoral Associate.
  - Nicholas School of the Environment, Duke University, USA
  - Supervisor: Tong Qiu (https://ecotongqiu.com/)
* 2024-2025  Postdoctoral Research Associate
  - Geospatial Sciences Center of Excellence (GSCE), South Dakota State University, USA
  - Supervisor: Xiaoyang Zhang (https://www.sdstate.edu/geography-geospatial-sciences/xiaoyang-zhang-lab)
  
Skills
======
* Computing skill:
  - Interactive Data Language (IDL)
  - R
  - C
  - Perl
  - Python
* HPC cluster
  - SDSU Innovator cluster
  - Duke Compute Cluster
* Software
  - ENVI
  - ArcGIS Pro
  - Google Earth Engine

Publications
======
  {% raw %}{% assign pubs = site.publications | sort: "date" | reverse %}
  {% assign years = pubs | map: "year" | uniq %}
  {% for y in years %}
  ### {{ y }}
  {% for post in pubs %}
    {% if post.year == y %}
      {% include archive-single-cv.html %}
    {% endif %}
  {% endfor %}
  {% endfor %}{% endraw %}
  
Talks
======
  <ul>{% for post in site.talks reversed %}
    {% include archive-single-talk-cv.html  %}
  {% endfor %}</ul>
  
Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Service and leadership
======
* Currently signed in to 43 different slack teams
