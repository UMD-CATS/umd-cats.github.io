---
layout: default
title: Capital Area Theory Seminar
semester: Spring 2023
---

The Capital Area Theory Seminar (CATS) is a series of talks in 
Theoretical Computer Science, organized at the department of Computer 
Science, University of Maryland, College Park. 

<!-- Modify this -->
This semester, the seminar meets on Fridays from 11 am to 12 am at IRB 4107. 
Please sign up for our [mailing list][theory-local] if you would like to 
receive notifications (and Zoom meeting details) for the talks.

If you are interested in giving a talk, please contact [Sharmila Duppala][sharmila]
and [Laxman Dhulipala][laxman].
<!--  -->

{% include button.html url="https://calendar.google.com/calendar/u/0?cid=Y182NmExZjJmNjU3MmMwNmI0ZDRkYjc2NmQ1MTNlZGZjNGJlYmY2YjJmNTJlMTg3NGY0NmYxNmExZWQ3YjBlODM2QGdyb3VwLmNhbGVuZGFyLmdvb2dsZS5jb20" content="Add Calendar" %} {% include button.html url="https://www.youtube.com/channel/UCfHfM0BLanICsjnzm_dCLXg" content="Youtube" %}
<br>
<br>

<!-- Modify this -->
<h1>Spring 2023 Series <span><a href="https://calendar.google.com/calendar/embed?src=c_66a1f2f6572c06b4d4db766d513edfc4bebf6b2f52e1874f46f16a1ed7b0e836%40group.calendar.google.com&ctz=America%2FNew_York">[Calendar View]</a></span></h1>
<!--  -->
<hr/>

### Upcoming Talks
<!-- Modify this -->
{% assign talks = site.data.spring23 | sort: 'datetime' %}
<!--  -->
{% capture today %}{{ 'now' | date: '%s' }}{% endcapture %}

<ul>
{% for talk in talks %}
  {% capture talk_date %}{{ talk.datetime | date: '%s' | plus: 0 }}{% endcapture %}
  {% if talk_date >= today %}
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
<br/>
[Web Accessibility][accessibility]

<!-- Modify this -->
[sharmila]: https://trinity24.github.io/
[laxman]: https://www.cs.umd.edu/~laxman/
[theory-local]: https://mailman.cs.umd.edu/mailman/listinfo/theory-local
[accessibility]: https://www.umd.edu/web-accessibility
<!--  -->