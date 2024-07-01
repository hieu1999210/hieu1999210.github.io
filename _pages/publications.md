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
<table id="pub" width="100%" cellspacing="0" cellpadding="0" border="None">
<tbody>
{% for post in site.publications reversed %}
  <tr> {% include pub.html %} </tr>
{% endfor %}
</tbody>
</table>