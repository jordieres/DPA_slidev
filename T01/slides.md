---
# try also 'default' to start simple
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: /images/Designer.png  # https://cover.sli.dev
# some information about your slides (markdown enabled)
title: Advanced Project Management Course
info: |
  # Master in Organizational Engineering
  Academic Year 2026-27 (https://apiivm01.etsii.upm.es/~jordieres/DPA/T01/)
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

# Advanced Project Management

## First steps

<div @click="$slidev.nav.next" class="mt-12 py-1" hover:bg="grey op-10">
  Press Space for next page <carbon:arrow-right />
</div>

<div class="abs-br m-6 text-xl">
  <button @click="$slidev.nav.openInEditor()" title="Open in Editor" class="slidev-icon-btn">
    <carbon:edit />
  </button>
  <a href="https://github.com/jordieres/DPA_slidev/" target="_blank"      class="slidev-icon-btn">
    <carbon:logo-github />
  </a>
</div>

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---
title: "PM: What Does It Mean?"
layout: default
transition: fade-out
---

## Course Motivation: DPA

### Project Management as a Profession in Its Own Right

<div class="mt-10 text-sm opacity-70">
  Updated with labour-market and professional evidence available in 2025–26
</div>

<br />

<div class="profession-panel motivation-list">

- <span v-click>A <strong>technical expert</strong> knows how to design or build the project’s outputs.</span>
- <span v-click>A <strong>functional manager</strong> maintains an organizational capability over time.</span>
- <span v-click>A <strong>Project Manager</strong> integrates people, decisions, resources, uncertainty and stakeholders to deliver a temporary change.</span>

</div>

<div v-click class="big-statement">

Project management is not simply “general management applied to a project.” It has a **distinct object, temporary governance structures, dedicated practices and identifiable accountability** for value delivery.
</div>

---
title: "When Can We Call Something a Profession?"
layout: default
transition: fade-out
---

<div class="visual-chain">
  <div v-click class="visual-node"><div class="icon">🎯</div><div class="node-title">Social function</div><div class="node-sub">Deliver complex change and value</div></div>
  <div class="visual-arrow">→</div>
  <div v-click class="visual-node"><div class="icon">🧠</div><div class="node-title">Specialized knowledge</div><div class="node-sub">Methods, tools and judgement</div></div>
  <div class="visual-arrow">→</div>
  <div v-click class="visual-node"><div class="icon">🪪</div><div class="node-title">Occupational identity</div><div class="node-sub">Recognized roles and careers</div></div>
</div>

<div class="visual-chain">
  <div v-click class="visual-node"><div class="icon">📏</div><div class="node-title">Standards and ethics</div><div class="node-sub">Shared practices and conduct</div></div>
  <div class="visual-arrow">→</div>
  <div v-click class="visual-node"><div class="icon">✅</div><div class="node-title">Competence assurance</div><div class="node-sub">Education, experience and assessment</div></div>
  <div class="visual-arrow">→</div>
  <div v-click class="visual-node"><div class="icon">🌐</div><div class="node-title">Professional community</div><div class="node-sub">Institutions, research and CPD</div></div>
</div>

<div v-click class="profession-panel warning motivation-list compact" style="margin-top:.5rem">

<br />

<strong>Important distinction:</strong> project management can be a profession <em>per se</em> without being a legally regulated profession in every jurisdiction. “Professionalized” and “statutorily licensed” are not synonyms.

</div>

---
title: "An Occupation Recognized in Its Own Right"
layout: default
transition: fade-out
---

<div class="evidence-grid">
  <div v-click class="evidence-card">
    <div class="metric">13-1082</div>
    <div class="label">Dedicated US occupational code for Project Management Specialists</div>
  </div>
  <div v-click class="evidence-card">
    <div class="metric">1.046M</div>
    <div class="label">Jobs in the United States in 2024</div>
  </div>
  <div v-click class="evidence-card">
    <div class="metric">78,200</div>
    <div class="label">Average projected openings per year, 2024–34</div>
  </div>
</div>

<div v-click class="profession-panel motivation-list compact" style="margin-top:.6rem">

The US Bureau of Labor Statistics defines common duties across industries: establishing scope and goals, planning activities and resources, estimating cost and risk, coordinating stakeholders, monitoring milestones and deliverables, managing change and closing the project.

<div class="source-note">Source: <a href="https://www.bls.gov/ooh/business-and-financial/project-management-specialists.htm" target="_blank">US Bureau of Labor Statistics, Project Management Specialists</a>, 2024 employment and 2024–34 projections; page updated August 2025.</div>

</div>


<div class="evidence-grid">
  <div v-click class="evidence-card">
    <div class="metric">39.6M</div>
    <div class="label">Project professionals worldwide in 2025</div>
  </div>
  <div v-click class="evidence-card">
    <div class="metric">+64%</div>
    <div class="label">Potential growth in global demand from 2025 to 2035</div>
  </div>
  <div v-click class="evidence-card">
    <div class="metric">29.8M</div>
    <div class="label">Potential shortfall of qualified professionals by 2035</div>
  </div>
</div>

<div v-click class="big-statement" style="font-size:.88em">
The current global population of project professionals is already comparable in scale to major established occupations. The issue is no longer whether the role exists, but whether the supply of competent professionals can keep pace with transformation.

<div class="source-note">Source: <a href="https://www.pmi.org/learning/thought-leadership/global-project-management-talent-gap" target="_blank">PMI, Global Project Management Talent Gap</a>, May 2025. Estimates combine PMI workforce analysis with LinkedIn Talent Insights.</div>

</div>


---
title: "Demand Is Structural, Not Sector-Specific"
layout: default
transition: fade-out
---

<div class="sector-wheel">
  <div v-click class="sector"><div class="icon">🤖</div><div class="name">Digital & AI</div></div>
  <div v-click class="sector"><div class="icon">🏗️</div><div class="name">Infrastructure</div></div>
  <div v-click class="sector"><div class="icon">🌱</div><div class="name">Energy transition</div></div>
  <div v-click class="sector"><div class="icon">🏥</div><div class="name">Healthcare</div></div>
  <div v-click class="sector"><div class="icon">🏭</div><div class="name">Manufacturing</div></div>
</div>

<div v-click class="big-statement" style="font-size:.80em;margin:.55rem auto">
Different outputs; the same professional challenge: integrate technology, organizations, resources, uncertainty, adoption and benefits.
</div>

<div v-click class="profession-panel motivation-list compact" style="margin-top:.55rem">

PMI identifies construction, manufacturing, IT services and healthcare among the sectors under the greatest pressure, with demand in some sectors projected to increase by as much as <strong>66%</strong>. Project managers were also identified as a major net-growth role in the World Economic Forum’s <em>Future of Jobs Report 2025</em>.

<div class="source-note">Sources: <a href="https://www.pmi.org/about/press-media/2025/shortage-of-project-talent-endangers-global-growth" target="_blank">PMI Talent Gap press release</a>, 7 May 2025; <a href="https://www.weforum.org/publications/the-future-of-jobs-report-2025/" target="_blank">World Economic Forum, Future of Jobs Report 2025</a>.</div>

</div>



---
title: "A Specific and Evolving Body of Knowledge"
layout: default
transition: fade-out
---

<div class="iso-track">
  <div v-click class="iso-item"><div class="code">ISO 21500</div><div class="topic">Context & concepts<br>2021</div></div>
  <div v-click class="iso-item"><div class="code">ISO 21502</div><div class="topic">Project-management practices<br>2020</div></div>
  <div v-click class="iso-item"><div class="code">ISO 21505</div><div class="topic">Governance<br>2017</div></div>
  <div v-click class="iso-item"><div class="code">ISO 21506</div><div class="topic">Vocabulary<br>2024</div></div>
  <div v-click class="iso-item"><div class="code">ISO 21511</div><div class="topic">Work breakdown structures</div></div>
  <div v-click class="iso-item"><div class="code">ISO 21508 / 12</div><div class="topic">Earned value management<br>2024–26</div></div>
  <div v-click class="iso-item future"><div class="code">ISO 21515</div><div class="topic">Professional competence<br>in development</div></div>
  <div v-click class="iso-item future"><div class="code">ISO 21520</div><div class="topic">AI and project management<br>in development</div></div>
</div>

<div v-click class="profession-panel motivation-list compact" style="margin-top:.4rem">

This is evidence of a field with its own language, governance concepts, practices, performance-control methods and evolving competence requirements—not merely a generic managerial title.

<div class="source-note">Sources: <a href="https://committee.iso.org/sites/tc258/home/projects.html" target="_blank">ISO/TC 258 portfolio of standards</a>; <a href="https://www.iso.org/standard/74947.html" target="_blank">ISO 21502:2020</a>.</div>

</div>



---
title: "The Labour Market Places a Premium on the Role"
layout: default
transition: fade-out
---

<div class="bar-chart">
  <div style="font-size:.82rem;font-weight:700;margin-bottom:.4rem">US median annual pay, May 2024</div>
  <div v-click class="bar-row"><div>Project-management specialists</div><div class="bar-bg"><div class="bar-fill" style="width:91%"></div></div><div class="bar-value">$100,750</div></div>
  <div v-click class="bar-row"><div>Business-operations specialists</div><div class="bar-bg"><div class="bar-fill alt" style="width:73%"></div></div><div class="bar-value">$80,410</div></div>
  <div v-click class="bar-row"><div>All occupations</div><div class="bar-bg"><div class="bar-fill alt" style="width:45%"></div></div><div class="bar-value">$49,500</div></div>
</div>

<div class="bar-chart">
  <div style="font-size:.82rem;font-weight:700;margin-bottom:.4rem">US employment growth, 2024–34</div>
  <div v-click class="bar-row"><div>Project-management specialists</div><div class="bar-bg"><div class="bar-fill" style="width:100%"></div></div><div class="bar-value">6%</div></div>
  <div v-click class="bar-row"><div>All occupations</div><div class="bar-bg"><div class="bar-fill alt" style="width:50%"></div></div><div class="bar-value">3%</div></div>
</div>

<div v-click class="source-note">Source: <a href="https://www.bls.gov/ooh/business-and-financial/project-management-specialists.htm" target="_blank">US Bureau of Labor Statistics</a>. These are US occupational statistics, not globally comparable salary figures.</div>

---
title: "Competence and Credentials Have Market Value"
layout: default
transition: fade-out
---

<div class="evidence-grid two">
  <div v-click class="evidence-card">
    <div class="metric">20,000+</div>
    <div class="label">Professionals represented in PMI’s 14th Salary Survey</div>
  </div>
  <div v-click class="evidence-card">
    <div class="metric">21</div>
    <div class="label">Countries covered by the salary comparison</div>
  </div>
  <div v-click class="evidence-card">
    <div class="metric">+17%</div>
    <div class="label">Median salary reported by PMP holders versus non-holders across the surveyed countries</div>
  </div>
  <div v-click class="evidence-card">
    <div class="metric">3+ years</div>
    <div class="label">Leadership experience associated with PMP eligibility routes</div>
  </div>
</div>

<br />

<div v-click class="profession-panel warning motivation-list compact" style="margin-top:.5rem">

The salary premium is an association, not proof that certification itself causes higher pay: experience, responsibility, country, sector and employer selection also matter. Nevertheless, employers and professionals demonstrably assign economic value to validated PM competence.

<div class="source-note">Sources: <a href="https://www.pmi.org/learning/careers/project-management-salary-survey" target="_blank">PMI Salary Survey, 14th edition</a>; <a href="https://www.pmi.org/blog/pmp-certification" target="_blank">PMI’s 2026 summary of the latest survey results</a>.</div>

</div>



---
title: "Indicative Salary Snapshots across Major Economies"
layout: default
transition: fade-out
---

<div class="salary-grid">
  <div v-click class="salary-card"><div><span class="flag">🇺🇸</span> <span class="country">United States</span></div><div class="salary">$100.8K</div><div class="range-line"></div><div class="dot"></div><div class="range">Median annual wage · PM specialists · May 2024</div></div>
  <div v-click class="salary-card"><div><span class="flag">🇬🇧</span> <span class="country">United Kingdom</span></div><div class="salary">£52.5K</div><div class="range-line"></div><div class="dot"></div><div class="range">Average PM salary · APM survey 2025</div></div>
  <div v-click class="salary-card"><div><span class="flag">🇩🇪</span> <span class="country">Germany</span></div><div class="salary">€92.6K</div><div class="range-line"></div><div class="dot"></div><div class="range">Median total compensation · P25 €74.9K · P75 €103K</div></div>
  <div v-click class="salary-card"><div><span class="flag">🇫🇷</span> <span class="country">France</span></div><div class="salary">€55.8K</div><div class="range-line"></div><div class="dot"></div><div class="range">Median total compensation · P25 €44.4K · P75 €71.1K</div></div>
  <div v-click class="salary-card"><div><span class="flag">🇪🇸</span> <span class="country">Spain — Madrid</span></div><div class="salary">€45K</div><div class="range-line"></div><div class="dot"></div><div class="range">Median total pay · reported range €32K–€58K</div></div>
  <div v-click class="salary-card" style="display:flex;align-items:center;text-align:center"><div class="range"><strong>Do not rank these values directly.</strong><br>Different role definitions, samples, coverage and compensation concepts.</div></div>
</div>

<div v-click class="source-note">Sources: <a href="https://www.bls.gov/ooh/business-and-financial/project-management-specialists.htm" target="_blank">BLS, USA</a>; <a href="https://www.apm.org.uk/project-management-salary-survey/" target="_blank">APM Salary Survey 2025, UK</a>; <a href="https://www.levels.fyi/t/project-manager/locations/germany" target="_blank">Levels.fyi, Germany</a>; <a href="https://www.levels.fyi/t/project-manager/locations/france" target="_blank">Levels.fyi, France</a>; <a href="https://www.glassdoor.com/Salaries/madrid-spain-project-manager-salary-SRCH_IL.0,12_IM1030_KO13,28.htm" target="_blank">Glassdoor, Madrid</a>. European platform data accessed 14 August 2026.</div>


<div class="visual-chain">
  <div v-click class="visual-node"><div class="icon">🛒</div><div class="node-title">Purchasing power</div><div class="node-sub">Local cost of living</div></div>
  <div class="visual-arrow">+</div>
  <div v-click class="visual-node"><div class="icon">🏛️</div><div class="node-title">Tax & benefits</div><div class="node-sub">Net income and social protection</div></div>
  <div class="visual-arrow">+</div>
  <div v-click class="visual-node"><div class="icon">🧭</div><div class="node-title">Role scope</div><div class="node-sub">Authority, complexity and seniority</div></div>
</div>

<div class="visual-chain">
  <div v-click class="visual-node"><div class="icon">🏢</div><div class="node-title">Market context</div><div class="node-sub">Sector, firm size and city</div></div>
  <div class="visual-arrow">+</div>
  <div v-click class="visual-node"><div class="icon">📊</div><div class="node-title">Survey design</div><div class="node-sub">Sample and compensation definition</div></div>
  <div class="visual-arrow">→</div>
  <div v-click class="visual-node"><div class="icon">⚖️</div><div class="node-title">Comparable value</div><div class="node-sub">Only after harmonization</div></div>
</div>

<div v-click class="source-note">Salary snapshots illustrate active labour markets; they do not constitute a harmonized international ranking. PMI’s 14th Salary Survey provides a more consistent 21-country framework, but its detailed interactive country data are restricted to members.</div>

---
title: "AI Changes the Profession; It Does Not Remove It"
layout: default
transition: fade-out
---

<div class="ai-flow">
  <div v-click class="ai-column">
    <h2>🤖 Increasingly augmented</h2>
    <div class="ai-task">Draft schedules, reports and risk registers</div>
    <div class="ai-task">Consolidate data and detect anomalies</div>
    <div class="ai-task">Produce forecasts and scenarios</div>
    <div class="ai-task">Maintain documentation and traceability</div>
    <div class="ai-task">Recommend candidate actions</div>
  </div>
  <div class="ai-arrow">→</div>
  <div v-click class="ai-column">
    <h2>🧑‍💼 Persistently accountable</h2>
    <div class="ai-task">Decide what matters and why</div>
    <div class="ai-task">Negotiate priorities and trade-offs</div>
    <div class="ai-task">Exercise judgement under ambiguity</div>
    <div class="ai-task">Build trust, resolve conflict and lead change</div>
    <div class="ai-task">Own governance, ethics and outcomes</div>
  </div>
</div>

<div v-click class="profession-panel motivation-list compact" style="margin-top:.55rem">

The professional boundary shifts from producing administrative artefacts towards orchestrating socio-technical change, validating AI-supported evidence and remaining accountable for decisions and outcomes.

<div class="source-note">Context: <a href="https://www.weforum.org/publications/the-future-of-jobs-report-2025/" target="_blank">WEF Future of Jobs Report 2025</a> emphasizes the simultaneous rise of technological skills and human capabilities such as analytical thinking, resilience, leadership and collaboration.</div>

</div>



---
title: "Conclusion: Profession Per Se"
layout: default
transition: fade-out
---

<div class="big-statement">
Project management qualifies as a profession in its own right because society and organizations recognize a distinct role, entrust it with consequential accountability, reward specialized competence and sustain a global ecosystem of standards, education, credentials, research and continuing development.
</div>

<div class="motivation-list compact">

- <span v-click><strong>It is not tied to one engineering discipline.</strong></span>
- <span v-click><strong>It is not reducible to administrative coordination.</strong></span>
- <span v-click><strong>It is not necessarily a legally protected profession.</strong></span>
- <span v-click><strong>Professionals are hired independently, depending on the market and geographic area.</strong></span>
- <span v-click><strong>It is a transferable professional capability for delivering change and value.</strong></span>

</div>

---
title: "Sources and Data Boundaries"
layout: default
transition: fade-out
---

<div class="source-list">

- <a href="https://www.pmi.org/learning/thought-leadership/global-project-management-talent-gap" target="_blank">PMI (2025), Global Project Management Talent Gap</a> — global workforce and demand estimates.
- <a href="https://www.bls.gov/ooh/business-and-financial/project-management-specialists.htm" target="_blank">US Bureau of Labor Statistics (2025 update)</a> — US employment, duties, pay and 2024–34 projections.
- <a href="https://www.pmi.org/learning/careers/project-management-salary-survey" target="_blank">PMI, Project Management Salary Survey, 14th edition</a> — survey coverage and credential-related salary comparisons.
- <a href="https://www.weforum.org/publications/the-future-of-jobs-report-2025/" target="_blank">World Economic Forum (2025), Future of Jobs Report</a> — global labour-market and skills context.
- <a href="https://committee.iso.org/sites/tc258/home/projects.html" target="_blank">ISO/TC 258</a> — current standards and standards under development for project, programme and portfolio management.
- <a href="https://www.apm.org.uk/project-management-salary-survey/" target="_blank">APM Salary and Market Trends Survey 2025</a> — United Kingdom project-management salary evidence.
- <a href="https://www.levels.fyi/t/project-manager/locations/germany" target="_blank">Levels.fyi, Germany</a>; <a href="https://www.levels.fyi/t/project-manager/locations/france" target="_blank">Levels.fyi, France</a> — indicative self-reported total-compensation snapshots.
- <a href="https://www.glassdoor.com/Salaries/madrid-spain-project-manager-salary-SRCH_IL.0,12_IM1030_KO13,28.htm" target="_blank">Glassdoor, Madrid</a> — indicative self-reported total-pay snapshot.

</div>

<div class="profession-panel warning motivation-list compact" style="margin-top:.55rem">

<strong>Interpretation limits:</strong> PMI figures include the wider population of “project professionals,” whereas BLS figures refer to the narrower US occupation “Project Management Specialists.” Salary figures from different countries should not be compared without harmonizing purchasing power, role and sample composition.

</div>
