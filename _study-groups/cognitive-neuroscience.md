---
layout: post
title: Cognitive neuroscience
# leader ID = speaker ID - 1
leader: 5
image: banner_BSI_groups.jpg
---

#### List of Resources

**News/Articles**

- [https://www.cell.com/trends/cognitive-sciences/newarticles](https://www.cell.com/trends/cognitive-sciences/newarticles)
- [https://www.sciencedirect.com/topics/psychology/cognitive-neuroscience](https://www.sciencedirect.com/topics/psychology/cognitive-neuroscience)
- [https://www.nature.com/subjects/cognitive-neuroscience](https://www.nature.com/subjects/cognitive-neuroscience)
- [https://theconversation.com/us/topics/cognitive-neuroscience-51190](https://theconversation.com/us/topics/cognitive-neuroscience-51190)

*For BIPOC-authored papers, the "Cognitive" and "Neuroscience" tabs of
the Google Sheet cited here:*
- [https://commons.srcd.org/viewdocument/bipoc-authored-psychology-papers?CommunityKey=b098f303-d3eb-46cd-962d-1b05006fd6c5&tab=librarydocuments](https://commons.srcd.org/viewdocument/bipoc-authored-psychology-papers?CommunityKey=b098f303-d3eb-46cd-962d-1b05006fd6c5&tab=librarydocuments)

*List of Cognitive Neuroscience journals:*
- [https://www.scimagojr.com/journalrank.php?category=2805](https://www.scimagojr.com/journalrank.php?category=2805)

**Social Media Accounts**
- [Cognitive Neuroscience Society](https://twitter.com/cogsci_soc?lang=en)
- [https://twitter.com/cogneuronews?lang=en](https://twitter.com/cogneuronews?lang=en)
- [Trends in Cognitive Sciences](https://twitter.com/trendscognsci?lang=en)
- [The Neuro (Montreal Neurological Institute)](https://twitter.com/theneuro_mni?lang=en)
- [UCL Institute of Cognitive Neuroscience](https://twitter.com/UCL_ICN)
- [Black In Neuro](https://twitter.com/blackinneuro?lang=en)
- [LGBT_PsychNeuro](https://twitter.com/LGBT_PsychNeuro)

**Podcasts**

- [Brain Science](https://brainsciencepodcast.com/)
- [Brain Matters](https://brainpodcast.com/)

*There are also many good selections listed here:*
- [https://byrdnick.com/archives/10238/cognitive-science-philosophy-podcasts](https://byrdnick.com/archives/10238/cognitive-science-philosophy-podcasts)

**Books**

- [How Emotions Are Made: The Secret Life of the Brain - Lisa Feldman Barrett](https://www.goodreads.com/book/show/23719305-how-emotions-are-made)
- [Tales From Both Sides of the Brain -- Michael S. Gazzaniga](https://www.goodreads.com/book/show/22291128-tales-from-both-sides-of-the-brain?ac=1&from_search=true&qid=Em9ZShHWv1&rank=1)
- [How We Learn: The New Science of Education and the Brain -- Stanislas Dehaene](https://www.goodreads.com/book/show/46064083-how-we-learn?from_search=true&from_srp=true&qid=1PKfhSV7SK&rank=7)
- [The Man Who Mistook His Wife for a Hat -- Oliver Sacks](https://www.goodreads.com/book/show/63697.The_Man_Who_Mistook_His_Wife_for_a_Hat_and_Other_Clinical_Tales?ac=1&from_search=true&qid=fgLhIBilUD&rank=1)

<!-- source: https://docs.google.com/document/d/1U87ZWMRvg4ZnBp25x02MqV6nE0bYhf-_Nbzf55OHN8k/edit -->

<!-- #### Journal Club Info -->

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

