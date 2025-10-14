---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: single
author_profile: true
---

I am a *Ph. D. student* at UCLouvain. My supervisor is [Raphaël Jungers](https://perso.uclouvain.be/raphael.jungers/content/home). My research interests are in the area of control theory, more specifically abstraction-based control.  


---

### Latest news

<ul style="list-style-type: disc; padding-left: 1.5em;">
  {% for post in site.posts %}
    <li style="margin-bottom: 0.5em;">
      {% if post.date %}
        <em>{{ post.date | date: "%b %-d, %Y" }}</em> – 
      {% endif %}
      {{ post.excerpt | markdownify | strip_html }}
    </li>
  {% endfor %}
</ul>