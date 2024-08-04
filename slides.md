---
theme: seriph
background: https://pkrauss-hohl.site/_next/image?url=/static/images/mud.png&w=1200&q=75
class: text-center
highlighter: shiki
lineNumbers: false
info: |
  ## Big Ball of Mud

drawings:
  persist: false
transition: slide-left
title: Welcome to Slidev
mdc: true
---

# Big Ball of Mud

Author: [Peter Krauß-Hohl](https://pkrauss-hohl.site)

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Press Space for next page <carbon:arrow-right class="inline"/>
  </span>
</div>


---
transition: slide-up
level: 2
---

# Introduction
Big Ball of Mud is a paper from Brian Foote and Joseph Yoder from the University of Illimois 
<br>
It was published in the the year **1999**

### It is the most used pattern in software architecture

it can be described:
- haphazardly structured
- sloppy
- unregulated growth
- repeated and expedient repair


---
transition: fade-out
---

# Agenda
<br>

- 📝 **Forces** - a list of forces that can push an org to produce a Big Ball of mud
- 💩 **Big Ball of Mud** - aka Shantytowns or Spaghetti Code
- ⚠️ **Throwaway Code** - "Quick Hack", "Kleenex Code", "Killer Demo" or "Permanent Prototype"
- 🍴 **Piecemeal Growth** - Iterative-Incremental Development
- 🚧 **Keep it Working** - Daily Builds
- 📤 **Shearing Layers** - How Buildings Learn
- 🗻 **Sweeping it under the Rug** - If you can’t make a mess go away, at least you can hide it
- 🏭 **Reconstruction** - Demolition, Throwaway the first one or Start Over
- ⁉️ **Conclusion** - People build BIG BALLS OF MUD because they __work__

<br>
<br>

Read the full paper [here](https://github.com/spring-media/paper_reading_group/blob/master/system_design/Big_Ball_of_Mud.pdf)

<!--
You can have `style` tag in markdown to override the style for the current page.
Learn more: https://sli.dev/guide/syntax#embedded-styles
-->

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

<!--
Here is another comment.
-->

---
layout: image-right
image: >-
  https://pkrauss-hohl.site/_next/image?url=/static/images/forces_ball_of_mud.png&w=1200&q=75
---

# Forces
A number of forces can conspire to drive even the most architecturally conscientious organizations to
produce BIG BALLS OF MUD

* Time
* Cost
* Experience
* Skill
* Visibility
* Complexity
* Change
* Scale

__-> You need to deliver quality software on time, and under budget.__


---
layout: image-right
image: >-
  https://nmgprod.s3.amazonaws.com/media/files/00/f2/00f2634736ffd06a963e5a119dca0861/cover_image.jpg.760x400_q85_crop_upscale.jpg
---

# Time
<br>

* Architecture is a long-term concern, and is only realized later after the market launch - so it is often seen as a luxury.
* It can be even seen as a __risk__ that will consume resources better directed at meeting a fleeting market window.
* Premature architecture can be more dangerous than none at all, as unproved architectural
hypotheses turn into straightjackets that discourage evolution and experimentation


---
layout: image-right
image: >-
  https://www.thedailyhaze.com/wp-content/uploads/2020/11/1604074883897-1024x856.png
---

# Cost
<br>

* Architecture is expensive - it does not pay off immediately
* Quick and dirty can be enough to make money


---
layout: image-right
image: https://tse2.mm.bing.net/th?id=OIP.hNNyi5S7WMtvTgQKtLOpNQHaGq&pid=Api
---

# Experience / Inexperience
<br>

* fresh out of school inexperience
* lack of domain experience
* domain expert who knows the code cold may not have
architectural experience
* Employee turnover can wreak havoc on an organization’s institutional memory
* "on average, average organizations will
have average people"


---
layout: image-right
image: >-
  https://image.tmdb.org/t/p/w600_and_h900_bestv2/oiNc4aTeaUMVNkxL0UWnezmKJgM.jpg
---

# Visibility
<br>

* most development work is "under the hood"
* only developers "realize/see" the architecture of software

---
layout: image-right
image: >-
  https://simplesnippets.tech/wp-content/uploads/2018/06/np-hard-np-complete.jpg
---

# Complexity
<br>

* software often reflects the inherent
complexity of the application domain

-> the software is ugly because the problem is ugly, or at least not well
understood

* __Conways Law__ -> the organization of the system reflects the sprawl and history of the
organization that built it


---
layout: image-right
image: >-
  https://miro.medium.com/v2/resize:fit:2800/0*SBQNWUA1dDtFsMHv.png
---

# Change
<br>

* Architecture is a hypothesis about the future that holds that subsequent change will be
confined to that part of the design space encompassed by that architecture
* expect the unexpected


---
layout: image-right
image: >-
  https://www.alll.com/wp-content/uploads/2014/12/Balanced-Scale.jpg
---

# Scale
<br>

* "good ideas don't always scale"
* "so what do we do, just scale the bad ones?"

---
layout: image-right
image: >-
  https://c8.alamy.com/comp/CT1PN9/shantytown-CT1PN9.jpg
---

# Shantytowns
<br>

* built by using relatively unskilled labor
* maintenance is quite labor intensive
* constructed and maintained primarily by its inhabitants
* There is little overall planning or regulation of growth
* Shantytowns fulfill an immediate, local need for housing by bringing available resources to bear on the problem. Loftier architectural goals are a luxury that has to wait.

---
layout: image-right
image: https://lwfiles.mycourse.app/networkcapitalinsider-public/ddbe61376b4e175b834c65512c7f4687.jpeg
transition: slide-up
---

# Oprganizational Impact of Big Ball of Mud
<br>
If the qualification of a swamp guide gets more valuable than the one of an architect
<br>
<br>

* Conway's Law
* Peter Principle

---
layout: image-left
image: http://images.clipartpanda.com/throwaway-clipart-70387_262_rg-130_b_lg.gif
---

#  Throwaway Code

* Prototypes or Spikes are necessary to understand the problem
* When you build a prototype, there is always the risk that someone will say "that's good enough, ship it"
* The real problem with THROWAWAY CODE comes when it isn't thrown away.

**-> produce, by any means available, simple, expedient, disposable code that adequately
addresses just the problem at-hand**

---
layout: image-left
image: http://www.americaspace.com/wp-content/uploads/2015/09/106iss.jpg
---

#  Piecemeal Growth

* Master plans are often rigid, misguided and out of date.
* "If you can adapt quickly to change, predicting it becomes far less crucial."
* YAGNI
* Feedback for every small piece

**-> Make it work. Make it right. Make it fast**

---
layout: image-left
image: https://sd.keepcalm-o-matic.co.uk/i-w600/keep-calm-and-keep-working-333.jpg
---

#  Keep it working

* Refactoring is the primary means by which programmers maintain order from inside the systems
* daily build
* CI/CD
* testing and testing and even more testing!


---
layout: image-left
image: https://miro.medium.com/v2/resize:fit:1200/1*2ruBRHEr7ynhekPfZ5ai4g.png
---

#  Shearing Layers

* Keep things together that change at the same rate
* Data changes faster than code
* Code changes faster than interfaces
* Interfaces changing faster than frameworks
* Some things should ideally never change in one version (schemas)
* Abstraction can help to keep things together

[Semantic Versioning can help](https://semver.org/)

---
layout: image-left
image: https://i2-prod.mirror.co.uk/incoming/article9361008.ece/ALTERNATES/s1200/The-town-of-Pripyat-near-Chernoby-Nuclear-Power-station-which-is-having-a-Gian-dome-fitted-overt-tod.jpg
---

#  Sweeping it under the rug

* If you can't fix, you can hide it
* Isolate the disordered parts and isolate it
* can be the first step on the way architectural rehabilitation

---
layout: image-left
image: >-
  https://img.izismile.com/img/img4/20111121/640/incredible_building_explosion_640_02.jpg
---

#  Reconstruction
aka the total rewrite

* Obsolescence
* Change of requirements
* Organization - maybe all people are gone who know the system
* of course this is the most drasticall measure 

-> As with any edifice, it is a judgement call, whether to rehab or use the wrecking ball.

---
layout: with-header
---

# Conclusion

* People write Big Balls of Mud because they work!
* There is an ebb and flow of software evolution
* like a messy kitchen while cooking
<br><br><br>

**-> "The key is to ensure that the
system, its programmers, and, indeed the entire organization, learn about the domain, and the
architectural opportunities looming within it, as the system grows and matures."**
