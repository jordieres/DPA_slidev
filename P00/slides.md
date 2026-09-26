---
# try also 'default' to start simple
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://cover.sli.dev
# some information about your slides (markdown enabled)
title: Welcome to DPA Course
info: |
  ## Slidev Starter Template
  Presentation slides for course participants.
  Learn more at [Sli.dev](https://sli.dev)
# apply UnoCSS classes to the current slide
class: text-center
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left
# enable Comark Syntax: https://comark.dev/syntax/markdown
comark: true
# duration of the presentation
duration: 35min
---

# Welcome to DPA T04 Presentation slides

<div @click="$slidev.nav.next" class="mt-12 py-1" hover:bg="white op-10">
  Press Space for next page <carbon:arrow-right />
</div>

<div class="abs-br m-6 text-xl">
  <button @click="$slidev.nav.openInEditor()" title="Open in Editor" class="slidev-icon-btn">
    <carbon:edit />
  </button>
  <a href="https://github.com/slidevjs/slidev" target="_blank" class="slidev-icon-btn">
    <carbon:logo-github />
  </a>
</div>

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---
title: DPA T04 Discussion: Milestones and others.
layout: default
transition: fade-out
background: ./images/Designer.png
backgroundSize: cover
info: DPA-T04 Planning
class: text-center
drawings:
  persist: false
---


# Scheduling

- <v-click>To create the schedule, from where do we start?</v-click>

- <v-click>Differences between Milestone diagram and Gantt diagram?</v-click>

- <v-click>And between a Gantt and a Precedence Diagram?</v-click>

- <v-click>What kind of precedence relationship do you know?</v-click>

---
title: DPA T04 Discussion: Lags and other details.
layout: default
transition: fade-out
background: ./images/Designer.png
backgroundSize: cover
info: DPA-T04 Planning
class: text-center
drawings:
  persist: false
---

# Schedule (II)

- [ ] What is the lag time between tasks?
- [ ] Is there any relationship between Work Package duration and its resources? If so, which one?
- [ ] Is the distribution of resources linear within the tasks and within the work packages?
- [ ] Shall I schedule tasks related to risk contingency actions in the regular schedule from the beginning?

---

# Schedule (III)

- [ ] If we accept a β distribution for task duration, how can we estimate the average duration?
- [ ] How much variance would we have?
- [ ] What are the main hypotheses of the PERT method?
- [ ] What are the differences between Critical Path Method and Critical Chain Project Management?
- [ ] Why is CCPM not more commonly used?

---

# From the CCPM Perspective

- [ ] What is the unit for monitoring and controlling the schedule in a Gantt chart?
- [ ] What is the major issue with the Gantt approach?
- [ ] What is the unit for monitoring and controlling the schedule in CPM?
- [ ] What are the major issues with CPM monitoring?
- [ ] What is the unit for monitoring and controlling the schedule in CCPM?

---

layout: center
---

# Practical Case of CPM

---

# Practical Case of CPM

| Task | Duration | Predecessor | Lag |
|------|----------|-------------|-----|
| A | 3 | - | 0 |
| B | 4 | - | 0 |
| C | 5 | FS(A/B) | 0 / -1 |
| D | 2 | FS(C) | 0 |
| E | 3 | FS(D) | +1 |
| F | 4 | FS(D/E) | +1 / -1 |

<div class="section-break"></div>

- [ ] ES for A?
- [ ] LS for D?
- [ ] LF for C?
- [ ] Total Slack for D?

---

# Another Example

<div class="text-center">

images/example-network.png

</div>

<div class="section-break"></div>

- [ ] Total Slack and Free Slack for E?
- [ ] Total Slack and Free Slack for B?

---

layout: center
---

# CCPM Case

---

# CCPM Case

| Task | Dur | Pred | Lag | Res-A | Res-B |
|------|------|------|------|------|------|
| A | 3 | - | 0 | 2 | 1 |
| B | 4 | - | 0 | 2 | 2 |
| C | 5 | FS(A/B) | 0 / -1 | 3 | 1 |
| D | 2 | FS(C) | 0 | 2 | 2 |
| E | 6 | FS(B) | 0 | 2 | 3 |
| F | 4 | FS(D) | -1 | 3 | 1 |

<div class="profession-panel">

**Resource limits**

- Resource A = 3
- Resource B = 3

</div>

<div class="section-break"></div>

- [ ] ES for E?
- [ ] LS for E?

---

# Proposed Solution

<div class="text-center">

images/ccpm-solution.png

</div>

---

# But...

<div class="grid grid-cols-2 gap-4">

<div>

images/ccpm-alternative-01.png

</div>

<div>

images/ccpm-alternative-02.png

</div>

</div>

---

# Other Concepts

- [ ] What is the time baseline? Why do we use it?
- [ ] What about resource control? Is it relevant regardless of the scheduling method?
- [ ] What are the main hypotheses of PERT?
- [ ] Does PERT help in the same way when used by the Project Owner and by the Project Manager?
- [ ] Have we already made a decision in the practical assignment regarding the use of a PMIS?

---

layout: center
class: text-center
---

# Discussion

Questions?