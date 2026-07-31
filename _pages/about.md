---
layout: page
nav_title: About
title: About
---

## What We Do

The **Learning Theory Circle** is an informal seminar where one participant presents one paper on the theory of learning. Presentations can cover the presenter's own work or a paper they find worth discussing. The emphasis is on understanding and open discussion rather than polished talks. Talks are held in Persian for now.


## Scope

Topics include, but are not limited to, optimization and training dynamics, generalization, implicit bias, the neural tangent kernel and infinite-width limits, approximation and expressivity, loss landscapes, and the theory behind architectures and modern practice.


## Format

- One presenter, one paper, roughly 60 minutes including discussion.
- Interactive, questions throughout are encouraged.
- Slides are optional; walking through the paper or the whiteboard is fine.


## When and Where

**Every two weeks on Sunday, 7:00&nbsp;pm Tehran time**, or equivalently UTC+3:30, 
{% if site.meet_url != blank %} we meet on [Google Meet]({{ site.meet_url }}). {% else %}
*(Add your recurring Google Meet link as `meet_url` in `_config.yml`.)*
{% endif %} {% if site.calendar_embed_url != blank %} Add the meetings to your own calendar from below.
<iframe src="{{ site.calendar_embed_url }}" style="border:0; margin-bottom: 25px" width="100%" height="500" frameborder="0" scrolling="no"></iframe>
{% endif %}


## Present a Paper

Everyone is welcome to present. There are two ways to sign up:

1. **Open a pull request** adding an entry to `_data/talks.yml` (see the file for the format), or
2. {% if site.contact_email != blank %}Email us at [{{ site.contact_email }}](mailto:{{ site.contact_email }}).{% else %}Email the organizers *(add a contact address in `_config.yml`)*.{% endif %}


## Stay in the Loop

{% if site.mailing_list_url != blank %}
- Join the [mailing list]({{ site.mailing_list_url }}) for announcements. {% else %}
- *Add a `mailing_list_url` in `_config.yml` to link your announcement list here.* {% endif %}
{% if site.youtube_playlist_url != blank %} - Watch past sessions on [YouTube]({{ site.youtube_playlist_url }}). {% endif %}


## Organizers
We are a group of young scholars passionate about learning theory and enjoy discussing research, exchanging ideas, and learning from one another. You are welcome to join us by helping organize the event or by suggesting a potential presenter. Here are the members of our organizing team.
{% include organizers.html %}
