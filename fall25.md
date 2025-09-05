---
layout: default
title: Capital Area Theory Seminar
semester: Fall 2025
---

The Capital Area Theory Seminar (CATS) is a series of talks in 
Theoretical Computer Science, organized at the department of Computer 
Science, University of Maryland, College Park. 

<!-- Modify this -->
This semester, the seminar meets on Friday (time and location TBA)
(might differ sometimes, check the schedule below).
Please sign up for our [mailing list][theory-local] if you would like to 
receive notifications (and Zoom meeting details) for the talks.

If you are interested in giving a talk, please contact [Sijing Yu][sijing] (sjyu AT umd DOT edu).
<!--  -->

{% include button.html url="https://calendar.google.com/calendar/u/0?cid=Y182NmExZjJmNjU3MmMwNmI0ZDRkYjc2NmQ1MTNlZGZjNGJlYmY2YjJmNTJlMTg3NGY0NmYxNmExZWQ3YjBlODM2QGdyb3VwLmNhbGVuZGFyLmdvb2dsZS5jb20" content="Add Calendar" %} {% include button.html url="https://www.youtube.com/channel/UCfHfM0BLanICsjnzm_dCLXg" content="Youtube" %}
<br>
<br>

<!-- Modify this -->
<h1>Fall 2025 Series <span><a href="https://calendar.google.com/calendar/u/0?cid=Y182NmExZjJmNjU3MmMwNmI0ZDRkYjc2NmQ1MTNlZGZjNGJlYmY2YjJmNTJlMTg3NGY0NmYxNmExZWQ3YjBlODM2QGdyb3VwLmNhbGVuZGFyLmdvb2dsZS5jb20">[Calendar View]</a>&nbsp;<a href="https://youtube.com/playlist?list=PLguvVsMLmA-DKnG_k6SPvpJfxVfVrvqts&si=BC13YVqgK_pV5_5_">[Youtube Playlist]</a></span></h1>
<!--  -->
<hr/>

### Upcoming Talks
<!-- Modify this -->
{% assign talks = site.data.fall25 | sort: 'datetime' %}
<!--  -->
{% capture today %}{{ 'now' | date: '%s' }}{% endcapture %}

<ul>
{% for talk in talks %}
  {% capture talk_date %}{{ talk.datetime | date: '%s' | plus: 0 }}{% endcapture %}
  {% if talk_date > today %}
      {% include talk.html %}
  {% endif %}
{% endfor %}
</ul>

### Past Talks
<ul>
{% for talk in talks %}
  {% capture talk_date %}{{ talk.datetime | date: '%s' | plus: 0 }}{% endcapture %}
  {% if talk_date < today %}
      {% include talk.html %}
  {% endif %}
{% endfor %}
</ul>

<hr/>

## Previous Semesters
- [Summer 2024]({{ '/summer25.html' | prepend: site.baseurl }})
- [Spring 2025]({{ '/spring25.html' | prepend: site.baseurl }})
- [Fall 2024]({{ '/fall24.html' | prepend: site.baseurl }})
- [Spring 2024]({{ '/spring24.html' | prepend: site.baseurl }})
- [Fall 2023]({{ '/fall23.html' | prepend: site.baseurl }})
- [Spring 2023]({{ '/spring23.html' | prepend: site.baseurl }})

<br/>
<hr/>
<br/>
[Web Accessibility][accessibility]

<!-- Modify this -->
[sijing]: https://www.cs.umd.edu/people/sjyu
[theory-local]: https://mailman.cs.umd.edu/mailman/listinfo/theory-local
[accessibility]: https://www.umd.edu/web-accessibility
<!--  -->