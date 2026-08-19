---
title: Exception Reports
url: exception_reports
published: true
front_page: false
---

When you deviate from an expected norm—missing a deadline or adapting a recommended process—you owe a written account. This document explains what that account looks like, why it matters, and how to write one well.

## Why Exception Reports Exist

In professional settings, exceptions to commitments and processes require transparent communication. A missed deadline doesn't disappear because no one mentioned it. A skipped step isn't validated just because the code still works. The written record is what makes the difference between professional judgment and avoidance.

The sprint structure has clear expectations: PRs raised by Week 1, code reviews completed by Week 2, sprint close submitted on time. When something doesn't go as expected, the exception report is how you account for it—to your Tech Lead, to the instructor, and to yourself.

**"Exception" means departure from the expected norm—not inherently negative.** A well-reasoned process adaptation is a positive exception. The report exists to make your reasoning visible, not to punish you for deviating.

This is a learning objective. The ability to communicate transparently about variations from plan is a professional skill that distinguishes effective developers from those who hope problems go unnoticed.

---

## Two Types of Exceptions

### Deadline Misses

You committed to a date and didn't meet it. The commitment was explicit—published in Canvas, established by sprint structure, or agreed to with your Tech Lead. The report explains what happened and what you did about it.

**Examples**: Your PR wasn't raised by the Week 1 Monday deadline. You missed a sprint close submission. You didn't complete a code review you were assigned.

### Process Adaptations

You deliberately changed how you work. The recommended practice exists for good reasons; your adaptation should be grounded in better reasons for your specific context.

The course values contextual judgment over blind compliance. But adaptation without documentation is indistinguishable from ignorance. The report is what makes the difference.

**Examples**: You skipped the draft PR step because your issue was small enough to review in one pass—and you can explain why that was appropriate. You worked outside your assigned issue because you discovered a blocking bug—and you documented the decision before switching. You used a different testing approach than what your team agreed on—and the reasoning holds up to scrutiny.

---

## The Exception Report Format

Every exception report includes these elements:

### Summary
One sentence: what varied and when.

> *"My Sprint 3 PR was raised on Wednesday instead of the Monday deadline."*
> *"I skipped the draft PR step for issue #47 and opened it directly as ready for review."*

### Context
What was the expectation, and what actually happened? Be specific—reference the deadline, the recommended practice, or the agreement with your Tech Lead.

### Evidence
Concrete artifacts that corroborate your account. These must be **attached or linked**, not just described:

- Commit history and PR timelines
- Slack or Discord message threads
- Work logs or time tracking
- GitHub issue comments
- Messages to your Tech Lead

"I was working on it all week" is a claim. Your commit history showing steady work through Tuesday followed by silence through Friday is evidence.

### Reasoning
A causal account connecting circumstances to the outcome. What decisions were made, when, and why? This is the core of the report—walk through the sequence of events and decisions that led to the variation.

### Alternatives Considered
What other options were available, and why were they not selected? This demonstrates that the exception was a deliberate choice—or, in the case of a deadline miss, that you considered recovery options.

### Impact
What was affected—your team's sprint, the deliverable, someone else's code review schedule—and what was done to mitigate the impact.

### Going Forward
For deadline misses: what changes will prevent recurrence? Be concrete—"I'll start earlier" is not a change. "I'll raise a draft PR by Thursday even if the implementation is incomplete, so my Tech Lead has visibility" is a change.

For process adaptations: what did you learn? Would you make the same choice again? Under what conditions would you revert to the recommended practice?

---

## Reasoning vs. Rationalization

The difference matters, and it's worth being explicit about it.

**Reasoning** works forward from evidence to conclusion. You observed something, evaluated options, and made a decision. The evidence came first; the conclusion followed.

**Rationalization** works backward from a desired conclusion to cherry-picked justification. You already know what you want to say happened, and you're selecting facts to support it.

A useful test: **could a skeptical peer follow your evidence to the same conclusion?** If your account requires the reader to already agree with you in order to find it persuasive, you're rationalizing.

|                  | Reasoning                        | Rationalization                  |
| ---------------- | -------------------------------- | -------------------------------- |
| **Direction**    | Evidence → conclusion            | Conclusion → supporting evidence |
| **Completeness** | Includes inconvenient facts      | Omits anything that contradicts  |
| **Tone**         | "Here's what happened"           | "It wasn't my fault because..."  |
| **Test**         | A skeptic would follow the logic | Only works if you already agree  |

**Example — deadline miss:**
- **Reasoning**: "I underestimated the complexity of the database migration. By Thursday I realized I wouldn't have a functional PR by Monday, and I messaged my Tech Lead to discuss options. We agreed I'd raise a draft PR with the schema changes and open a second issue for the data migration logic."
- **Rationalization**: "The issue was way bigger than expected. It should have been broken into smaller pieces before the sprint started."

**Example — process adaptation:**
- **Reasoning**: "Issue #47 was a three-line configuration fix. Opening a draft PR, waiting for feedback, then converting to ready-for-review would have added two days to a change that took 15 minutes. I opened it directly as ready-for-review and tagged my Tech Lead in Slack. The review was completed within an hour."
- **Rationalization**: "Draft PRs are busywork for small changes. Everyone knows that."

---

## Timing and Routing

### When to Submit

**Proactive reports**—submitted before or at the time of the variation—are expected and noted favorably. If you know a deadline is at risk, say so before the deadline passes. If you're adapting a process, document the decision when you make it.

**Reactive reports**—submitted after the fact—are accepted but viewed less favorably. Late communication about late work compounds the issue. The exception report itself shouldn't require an exception report.

### Where to Submit

- **Individual exceptions** (your own deadlines, your own process choices): submit to your Tech Lead, who may escalate to the instructor. For matters you'd prefer to discuss directly with the instructor, you may submit to them instead.
- **Team-level exceptions** (missed sprint close, team process adaptation): your team designates a reporter—typically the person closest to the situation—who files on behalf of the team.

---

## How Reports Are Evaluated

Exception reports are acknowledged and factor into performance evaluations. They are not graded as standalone assignments—they exist alongside the work they describe.

**Quality of reasoning matters.** A well-documented variation demonstrates professional maturity. A vague or defensive report suggests the underlying issue hasn't been understood.

**One exception report is normal.** Things happen—schedules conflict, technical surprises arise, reasonable people adapt. A pattern of reports, however, is itself a signal worth examining. If you're filing exception reports every sprint, the exceptions may be symptoms of a deeper issue that needs direct attention.

**There is no approve/deny.** The report is not a permission request. The variation already happened (or is happening). The report makes the reasoning visible so it can be evaluated in context—alongside your other work, your contributions to the team, and the overall pattern of your performance.
