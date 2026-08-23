---
title: "Welcome to Capstone: Start Here Before Monday"
type: announcement
published: true
send_at: sprint_0_first_session_minus_1
---

<!--
REUSE NOTES

Sent at the start of each semester, before the first full Monday session.

MosTidy does not yet insert announcements (`canvas insert` handles files,
assignments, quizzes, pages, and modules only). Post this manually, or via the
Canvas API:

    POST /api/v1/courses/{course_id}/discussion_topics
      title=...  message=<html>  is_announcement=true

The five links below are Canvas MODULE ITEM ids, which are unique per course
instance. They MUST be re-resolved each semester. To collect them:

    GET /api/v1/courses/{course_id}/modules
    GET /api/v1/courses/{course_id}/modules/{module_id}/items

Fall 2026 values (course 92754) are recorded inline as a worked example.

Placeholders:
  {first_session}       first full Monday session, e.g. "Monday, August 24"
  {class_time}          e.g. "4:10-5:50 p.m."
  {survey_deadline}     e.g. "4:00 p.m. Monday, August 24"
  {video_url}           Welcome video module item
  {slides_url}          Welcome presentation slides module item
  {abstracts_url}       Product Abstracts page module item
  {syllabus_url}        Syllabus file module item
  {survey_url}          Pre-registration survey (external MS Form)
-->

Welcome to Capstone. Our first full session together is **{first_session},
{class_time}**.

Before then, please work through the items below. The survey is the only thing you
need to submit, and it drives how teams get formed, so please do not skip it.

**1. Watch the welcome video (about 15 minutes)**
{video_url}
Recorded in a prior semester. The program structure it describes still holds.

**2. Review the welcome presentation slides**
{slides_url}
Updated for this semester and reflects how things are organized now.

**3. Read the Product Abstracts**
{abstracts_url}
Teams support **multiple related products** rather than one. You will be joining a
team, not a single product, and you can expect to contribute across more than one of
its products. Read these carefully before ranking your preferences.

**4. Review the syllabus**
{syllabus_url}

**5. Fill out the Capstone Project Pre-Registration Survey**
{survey_url}
Due **{survey_deadline}**. This is where you tell me which teams interest you. There
is also a separate section for unconfirmed teams that may or may not run. Indicating
interest there does not affect your ranked preferences for the confirmed teams.

Bring questions on Monday. See you then.

<!--
FALL 2026 RESOLVED VALUES (course 92754), for reference:

  first_session    Monday, August 24
  class_time       4:10-5:50 p.m.
  survey_deadline  4:00 p.m. Monday, August 24
  video_url        https://canvas.slu.edu/courses/92754/modules/items/2755688
  slides_url       https://canvas.slu.edu/courses/92754/modules/items/2770708
  abstracts_url    https://canvas.slu.edu/courses/92754/modules/items/2755690
  syllabus_url     https://canvas.slu.edu/courses/92754/modules/items/2755862
  survey_url       https://forms.cloud.microsoft/r/fgk6RFSPqX
-->
