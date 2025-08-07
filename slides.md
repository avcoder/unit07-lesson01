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
Deployment: Unit 07 - Lesson 01

- [ ] Various Deployment Strategies
- [ ] Microservices vs Monolithic Architectures
- [ ] Deployment Examples

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
transition: slide-left
---

# Processes Involved in Web Deployment

- Testing #1: to ensure the application works locally before going live
   - Unit testing, Integration testing, End-to-End testing, Automated testing in CI/CD pipelines
- Testing #2: to ensure application still works in staging (just before it gets deployed to prod)
  - Watch me [test on staging](https://www.loom.com/share/d3b4d1c3c7f64ffebeee0a6a9dfc5cc7?sid=2329b9da-90bb-4901-a41d-4d348179e26f) for my former workplace 
- Testing #3: Once deployed, test one more time to make sure everything looks/functions correctly
- Monitoring:
  - Tools like Sentry can capture runtime errors and log them
  - DevOps team can monitor real-time server health and performance, as well as rollback if needed

---
transition: slide-left
---

# Exercise
5 min

1. Use [excalidraw](https://excalidraw.com/) to draw a simple diagram of the architecture of our Express/MongoDB/EJS app
2. Now draw a 2nd diagram of the architecture of an Express (JSON API)/MongoDB/React app
3. Once done, click "Share" > Export to Link > Copy link, then paste it in chat 

---
transition: slide-left
---

# Architecture

- Right now, all of this runs on your computer, but how do we make this available to the world?
  - Each piece (frontend, backend, DB) needs to live somewhere online (ex: Netlify, Render, MongoDB Atlas)
- Examine the Fetch/XHR requests on Network tab for app.agencyanalytics.com - where does it go?
- Exercise: Draw a diagram on excalidraw showing how the app is architected
- How can your Express backend and React Frontend be deployed in similar fashion?

---
transition: slide-left
---

# Architecture: Monolithic vs Microservice vs. Other

- Monolithic App: One codebase that contains everything: frontend, backend, and logic together.
  - ex: The Note-taking app you built
- Microservices: Different services doing different tasks, each deployable separately.
  - ex: One service for user auth, another for task management, another for notifications.
- Other: Somewhere in between where it's modular or decoupled

| Feature    | Monolith   | Microservices              |
| ---------- | ---------- | -------------------------- |
| Codebase   | Single     | Multiple                   |
| Deployment | One deploy | Many deploys               |
| Scaling    | Harder     | Easier (scale per service) |
| Good for   | Small apps | Large apps with teams      |

---
transition: slide-left
---

# What kind of architecture might the following be?

- front-end React code stored in one Github repo, perhaps hosted on Netlify/Vercel
- back-end Node/Express JSON APIs stored on another Github repo, perhaps hosted on render
- Mongo DB hosted on cloud (Atlas) 

| Feature    | Architecture   | 
| ---------- | ---------- | 
| Frontend & backend separated?   | ✅ Yes     | 
| Independent deployment? | ✅ Yes | 
| Multiple microservices?    | ❌ No (single backend)     | 
| Shared DB?  | ✅ MongoDB Atlas | 
| Monolithic? | ❌ No |
| Microservices? | ⚠️ Not quite |


---
transition: slide-left
---

# Architecture: Modular or Decoupled

- Previous slide described what might be called Decoupled / Modular Architecture
- Since frontend and backend are separated into different services and repositories, this is already one major step away from a monolith
- This modularity allows independent deployment and scaling of frontend / backend
- It also borrows some microservices principles:
   - independent deployment pipelines
   - separation of concerns
   - individual hosting environments

---
transition: slide-left
---

# Deployment Foundations 

| **Topic**                        | **Subtopics**                                                                              |
| -------------------------------- | ------------------------------------------------------------------------------------------ |
| **Version Control Systems**      | - Git overview<br>- Why version control matters                      |
| **Using Branches**               | - Naming conventions (`feature/`, `bugfix/`, etc.)<br>- Merging & pull requests            |
| **Local vs. Remote Development** | - Local setup vs. staging/production environments<br>- Tools like VS Code, Docker, etc.    |
| **Scheduling & Timing**          | - Deploying during low-traffic hours (not Fridays)<br>- CI/CD pipeline triggers (GitHub Actions)         |
| **Environment Variables**        | - `.env` files<br>- Keeping secrets out of source code|


---
layout: image-right
transition: slide-left
image: /assets/netlify.png
backgroundSize: 400px 400px
class: text-left
---

# 10 minute break

🍦 Cool Tips, Trends and Resources:
- 🚢 [What is Deployment](https://umbraco.com/knowledge-base/deployment/)
- 🌴 [Growthbook FeatureFlag Tool](https://www.growthbook.io/get-started)
- 🎭 [Playwright](https://playwright.dev/)
- 8️⃣ [Kubernetes](https://kubernetes.io/)
- 📦 [Docker](https://www.docker.com/)
- 💯 [Vitest](https://vitest.dev/)
- 📝 [React Testing Library](https://testing-library.com/docs/react-testing-library/intro/)
- 🎧 [MixPanel](https://mixpanel.com/home/)

<br>
<hr>
<br>

- 🧪 [Enter anonymous lab questions](https://docs.google.com/forms/d/e/1FAIpQLSevvGARdHQikso-uLqFCO481MABKE5HofuSrlzEPMNQ2ZLykw/viewform?usp=dialog)
- ℹ️ [Course feedback survey](https://circuitstream.typeform.com/to/ZoyYk7px#course_id=SoftwareAN&instructor=9514)

---
transition: slide-left
---

# Exercise

- Deploy https://github.com/avcoder/deploy-front to Netlify or other
- Deploy https://github.com/avcoder/deploy-back to Render or other
- What issues come up when trying to make it work.  How did you resolve it?

---
transition: slide-left
---

# Homework

- Work on your "Algorithm and Structural Foundations" assignment due July 20 midnight EST
   - can submit before due date if you wish