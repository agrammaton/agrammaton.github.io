---
layout: about
title: Home
permalink: /

profile:
  align: right
  image: prof_pic.jpg
  image_circular: false
  more_info: >
    <div style="text-align:center">
    <strong>Syed Taha Ali</strong><br>
    Associate Professor<br>
    NUST-SEECS<br>
    Islamabad
    </div>

news: true
selected_papers: false
social: true
---
# Syed Taha Ali

### Engineer  •  Researcher  •  Writer

> *Exploring the intersection of technology, institutions, and society through research, policy, and public engagement.*

I am an Associate Professor in the Department of Electrical Engineering at the **NUST School of Electrical Engineering and Computer Science (NUST-SEECS)**, Islamabad.

My research focuses on computer networks, information security, and technology policy, with particular interests in cryptocurrencies, Internet of Things, machine learning, and emerging technologies.

Beyond academia, I advise government and civil society organizations on technology policy, digital transformation, and institutional best practices. I also write regularly for local media and contribute to the *In Plato's Cave* podcast.

## News

<div class="news">
  {% if site.news and site.news.size > 0 %}
    {% assign news = site.news | sort: "date" | reverse %}
    {% for item in news limit:5 %}
      <div class="news-item">
        <span class="news-date">{{ item.date | date: "%b %-d, %Y" }}</span>
        <div class="news-content">
          {{ item.content }}
        </div>
      </div>
    {% endfor %}
  {% else %}
    <p>No news yet.</p>
  {% endif %}
</div>
