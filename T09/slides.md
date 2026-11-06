---
theme: seriph
title: DPA T09 — Project Tracking & Monitoring
info: |
  # Discussion: Project Tracking & Monitoring
  Academic Year 2026–2027
background: /images/Designer_02.png
class: text-center
drawings:
  persist: false
transition: slide-left
mdc: true
duration: 40min
---

<style>
.slidev-layout,
.slidev-layout h1,
.slidev-layout h2,
.slidev-layout h3 { color: #102a43; }
.discussion-list { font-size: .84em; line-height: 1.18; }
.discussion-list li { margin-bottom: .42rem; }
.discussion-list.compact { font-size: .75em; line-height: 1.10; }
.discussion-list.compact li { margin-bottom: .27rem; }
.discussion-panel { padding: .6rem .9rem; border-radius: 10px; background: rgba(255,255,255,.70); }
.discussion-panel.info { border-left: 5px solid #2196f3; }
.discussion-panel.warning { border-left: 5px solid #f59e0b; }
.discussion-panel.success { border-left: 5px solid #22a06b; }
.slide-image { display: block; margin: .35rem auto 0; max-height: 300px; max-width: 94%; width: auto; }
.slide-image-large { display: block; margin: .25rem auto 0; max-height: 390px; max-width: 96%; width: auto; }
.section-label { letter-spacing: .12em; text-transform: uppercase; font-size: .8rem; opacity: .65; }
</style>

# T09 Project Tracking & Monitoring

## Project Monitoring

Academic Year 2026–2027

<div class="source-note">
Project Monitoring Discussion Session
</div>

---
title: "Tracking Techniques"
layout: two-cols
transition: fade-out
background: /images/Designer_02.png
backgroundSize: cover
---

## Tracking Techniques

::left::

<img
  src="/images/wbs-obs.png"
  alt="WBS OBS relationship"
  class="slide-image"
/>

::right::

<div style="height:15px;"></div>
<div class="discussion-list">

- <span v-click>What does cost account include?</span>
- <span v-click>Which costs are included in a specific cost account?</span>
- <span v-click>Does one team member belong to a single cost account or to many?</span>

</div>

---
title: "Tracking Techniques"
layout: two-cols
transition: fade-out
background: /images/Designer_02.png
backgroundSize: cover
---

## Concepts

::left::

<div class="discussion-list">

- <span v-click>What techniques for project tracking do you know?</span>
- <span v-click>In PM<sup>2</sup> how tracking communication is implemented?</span>
- <span v-click>What Project Status Report (PSR) aims to?</span>
- <span v-click>What Project Progress Report (PPR) aims to?</span>
- <span v-click>Which technique do you recommend? Why?</span>
- <span v-click>Can you figure out connections between tracking, RRG, and tolerances? Between all the three or just by pairs? If so, which ones?</span>

</div>

::right::

<div style="height:15px;"></div>

<div class="discussion-list">

- <span v-click>What does 0/50/100% means for tracking?</span>
- <span v-click>Is it Cost Control (Real vs Foreseen) a valid tracking tool?</span>
- <span v-click>What does EVMS mean? and What does ESMS mean?</span>
- <span v-click>What is the differencebetween them?</span>
- <span v-click>Which of these techniques work at Project level? At WorkPackage Level? at Task level? Why?</span>

</div>

---
title: "EVMS"
layout: two-cols
transition: fade-out
background: /images/Designer_02.png
backgroundSize: cover
---

## Terminology

::left::

<div style="height:15px;"></div>

<div class="discussion-list">

- <span v-click>What does BAC mean? And EAC?</span>
- <span v-click>Is there a single estimation for EAC? Why?</span>
- <span v-click>What does SPI means? and CPI?</span>
- <span v-click>How to calculate the PV?</span>
- <span v-click>How to calculate the EV?</span>
- <span v-click>How to calculate the AC?</span>
- <span v-click>What does TCPI mean?</span>
- <span v-click>What does LRE mean?</span>
- <span v-click>If you do have tasks lasting 4 days and you have an EVMS system in operation, when progress and effort must be reported?</span>

</div>

::right::

<div style="height:15px;"></div>

<div class="discussion-list">

- <span v-click>Do these techniques work for tracking individual resources instead of tasks? Why?</span>
- <span v-click>What do you think if during one project CPI > 1 and SPI < 1 ? Do you expect the project finish on time? Why?</span>
- <span v-click>Is there a single TCPI for a single project in a specific moment? Why? And SPI?, and CPI?</span>
- <span v-click>What is the meaning for TCPI(LRE) = 1.3 ? Why?</span>
- <span v-click>Do you have a clear vision on how to implement EVMS method in your project?</span>

</div>


---
title: "EVMS"
layout: two-cols
transition: fade-out
background: /images/Designer_02.png
backgroundSize: cover
---

## Examples

::left::

<div class="discussion-list">

- <span v-click>What do you think when one project CPI = 0.76 and TCPI = 1.15 ? Do you expect the project finish on time? Why?</span>
- <span v-click>What do you think when one project CPI = 0.99 and SPI = 0.75 ? Do you expect the project finish on time? Why?</span>
- <span v-click>What do you think when one project SPI = 0.76 and TCPI = 1.15 ? What is the CPI value? Why?</span>
- <span v-click>Interpretation of the next picture?</span>

</div>

::right::

<img
  src="/images/scurve.png"
  alt="S-courve"
  class="slide-image"
/>

---
title: "SPI - CPI"
layout: default
transition: fade-out
background: /images/Designer_02.png
backgroundSize: cover
---

## Interpretation

<img
  src="/images/spi-cpi.png"
  alt="SPI-CPI"
  class="slide-image"
/>

<div class="discussion-list">

- <span v-click>How to read the previous picture?</span>

</div>

---
title: "Performance SPI - CPI"
layout: default
transition: fade-out
background: /images/Designer_02.png
backgroundSize: cover
---

<img
  src="/images/performance-spi-cpi.png"
  alt="SPI-CPI"
  class="slide-image"
  style="max-height: 400px; width: auto;"
/>

<div class="discussion-list">

- <span v-click>How to read the previous picture?</span>

</div>