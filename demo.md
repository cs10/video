---
layout: default
title: L@S Demo
stuff:
    - name: Canon XA10
      amzn:
      bpho: 749467-REG
      desc: This was the camera we used to record the demo. It's compact, but high quality and includes an HDMI output feed to the computer.
    - name: 15" Macbook Pro (retina display)
      amzn:
      bpho:
      desc:
    - name: Blackmagic Ultrastudio Mini Recorder
      amzn:
      bpho:
      desc:
    - name: Blackmagic Intensity Extreme
      amzn:
      bpho:
      desc:
    - name: Blackmagic Ultrastudio Express
      amzn:
      bpho:
      desc: While we didn't actually use this for the demo, we have this slightly larger box because it allows us to more easily record high quality audio when necessary.
    - name: Green Screen
      amzn:
      bpho:
      desc:
    - name: Tripod
      amzn:
      bpho:
      desc:
    - name: Tripod Head
      amzn:
      bpho:
      desc:
    - name: Arri Light
      amzn:
      bpho:
      desc:
    - name: Softbox (for Light)
      amzn:
      bpho:
      desc:
    - name: HDMI Splitter
      amzn:
      bpho:
      desc:
---

# DEMO: Best Practices for MOOC Video
This page describes our setup for the demo we presented at Learning @ Scale 2014. While the demo was a 15 minute overview with some tips for production, this page includes a lot more detail about how we made everything work.

## Slides
<!-- TODO: Post file version to slideshare and embed. -->
An **unfinished** version of our slides can be found, [here][as-given]. (PDF link).

We'll upload a more finished version with lots of bonus material soon! Promise! :)

## Setup
Our setup was relatively simple for the demo, and once configured could be setup in a couple minutes. The signal flow diagram below shows how everything was connected. We had a green screen, and a light standing next to the camera, facing the green screen to help with lighting. The "Host" computer was the main computer providing video to a single projector.

As a quick point, the entire setup (excluding a laptop) could be built for around $2,000 depending on how much extra equipment or features you need. If you're looking to build a setup yourself, shoot for a good middle-range for flexibility that would allow you to upgrade as necessary.

__At the demo, we projected the composite feed (green screen overlay on slides) to the projector. In a normal lecture setup, you would probably want to project the presenter's output. To do this you would split the output of the presenter computer. We've listed one recommendation for a splitter below.__

![demo-setup][flow-jpg]

<!-- TODO: Add an image showing setup + camera screen grab. -->


## Hardware
This is a list of the specific hardware that we used during the presentation, with a little bit about what each piece was doing. We've listed specific models, but you should be able to swap any item for something similar if you'd like.

<ul>
    {% for i in page.stuff %}
    <li>
        {{ i.name }}
        (<a href="{{ i.amzn }}&{{ site.amzn }}">Amazon</a>)
        (<a type="bhphoto" data-sku="{{ i.bpho }}">B&amp;H Photo</a>)
        <br />{{ i.desc }}
    </li>
    {% endfor %}
</ul>

#### Additional Tools
* Presenter Computer
* HDMI Cables
* Mini-HDMI Cable -- Our camera has a special HDMI connector.
* Thunderbolt Cables
* Power strip
* Wireless Microphone (The room was small at the talk, so we didn't actually need this.)


## Software


[as-given]: mooc-vide-as-given-ROUGH.pdf
[keynote]: xxx
[keynote-small]: xxx
[pdf]: xxx
[conduit]: xxx
[conduti-as]: xxx
[flow-jpg]: demo-flow-las2014-ball-arvai-parikh.jpg