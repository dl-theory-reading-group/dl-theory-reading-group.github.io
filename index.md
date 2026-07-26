---
layout: page
title: Deep Learning Theory Reading Group
---

We meet **every Sunday at 7:00&nbsp;pm Tehran time**. Each session, one person
presents one paper — their own work or someone else's — on the theory of deep
learning, followed by open discussion. See the [About page](about.md) for the
format and how to present.

{% if site.mailing_list_url %}
Announcements go out on our [mailing list]({{ site.mailing_list_url }}).
{% endif %}
{% if site.youtube_playlist_url %}
Recordings live on [YouTube]({{ site.youtube_playlist_url }}).
{% endif %}

{% if site.calendar_embed_url %}
<iframe src="{{ site.calendar_embed_url }}" style="border:0" width="100%" height="500" frameborder="0" scrolling="no"></iframe>
{% endif %}

{% assign sorted = site.data.talks | sort: "date" %}
{% assign today = site.time | date: "%Y%m%d" | plus: 0 %}

## Upcoming talks

<table class="talks">
  <thead>
    <tr><th>Date</th><th>Presenter</th><th>Paper</th><th>Slides</th><th>Video</th></tr>
  </thead>
  <tbody>
  {% assign has_upcoming = false %}
  {% for talk in sorted %}
    {% assign ts = talk.date | date: "%Y%m%d" | plus: 0 %}
    {% if ts >= today %}
      {% assign has_upcoming = true %}
      {% include talk_row.html talk=talk %}
    {% endif %}
  {% endfor %}
  {% unless has_upcoming %}
    <tr><td colspan="5" class="talk-muted">Nothing scheduled yet — check back soon.</td></tr>
  {% endunless %}
  </tbody>
</table>

## Past talks

<table class="talks">
  <thead>
    <tr><th>Date</th><th>Presenter</th><th>Paper</th><th>Slides</th><th>Video</th></tr>
  </thead>
  <tbody>
  {% assign sorted_desc = sorted | reverse %}
  {% for talk in sorted_desc %}
    {% assign ts = talk.date | date: "%Y%m%d" | plus: 0 %}
    {% if ts < today %}
      {% include talk_row.html talk=talk %}
    {% endif %}
  {% endfor %}
  </tbody>
</table>
