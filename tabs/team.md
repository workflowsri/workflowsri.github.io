---
title: Team
---

## Leadership

workflowsRI is a collaborative effort led by the University of Southern California (USC), 
the University of Hawai'i at Mãnoa (UHM), and the University of Chicago (UChicago).

{% for m in site.data.team %}

<div class="row">
    <div class="col-sm-12 col-md-12">
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
</div>

{% endfor %}
