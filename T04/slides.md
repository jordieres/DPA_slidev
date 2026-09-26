---
theme: seriph
title: DPA T04 — Project Time Management
info: |
  # Discussion: Project Scope
  Academic Year 2026–27
background: https://apiivm01.etsii.upm.es/~jordieres/DPA/T01/images/Designer_02.png
class: text-center
drawings:
  persist: false
transition: slide-left
comark: true
duration: 35min
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

# T04 DPA Discussion

## Time Management Discussion

Academic Year 2026–2027

<div class="mt-9 text-sm opacity-70">
  Source decks:
  <a href="https://apiivm01.etsii.upm.es/~jordieres/DPA/T04/" target="_blank">Time Management</a>
</div>


---
title: "Basic Concepts"
layout: two-cols
transition: fade-out
---

::left::

## Scheduling

<div class="discussion-panel info discussion-list pt-2">

- <v-click>To create the schedule, from where do we start?</v-click>
- <v-click>What are the methods you know for scheduling the work?</v-click>
- <v-click>Differences between Milestone diagram and Gantt diagram?</v-click>
- <v-click>And between a Gantt and a Precedence Diagram?</v-click>
- <v-click>What kind of precedence relationship do you know?</v-click>

</div>

::right::


<div class="discussion-panel info discussion-list pt-2">

- <v-click>What is the lag time between tasks?</v-click>
- <v-click>Is there any relationship between Work Package duration and its resources? If so, which one?</v-click>
- <v-click>Is the distribution of resources linear within the tasks? And within the work packages?</v-click>
- <v-click>Shall I schedule tasks related to risk contingent actions in the regular schedule from the beginning?</v-click>

</div>

---
title: "Main hipothesis"
layout: two-cols
transition: fade-out
---

::left::

## Precedence approches

<div class="discussion-panel info discussion-list pt-2">

- <v-click>If we accept probabilistic distribution β for task duration, how can we estimate its average duration?</v-click>
- <v-click>How much would the task variance be?</v-click>
- <v-click>What are the main hypotheses of the PERT method?</v-click>
- <v-click>What are the differences between the Critical Path Method and Critical Chain Project Management?</v-click>
- <v-click>Why is CCPM not more common, if it is supposedly so powerful?</v-click>

</div>

::right::

## Operating time approach

<div class="discussion-panel info discussion-list pt-2">

- <v-click>What is the unit for monitoring and controlling schedule progress in Gantt?</v-click>
- <v-click>What is the major issue with the Gantt approach?</v-click>
- <v-click>What is the unit for monitoring and controlling schedule progress in CPM?</v-click>
- <v-click>What are the major issues with CPM when monitoring project execution?</v-click>
- <v-click>What is the unit for monitoring and controlling schedule progress in CCPM?</v-click>

</div>


---
title: "Application usage: Practical Case"
layout: two-cols
transition: fade-out
---

::left:: 

## Let us solve this example
 
<div class="discussion-panel warning discussion-list pt-2 [&_td]:py-1 [&_th]:py-1 [&_li]:my-0.5 text-sm">

| **Task** | **Dur.** | **Pred.** | **Lag** |
|------|:-----:|:------:|------:|
| A | 3 | - | 0 |
| B | 4 | - | 0 |
| C | 5 | FS(A/B) | 0 / -1 |
| D | 2 | FS(C\) | 0 |
| E | 3 | FS(D) | +1 |
| F | 4 | FS(D/E) | +1 / -1 |

</div>

<div class="section-break"></div>

<div class="discussion-panel warning discussion-list pt-2">

- <v-click>ES for A?</v-click>
- <v-click>LS for D?</v-click>
- <v-click>LF for C?</v-click>
- <v-click>Total Slack (TS) for D?</v-click>

</div>


::right::

## Another example

<span v-click><img src="/images/planning_pert.png" class="slide-image-wide" style="max-height: 225px" alt="Solved Scheduling"></span>

<div class="discussion-panel warning discussion-list pt-2">

- <v-click>Total Slack (TS) and Free Slack (FS) for E?</v-click>
- <v-click>Total Slack (TS) and Free Slack (FS) for B?</v-click>

</div>


---
title: "CCPM Case"
layout: two-cols
transition: fade-out
---

::left::

## New case

<div class="discussion-panel warning discussion-list pt-2 [&_td]:py-1 [&_th]:py-1 [&_li]:my-0.5 text-sm">

| **Task** | **Dur.** | **Pred.** | **Lag** | **Res-A** | **Res-B** |
|------|:-----:|--------|:---:|:----:|:----:|
| A | 3 | - | 0 | 2 | 1 |
| B | 4 | - | 0 | 2 | 2 |
| C | 5 | FS(A/B) | 0 / -1 | 3 | 1 |
| D | 2 | FS(C\) | 0 | 2 | 2 |
| E | 6 | FS(B) | 0 | 2 | 3 |
| F | 4 | FS(D) | -1 | 3 | 1 |

</div>

<v-clicks> 

**Resource constraints**

</v-clicks>

<div class="discussion-panel info discussion-list">

- <span v-click>Resource type A = 3</span>
- <span v-click>Resource type B = 3</span>
- <span v-click>ES for E?</span>
- <span v-click>LS for E?</span>
 
</div>

::right::

## Solution

<span v-click><img src="/images/ccpm-01.png" class="slide-image-wide" style="max-height: 225px" alt="Solved Scheduling"></span>

<span v-click><img src="/images/ccpm-02.png" class="slide-image-wide" style="max-height: 225px" alt="Solved Scheduling"></span>

<span v-click><img src="/images/ccpm-03.png" class="slide-image-wide" style="max-height: 225px" alt="Solved Scheduling"></span>


---
title: "📖 Other Concepts"
layout: default
transition: fade-out
---

<div class="discussion-panel info discussion-list compact">

## More questions

<div style="height:15px;"></div>


- <v-click>What is the time baseline? Why do we use it?</v-click>
- <v-click>What about resource control? Is it relevant regardless of the scheduling method?</v-click>
- <v-click>We already know the main hypotheses of the PERT method. Does PERT help in the same way when used by the Project Owner and by the Project Manager?</v-click>
- <v-click>Are you familiar with MS Project?</v-click>
- <v-click>Are you using it already?</v-click>
- <v-click>Did we decide, for the practical assignment, whether to use a PMIS?</v-click>

</div>
