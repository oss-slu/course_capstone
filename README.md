# CS Capstone — Open Source Software Development

A capstone course where you contribute to a real open source software product as a developer, working in sprints alongside a team to deliver working software over a full semester.

## Getting Started

The **Welcome** module orients you to the course and helps you select a project:

- **Welcome Presentation** — a short video and slides introducing the course structure and expectations
- **Product Abstracts** — descriptions of the available client-based projects you can join
- **Pre-Registration Survey** — submit your project preferences early so teams can form

## Resources & Information

The **Resources & Information** module provides materials you'll reference throughout the semester:

- **Developer Handbook** — the [Developer Handbook](https://github.com/oss-slu/handbook_developer) is your primary guide for development practices, workflows, and expectations
- **BLA3DE** — a structured activity for learning about your assigned product's Background, Landscape, Architecture, Data, Dependencies, and Environment
- **Scheduling 1:1 Meetings** — guidelines for constructive feedback sessions with your Tech Lead
- **Conference Travel Stipend** — information about travel support for open source conferences
- **Excellence** — a semester-long assignment for students aiming for A-level performance

## Sprint Structure & Schedule

The semester follows a two-week sprint cycle. The **Sprint Structure & Expectations** page explains how sprints work and what's expected of you as a developer — read it early.

Each sprint runs Monday to Monday. Your core responsibilities each sprint:

- Pick up issues from the backlog and deliver working code
- Raise PRs by the end of Week 1
- Respond to code review feedback in Week 2
- Submit a Sprint Close report at the end of each sprint

## The Semester at a Glance

### Sprint 0 (Jan 13–26) — Onboarding

- **Project Pre-Registration** — confirm your project assignment
- **Team Formation & Onboarding** — set up your development environment, meet your team, complete BLA3DE

### Sprints 1–3 (Jan 27–Mar 9) — Iteration 1

- **Sprint 1** includes a **Team Working Agreement** checkpoint, a **Peer Code Review** good practice, and your first Sprint Close
- **Sprint 2** includes a **Team Outing** checkpoint and **Client Demo & Feedback 1** (bonus)
- **Sprint 3** includes a **Team Retrospective** checkpoint
- Iteration 1 ends with **Milestone 1** and a **Performance Evaluation — Iteration Check-Up**

### Spring Break (Mar 10–15)

### Sprints 4–6 (Mar 16–Apr 27) — Iteration 2

- **Sprint 4** includes **Client Demo & Feedback 2** (bonus) and a second **Retrospective**
- **Sprint 5** includes a **Poster Presentation Draft** checkpoint for the SSE Undergraduate Showcase
- **Sprint 6** is the final development sprint
- Iteration 2 ends with **Milestone 2** and a second **Performance Evaluation**

### Launch & Course Reflection (Apr 28–May 11)

The final phase shifts from development to delivery and reflection:

- **Team Presentation** — present your work to the class
- **Working Software Submission** — deliver functional, merged software
- **Excellence** — demonstrate growth beyond baseline expectations
- **Retrospective #3** — final team reflection
- **Performance Evaluation — Final Review** — comprehensive semester evaluation

## Repository Structure

This repository holds the source materials used to build and deliver the course through Canvas. Students access course content through Canvas directly — this repo is the behind-the-scenes source.

```
assignments/    Assignment definitions (Markdown + YAML metadata)
content/        Long-form course content and page text
files/          Static files distributed through Canvas (PDFs, presentations, videos)
issues/         GitHub Issues for instructor course management
quizzes/        Quiz definitions (Markdown + YAML metadata)
modules.yaml    Canvas module structure and ordering
course-info.yaml  Per-instance course configuration
```

If you spot an error or have a suggestion for improving course materials, feel free to submit a pull request.

For course administration (creating new instances, provisioning tooling), see [ADMINISTERING.md](ADMINISTERING.md).
