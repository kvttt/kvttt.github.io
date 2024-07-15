---
layout: archive
title: "Sitemap"
permalink: /sitemap/
author_profile: true
---

{% include base_path %}

A list of all the posts and pages found on the site. For you robots out there is an [XML version]({{ base_path }}/sitemap.xml) available for digesting as well.

{% include archive-single.html title="Projects" url="/projects/" %}
{% include archive-single.html title="Notes" url="/notes/" %}
{% include archive-single.html title="Professional Experiences" url="/experiences/" %}
{% include archive-single.html title="About" url="/about/" %}
{% include archive-single.html title="Sitemap" url="/sitemap/" %}
{% include archive-single.html title="Videos" url="/videos/" %}

[//]: # (<h2>Pages</h2>)

[//]: # ({% for post in site.pages %})

[//]: # (  {% include archive-single.html %})

[//]: # ({% endfor %})

[//]: # (<h2>Posts</h2>)

[//]: # ({% for post in site.posts %})

[//]: # (  {% include archive-single.html %})

[//]: # ({% endfor %})

[//]: # ()
[//]: # ({% capture written_label %}'None'{% endcapture %})

[//]: # ()
[//]: # ({% for collection in site.collections %})

[//]: # ({% unless collection.output == false or collection.label == "posts" %})

[//]: # (  {% capture label %}{{ collection.label }}{% endcapture %})

[//]: # (  {% if label != written_label %})

[//]: # (  <h2>{{ label }}</h2>)

[//]: # (  {% capture written_label %}{{ label }}{% endcapture %})

[//]: # (  {% endif %})

[//]: # ({% endunless %})

[//]: # ({% for post in collection.docs %})

[//]: # (  {% unless collection.output == false or collection.label == "posts" %})

[//]: # (  {% include archive-single.html %})

[//]: # (  {% endunless %})

[//]: # ({% endfor %})

[//]: # ({% endfor %})
