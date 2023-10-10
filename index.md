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

 would like to give a talk about your research or your favorite theory paper. We also welcome students/faculty to present their favorite paper (need not be a co-author) with a friend/colleague and if you're looking for a partner to present please send us an email.
 
<br>
<br>

## Fall 2023 Series
<hr/>

### Upcoming Talks

<ul>
{% for talk in site.data.talks %}
  {% include talk.html %}
{% endfor %}
</ul>

### Past Talks

<!-- {% capture thirty_days_ago %}{{'now' | date: '%s' | minus: 2592000 }}{% endcapture %}
{% for post in site.posts %}
    {% capture post_date %}{{ post.posted_on | date: '%s' | plus: 0 }}{% endcapture %}

    {% if job_date > thirty_days_ago %}
        {% include components/job.html job=job %}
    {% endif %}
{% endfor %} -->

[kishen]: https://www.cs.umd.edu/people/kishen19
[renata]: https://www.cs.umd.edu/people/rvalieva
[theory-local]: https://mailman.cs.umd.edu/mailman/listinfo/theory-local
[guy]: http://www.cs.cmu.edu/~guyb/
[julian]: https://people.csail.mit.edu/jshun/
[gm]: https://research.google/teams/graph-mining/
[451F23]: {{ '/CMSC451-F23.html' | prepend: site.baseurl }}
[858NS23]: {{ '/CMSC858N-S23.html' | prepend: site.baseurl }}
