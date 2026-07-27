---
layout: page
title: Deep Learning Theory Reading Group
---

We meet **every Sunday at 7:00&nbsp;pm Tehran time**. Each session, one person
presents one paper — their own work or someone else's — on the theory of deep
learning, followed by open discussion. See the [About page](about.md) for the
format and how to present.

{% if site.mailing_list_url != blank or site.youtube_playlist_url != blank %}
{% if site.mailing_list_url != blank and site.youtube_playlist_url != blank %}
Announcements go out on our [mailing list]({{ site.mailing_list_url }}), and recordings live on [YouTube]({{ site.youtube_playlist_url }}).
{% elsif site.mailing_list_url != blank %}
Announcements go out on our [mailing list]({{ site.mailing_list_url }}).
{% elsif site.youtube_playlist_url != blank %}
Recordings live on [YouTube]({{ site.youtube_playlist_url }}).
{% endif %}
{% endif %}

{% if site.organizers %}
## Organizers

{% for organizer in site.organizers %}
- {{ organizer }}
{% endfor %}
{% endif %}

{% if site.calendar_embed_url != blank %}
<iframe src="{{ site.calendar_embed_url }}" style="border:0" width="100%" height="500" frameborder="0" scrolling="no"></iframe>
{% endif %}

{% include talks_tables.html %}
