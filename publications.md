---
title: Publications
permalink: /publications/
---
<div class="project-container">
  <h1>Publications</h1>
  <!-- <p>Some of the things I've dabbled on.</p>
  <br><center>
  <a href="{{ site.baseurl }}/portfolio-design-education"><span class="label label-danger">Design for Education</span></a>
  <a href="{{ site.baseurl }}/portfolio-design-sustainability"><span class="label label-danger">Design for Sustainability</span></a>
  <a href="{{ site.baseurl }}/portfolio-arts-games"><span class="label label-danger">Arts and Games</span></a>
  <a href="{{ site.baseurl }}/portfolio-others"><span class="label label-danger">Others</span></a></center> -->
</div>

<div class="row">
<div class="col-lg-12">
<h1>Publications</h1>
{% assign pubs = site.publications %}
{% for pub in pubs reversed %}
    <div class="project-box">
      <div class="row">
        <div class="col-lg-3 project-image">
          <a href="{{ site.baseurl }}{{ pub.url }}">
          {% if pub.image %}
          <img src="{{ site.baseurl }}{{ pub.image }}">
          {% else %}
          <div class="thumbnail blankbox"></div>
          {% endif %}
        </a>
        </div>
        <div class="col-lg-9 project-post">
          <a href="{{ site.baseurl }}{{ pub.url }}"><h3>{{ pub.title }}</h3></a>
          <!-- <p class="meta"><small>&nbsp;<i class="fa fa-calendar-o"></i><time>
            {{ pub.date | date_to_string | date: "%Y"  }}
          </time></small></p><hr/> -->
          <!-- <a href="{{ site.baseurl }}{{ pub.url }}">
            <div class="post">
          {{ pub.content | strip_html | truncatewords:75}}
            </div>
          </a> -->
          <p>{{ pub.bib }}</p>
        </div>
      </div>
    </div>
{% endfor %}
</div>
</div>
