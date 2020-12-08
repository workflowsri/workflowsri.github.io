---
layout: page
title: Team
---

## Leadership

<div style="margin: 2em 0em">
<strong>workflows<span class="RI">RI</span></strong> is a collaborative effort led by 
the University of Southern California (USC), the University of Hawai'i at Mãnoa (UHM), 
and the University of Chicago (UChicago).
</div>

<div class="row">
{% for m in site.data.team %}
    <div class="col-sm-12 col-md-12 col-lg-12 col-xl-6">
        <div class="team">
            <div class="person-thumb">
                <img src="/assets/images/team/{{ m.photo }}" alt=""/>
            </div>
            <div class="social-profile">
                <a href="mailto:{{ m.email }}"><i class="fa fa-envelope"></i></a>
                <br/>
                <a href="{{ m.linkedin }}" target="_blank"><i class="fab fa-linkedin"></i></a>
                <br/>
                <a href="{{ m.website }}" target="_blank"><i class="fa fa-link"></i></a>
            </div>
            <div class="person-info">
                <h3>{{ m.name }}</h3>
                <p>
                  {{ m.role }}
                  <br/>
                  {{ m.institution }}
                </p>
            </div>
        </div>
    </div>
{% endfor %}
</div>

You can reach the <strong>workflows<span class="RI">RI</span></strong> leadership team
at [leadership@workflowsri.org](mailto:leadership@workflowsri.org).

<br/>

## Board of Experts

<div style="margin: 2em 0em">
<strong>workflows<span class="RI">RI</span></strong> is supported by a <i>board of experts</i>, 
composed of lead researchers from distinct workflow management systems efforts, who are the 
primary drivers of the outcomes of this project.
</div>

<div class="row" style="margin-top: 1em">
{% for m in site.data.experts %}
    <div class="col-sm-12 col-md-12 col-lg-12 col-xl-5">
        <div class="team">
            <div class="expert-thumb">
                <img src="/assets/images/experts/{{ m.photo }}" alt=""/>
            </div>
            <div class="expert-info">
                <p>{{ m.name }}<br/>
                <a href="{{ m.website }}" target="_blank">{{ m.system }}</a></p>
            </div>
        </div>
    </div>
{% endfor %}
</div>
