---
layout: post
title: "#BSIsubspace Section"
# leader ID = speaker ID - 1
leader: 7
image: banner_BSI_groups.jpg
---

A (sub)space to discuss and learn about the relationships among classical & novel multivariate and subspace analysis methods 🤓


#### List of Resources
[Coming soon]

<!-- #### Journal Club Info 
[Coming soon] -->

#### Group Leader
<div class="text-left people-modal">
    <div class="modal-body">
        <div class="people-details">
            <div class="row">
                <div class="col-md-2 col-sm-2">
                    {% assign speaker = site.data.speakers[ page.leader ] %}
                    <div class="flow-img img-circle people-img" style="background-image: url({{ site.baseurl | append: '/img/people/' | append: speaker.thumbnailUrl }})"></div>
                </div>
                <div class="col-md-10 col-sm-10 details">
                    <p class="name">{{ speaker.name }} {{ speaker.surname }}
                        <span class="position">{{ speaker.title }}, {{ speaker.company }}</span>
                    </p>
                    {% if speaker.ribbon != null %}
                    <div class="modal-ribbon-wrapper">
                        {% for ribbon in speaker.ribbon %}
                            <a class="modal-ribbon" href="{{ ribbon["url"] }}" target="_blank">{{ ribbon["title"] }}</a>   
                        {% endfor %}
                    </div>
                    {% endif %}
                    <p class="about">{{ speaker.bio | strip_html | truncate: 350 }} <a href="/team">more</a></p>
                </div>
            </div>
        </div>
    </div>

</div>

#### Student Volunteer Core Members
<!-- Volunteer section begins -->
{% for speaker in site.data.subspace_volunteers %}
<div class="text-left people-modal">
    <div class="modal-body">
        <div class="people-details">
            <div class="row">
                <div class="col-md-2 col-sm-2">
                    <div class="flow-img img-circle people-img" style="background-image: url({{ site.baseurl | append: '/img/people/' | append: speaker.thumbnailUrl }})"></div>
                </div>
                <div class="col-md-10 col-sm-10 details">
                    <p class="name">{{ speaker.name }} {{ speaker.surname }}
                        <span class="position">{{ speaker.title }}, {{ speaker.company }}</span>
                    </p>
                    {% if speaker.ribbon != null %}
                    <div class="modal-ribbon-wrapper">
                        {% for ribbon in speaker.ribbon %}
                            <a class="modal-ribbon" href="{{ ribbon["url"] }}" target="_blank">{{ ribbon["title"] }}</a>   
                        {% endfor %}
                    </div>
                    {% endif %}                    
                    <p class="about">{{ speaker.bio | strip_html}}</p>
                    {% for social in speaker.social %}
                    <a href="{{ social["link"] }}" target="_blank">
                        <svg class="icon icon-{{ social["name"] }}" viewBox="0 0 30 32">
                            <use xlink:href="{{ site.baseurl }}/img/sprites/sprites.svg#icon-{{ social["name"] }}"></use>
                        </svg>
                    </a>
                    {% endfor %}
                </div>
            </div>
        </div>
    </div>
</div>
{% endfor %}
