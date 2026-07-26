---
layout: page
title: About
---

## What this is

The **Deep Learning Theory Reading Group** is an informal seminar where, every
other week, one participant presents one paper on the theory of deep learning.
Presentations can cover the presenter's own work or a paper they find worth
discussing. The emphasis is on understanding and open discussion rather than
polished talks.

## Scope

Topics include (but are not limited to): optimization and training dynamics,
generalization, implicit bias, the neural tangent kernel and infinite-width
limits, approximation and expressivity, loss landscapes, and the theory behind
architectures and modern practice.

## Format

- One presenter, one paper, roughly 60 minutes including discussion.
- Interactive — questions throughout are encouraged.
- Slides are optional; walking through the paper or the whiteboard is fine.

## When &amp; where

**Every Sunday, 7:00&nbsp;pm Tehran time** (UTC+3:30; Iran no longer observes DST,
so this is 15:30&nbsp;UTC year-round).
{% if site.meet_url != blank %}We meet on [Google Meet]({{ site.meet_url }}).{% else %}*(Add your recurring Google Meet link as `meet_url` in `_config.yml`.)*{% endif %}

{% if site.calendar_embed_url != blank %}
Add the meetings to your own calendar:

<iframe src="{{ site.calendar_embed_url }}" style="border:0" width="100%" height="500" frameborder="0" scrolling="no"></iframe>
{% endif %}

## Present a paper

Everyone is welcome to present. Two ways to sign up:

1. **Open a pull request** adding an entry to `_data/talks.yml` (see the file for
   the format), or
2. {% if site.contact_email != blank %}Email us at [{{ site.contact_email }}](mailto:{{ site.contact_email }}).{% else %}Email the organizers *(add a contact address in `_config.yml`)*.{% endif %}

## Stay in the loop

{% if site.mailing_list_url != blank %}
- Join the [mailing list]({{ site.mailing_list_url }}) for announcements.
{% else %}
- *Add a `mailing_list_url` in `_config.yml` to link your announcement list here.*
{% endif %}
{% if site.youtube_playlist_url != blank %}
- Watch past sessions on [YouTube]({{ site.youtube_playlist_url }}).
{% endif %}
