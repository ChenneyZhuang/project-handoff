---
name: project-handoff
description: |
  Keep a cross-session project continuable: maintain a handoff.md at the
  project root that any fresh session or different agent can read to get full
  context — what the project is, current state, decisions with their reasons,
  pitfalls as symptom/cause/fix, and dated next steps. Read it before starting
  work on a known project; create it after finishing work that will continue;
  update it the moment a milestone lands. Use when starting a session on an
  ongoing project, resuming after a gap, delegating a project to another agent
  or teammate, or closing out a work session on something long-lived.
  触发词：项目交接 / handoff / 接手项目 / 跨会话上下文。
license: MIT
metadata:
  version: "0.1.0"
---

# Project Handoff: make the next session as smart as this one

Long projects die in chat history: the context that matters lives in messages
that scroll away, get compressed, or belong to a session that has since ended.
A handoff file is the project's memory on disk — one markdown file the next
session reads first and this session updates last.

## Rules

1. **One handoff file per project, at the project root.** Fixed name
   (`handoff.md`), fixed home. It is the first thing a session reads and the
   last thing a session updates.
2. **Read before you build.** Starting work on an existing project means
   reading the handoff first. The fastest way to redo finished work is to
   skip this.
3. **Update when it lands, not later.** Milestone completed, decision made,
   pitfall discovered — write it immediately. A handoff updated "at the end
   of the day" records yesterday's project.
4. **State over narrative.** Record what is true now: versions, paths,
   counts, statuses. History belongs in version control; the handoff holds
   the current picture and the decisions behind it.
5. **Pitfalls are the payload.** The most valuable lines save the next
   session from a known trap. Write them as symptom → cause → fix: the
   command that fails, the setting that looks wrong but is right, the step
   that must run in order.
6. **Decisions carry their why.** "Use X" is a fact; "Use X because Y,
   rejected Z" is a decision the next session can respect or consciously
   revisit. Without the why, the next session relitigates it.
7. **Sensitive facts stay out.** The handoff is a working file that may be
   synced, shared, or published: credentials, client identifiers, and
   personal details live in dedicated stores, and the handoff points at where
   they live.
8. **Mark the date.** Every entry carries a date, so the reader can judge
   staleness instead of guessing.

## Steps

1. **Orient (existing project).** Read the handoff, then verify its claims
   against reality: do the listed paths exist, do the stated counts and
   statuses match the current files? Correct stale lines in place as you find
   them.
   Done when: every load-bearing claim is either confirmed or corrected.
2. **Create (new project).** The project will span sessions and no handoff
   exists: create it now with the five sections — what/why, current state,
   next steps, decisions, pitfalls.
   Done when: the file exists at the project root with all five sections.
3. **Work.** Do the task.
4. **Update.** Refresh current state, tick or rewrite next steps, append
   decisions with their reasons, add pitfalls as symptom → cause → fix, and
   date the entries.
   Done when: a fresh reader could resume the project from the file alone,
   with no claim contradicting the project's actual state.
5. **Close the loop.** When the session ends, the handoff's next-steps
   section names the next concrete action.
   Done when: next steps contains at least one dated, actionable item.

## Done when

The handoff exists, matches reality, carries the session's new knowledge
(decisions with reasons, pitfalls, current state), and leaves the next
session an actionable, dated starting point.
