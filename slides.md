---
# You can also start simply with 'default'
theme: default
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: /assets/intro.jpg
# some information about your slides (markdown enabled)
title: Software Development | Foundations
info: |
  ## Software Development | Foundations
# apply unocss classes to the current slide
class: text-left
drawings:
  persist: false
transition: slide-left
mdc: true
---

# Intro to Deployment
Deployment: Unit 07 - Lesson 02

- [ ] Various Deployment Strategies
- [ ] Microservices vs Monolithic Architectures
- [ ] Preparing to Deploy
- [ ] Deployment via FTP

<div class="abs-br m-6 text-xl">
  <a href="https://github.com/slidevjs/slidev" target="_blank" class="slidev-icon-btn">
    <carbon:logo-github />
  </a>
</div>

<!--
-->

---
transition: slide-left
---

# Software Development Life Cycle

<img src="/assets/sdlc.png" style="height: 400px; margin: 0 auto">

---
transition: slide-left
---

# Types of Deployment use-cases:

- Personal deployment: e.g., running code locally using localhost.
- Small applications: deploying to services like Netlify, Vercel, or Heroku.
- Enterprise deployment: CI/CD pipelines, cloud infrastructure (AWS, GCP, Azure).
- Open-source applications: community-driven deployment, contributor coordination.

<img src="/assets/cicd.webp" style="height: 300px; margin: 0 auto" />

---
transition: slide-left
---

# Types of Deployment Strategies

<img src="/assets/deploy1.webp" style="height: 470px; margin: 0 auto">

---
transition: slide-left
---

# Standard Web Deployment Process

- Local: Developer’s personal machine.
- Development: Internal environment for developers to share/test.
- Staging: Mirrors production, for final tests and approvals.
- Live (Production): Public-facing, used by end users.

## Deployment variations
- Some teams skip staging.
- Use of feature flags or canary releases.
- Continuous Deployment vs Manual Deployment.

---
layout: image-right
transition: slide-left
image: /assets/addy.png
backgroundSize: 400px 300px
class: text-left
---

# 10 minute break

🍦 Cool Tips, Trends and Resources:
- 🚢 [What is Deployment](https://umbraco.com/knowledge-base/deployment/)
- 🌴 [Growthbook FeatureFlag Tool](https://www.growthbook.io/get-started)
- 8️⃣ [Kubernetes](https://kubernetes.io/)
- 📦 [Docker](https://www.docker.com/)

<br>
<hr>
<br>

- 🧪 [Enter anonymous lab questions](https://docs.google.com/forms/d/e/1FAIpQLSevvGARdHQikso-uLqFCO481MABKE5HofuSrlzEPMNQ2ZLykw/viewform?usp=dialog)
- ℹ️ [Course feedback survey](https://circuitstream.typeform.com/to/ZoyYk7px#course_id=SoftwareAN&instructor=9514)

---
transition: slide-left
---

# Homework

- Work on your "Algorithm and Structural Foundations" assignment due July 20 midnight EST
   - can submit before due date if you wish