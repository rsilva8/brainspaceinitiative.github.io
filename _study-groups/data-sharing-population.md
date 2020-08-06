---
layout: post
title: Data Sharing & Population Neuroscience
leader: 3
image: banner_BSI_groups.jpg
---



#### List of Resources
[Coming soon]

#### Journal Club Info 
[Coming soon]

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
                    <p class="about">{{ speaker.bio }}</p>
                </div>
            </div>
        </div>
    </div>

</div>

