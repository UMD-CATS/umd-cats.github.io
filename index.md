---
layout: default
title: Capital Area Theory Seminar
# redirect_to: "https://cs.umd.edu/~laxman/"
---

The Capital Area Theory Seminar (CATS) is a series of talks in 
Theoretical Computer Science, organized at the department of Computer 
Science, University of Maryland, College Park. 

This semester, the seminar meets on Fridays from 10 am to 11 am at IRB 4105. 
Please sign up for our [mailing list][theory-local] if you would like to 
receive notifications (and Zoom meeting details) for the talks.

If you are interested in giving a talk, please contact [Kishen N Gowda][kishen]
and [Renata Valieva][renata].
<br>
<br>

## Fall 2023 Series
<hr/>

### Upcoming Talks
{% assign talks = site.data.talks | sort: 'datetime' %}
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

[kishen]: https://www.cs.umd.edu/people/kishen19
[renata]: https://www.cs.umd.edu/people/rvalieva
[theory-local]: https://mailman.cs.umd.edu/mailman/listinfo/theory-local
[guy]: http://www.cs.cmu.edu/~guyb/
[julian]: https://people.csail.mit.edu/jshun/
[gm]: https://research.google/teams/graph-mining/
[451F23]: {{ '/CMSC451-F23.html' | prepend: site.baseurl }}
[858NS23]: {{ '/CMSC858N-S23.html' | prepend: site.baseurl }}
