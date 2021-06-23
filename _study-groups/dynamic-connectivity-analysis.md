---
layout: post
title: Dynamic Activity/Connectivity Analysis
# leader ID = speaker ID - 1
leader: 1
image: banner_BSI_groups.jpg
---

{{ page.title }} group: This is a venue for discussion, study and brainstorming around analysis of dynamics in functional imaging data. We encourage naive inquiries and out-of-box ideas, technical questions, debates, sharing of papers and exploration of collaborative possibilities. In time we will also have speakers, panel discussions and a casual journal club. Suggestions for other exciting ways to use this channel are encouraged.

#### List of Resources
[Coming soon]

#### Journal Club Info 
Tentative date: August 21, 2:00 pm - 3:00 pm EST
More information coming soon.

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
                    <p class="about">{{ speaker.bio| strip_html | truncate: 350 }} <a href="/team">more</a></p>
                </div>
            </div>
        </div>
    </div>

</div>

