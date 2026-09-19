# Pre-Context Document Prompt (PCDP)

The next message will contain a continuation-ready context document for the **uGTgtdD / gtgtdd-sys** project.

Treat that document as **authoritative context for continuing the work**. Do not summarize, reformat, critique, optimize, redesign, or replace its terminology on receipt.

In particular:

- preserve Dave's existing GTD/uGTgtdD concepts and vocabulary unless he explicitly changes them;
- preserve the project-creation checklist as an **implementation-independent reusable checklist**;
- treat the existing context list as authoritative vocabulary to be mapped into Asana-native mechanisms rather than replaced with a new taxonomy;
- remember that the Asana connection is now working;
- keep the system **lean-to, not cathedral**;
- do not bulk-migrate the backlog before a small real workflow has been proven;
- use Asana's free-plan-compatible/native features where possible rather than making the system depend on premium-only features such as custom fields or timeline;
- use ChatGPT/kamMA as the conductor/orchestrator, not as canonical storage.

After reading the context document, respond only with a brief confirmation that you have received it and are ready to continue.

---

# CONTEXT DOCUMENT for continuation of the "uGTgtdD / gtgtdd-sys — ADHD-adapted action-management system using Asana as the canonical actionable layer, with reusable checklists and Dave's established GTD context vocabulary" project

DOCUMENT PREPARED FOR CONTINUATION:

1789828260_2026-09-19T10:31:00-0400

CONTINUED FROM CHAT ENTITLED:

"ADHD Coaching and Burnout"

ALSO INVOLVING

`(Asana connector setup | Google Keep GTD system | reusable checklists | context vocabulary | job applications | medical/admin | upskilling/portfolio | RMMFB/NTEC | no other subjects required for continuation)`

FROM USER

- (GitHub) @bballdave025

---

## Purpose of This Continuation Document

This is a continuation-ready lab-notebook/context document for the `gtgtdd-sys` project.

It is not polished product documentation. It preserves the design state necessary to resume work in a new chat without re-deriving the system.

The immediate work is to implement and test Dave's existing uGTgtdD concepts in Asana while preserving the workflow semantics that already exist in Google Keep and related reference documents.

Core question:

> If Dave resumes this work in a fresh environment, what does the next ChatGPT session need to know in order to continue without rebuilding the system from memory?

---

## Current System Intent

uGTgtdD is Dave's ADHD-adapted GTD/action-management system.

The practical goal is to reduce:

- working-memory load;
- repeated decisions;
- activation energy;
- decision paralysis;
- open loops;
- the need to scan large lists before acting.

Two useful design phrases from the work so far:

> Capture the branch. Stay on the trunk.

> Lean-to, not cathedral.

The system must help Dave get to a small set of plausible next actions without requiring him to repeatedly re-evaluate the whole universe of commitments.

---

## Current Tool Roles

### Asana

Asana is the current candidate for the **canonical actionable state**:

- Projects
- Next Actions
- Waiting Fors
- task/project status
- real deadlines where appropriate
- context filtering/tagging or the closest useful Asana-native equivalent

The Asana connector is now successfully connected to ChatGPT and has been tested for read access.

Do not make the system depend on premium-only Asana features. Dave specifically noticed the trial warning that he would lose access to features such as Timeline and Custom Fields. The system should remain functional on the free plan.

### Google Keep

Google Keep remains a strong candidate for:

- low-friction capture;
- scratch intake;
- quick temporary notes.

Existing Keep hashtags are **not implementation requirements** for Asana. They express semantics that should be mapped to whatever Asana-native mechanism is appropriate.

### Google Calendar

Calendar is the hard landscape:

- fixed appointments;
- genuinely time-specific commitments;
- real calendar events.

Do not use task due dates as fake calendar commitments unless there is a reason to do so.

### Google Drive

Drive is durable reference/storage for life/admin/reference documents and supporting material.

### GitHub

GitHub is durable engineering/research/source-controlled material and the home of `gtgtdd-sys`.

### ChatGPT / kamMA

ChatGPT is the **conductor/orchestrator**, not canonical memory.

Useful conductor functions include:

- clarify captured items;
- determine whether an item is a project, next action, waiting-for, reference, etc.;
- identify the next visible physical action;
- help choose among actions based on context, time, energy, location, people, and urgency;
- notice stale/overdue items;
- present a small, context-appropriate shortlist;
- help review and maintain the system.

---

## Current Asana State

The Asana connector works.

The existing sandbox project is:

`D's first project`

It contains three disposable demo tasks:

- `Task 1` — due 2026-09-08
- `Task 2` — due 2026-09-09
- `Task 3` — due 2026-09-10

The tasks contain no useful notes, subtasks, or comments. They are vendor/demo material and should not be treated as real work.

Their only useful lesson is:

> Storing a deadline is not enough. The conductor/review layer must notice stale/overdue work and help decide whether it still matters, should be rescheduled, clarified, or killed.

---

## Pilot Domains

Do **not** bulk-import Dave's full backlog.

Use a small number of real current items from a few domains to prove the workflow.

Good pilot domains discussed so far:

- job applications;
- medical/admin;
- upskilling and portfolio projects;
- science/research, especially RMMFB and NTEC.

The point is not to comprehensively migrate those domains. The point is to test the complete loop on a few real items.

Target loop:

> capture → clarify → project / next action → context → retrieve/triage → act → review

---

# Implementation-Independent Reusable Project-Creation Checklist

This is the canonical procedural checklist derived from Dave's existing Keep template and the `Setting_Up_New_Project_-_3x5` Google Doc.

**Every item below is a checklist item. Do not flatten these into headings or prose in future rewrites.**

The checklist describes what should happen when a project is created or clarified. It is intentionally implementation-independent. Asana, Keep, or another tool may implement each item differently.

- [ ] **Give the project a recognizable short name.** Use whatever naming convention is native and useful in the implementation. The old Keep form used `PROJ_<short_name>`; the semantic requirement is a compact recognizable project name, not the literal prefix or hashtag syntax.

- [ ] **Add a short project description if useful.** This is optional; add it when the title alone does not make the project sufficiently clear.

- [ ] **Identify and record the next visible, physical action needed to move the project forward.** The old Keep template represented this with `_next_action`; preserve the concept, not the hashtag.

- [ ] **Write at least a first-pass "what done looks like" blurb.** State the outcome/completion condition well enough that Future Dave can tell when the project is actually finished.

- [ ] **Consider foundational contexts.** Examples from the established system include calendar/time commitment, pseudo-deadline, assigned-to-me, waiting-for, errands, at-home, inbox/unclear state, and needs-pseudo-deadlines.

- [ ] **Consider unique-to-Dave contexts.** Examples include do-not-get-stuck, be-on-the-lookout, chip-away-little-by-little, more-info-on-paper, family-council, goals-and-tracking, tickler/reminder-like items, and description-needs-work.

- [ ] **Assign or consider general priority.** Existing semantic scale: priority 1–4. This is dynamic and represents general importance, not necessarily immediacy.

- [ ] **Assign or consider urgency/time-sensitivity.** Existing material contains an urgency scale of roughly 1–4/1–5 across versions. Preserve the concept; choose the exact scale deliberately during implementation rather than silently changing it.

- [ ] **Add relevant technology/tool/environment contexts.** Examples include network availability, phone, any computer, home laptop, work laptop, home desktop, and physical/snail-mail capability.

- [ ] **Add relevant location/activity contexts.** Examples include home, errands, church/building, FamilySearch Library, work site, or other named places.

- [ ] **Add relevant people/organization contexts.** Include a person, group, organization, meeting itinerary, doctor/provider, family member, friend, coworker, church organization, company, or other entity when being with/connected to that entity is required or especially useful.

- [ ] **Add an energy-available context when useful.** Existing vocabulary ranges from "at least alive" through rough numeric energy levels and "up to 11." The semantic question is: what level of energy is required to make this action realistically available?

- [ ] **Add a time-available context when useful.** Existing vocabulary includes seconds, approximately 5/15/30/45/60 minutes, about 2 hours, and "so long action needs splitting." The semantic question is: what time window makes this action realistically available?

- [ ] **Handle information-input/output/reference classification.** Decide whether the item involves reading/reviewing, reading/implementing, GTD reading/implementation, entertainment intake, a surf/list item, learning while surfing, moving material to General Reference, creating reference material, keeping quick reference, contact information, or another information-handling state. Move true reference material out of the action system when appropriate.

- [ ] **Apply a color/status treatment if useful and supported natively.** Historical project-setup guidance used green/sage for standard tasks, blue/storm for items tied to certain people, and maroon/blossom for errands/honey-dos. Preserve this as optional historical semantics; do not force a color system if Asana's free/native mechanisms make it unhelpful.

**Process note from the original project-setup card:**

> Try to finish the project name/description, next action, and "what done looks like" during the first move from inbox/capture into a project.

---

# Authoritative Context Vocabulary to Carry Forward

This section integrates the Google Doc `Context_List_3x5` with the later Keep template language.

The old syntax used Keep-style hashtags and prefixes such as `#CONTEXT@`, `#CONTEXT~`, and `_...`. Those punctuation conventions are **not** requirements for Asana.

The **concepts and vocabulary are the important part**.

Do not replace the context list with a newly invented simplified taxonomy. We may prune, rename, merge, or map contexts later, but that should be an explicit design decision after testing, not an accidental consequence of migration.

## Foundational

Historical vocabulary:

- assigned_to_me
- calendar / idea_calendar
- waiting_for
- pseudo_deadline / idea_pseudo_deadline
- errands / idea_errands
- at_home / home
- inbox
- needs_pseudo_deadlines

Interpretation:

These are basic action-state or availability contexts that may apply across many projects.

## Priority

Historical scale:

- priority 1–4

Interpretation:

General importance. Dynamic. Do not confuse priority with urgency.

## Urgency

Historical versions show:

- urgency 1–4
- urgency 1–5

This discrepancy should remain visible until Dave deliberately chooses one scale.

Interpretation:

Time sensitivity/immediacy, not overall importance.

## Tech / Objects / Environments

Historical vocabulary:

- any_network
- phone
- any_computer
- lappy_home
- lappy_work
- compy_home
- snail_mail

Interpretation:

The technology or physical tool/environment required to perform the action.

These should evolve to current devices/environments rather than being treated as frozen historical names.

## Information Input / Output

Historical vocabulary includes:

- read_and_review
- read_and_implement
- GTD_read_and_implement
- read_watch_listen_for_fun
- surf_list
- surf_list_but_learning
- move_to_General_Reference
- make_for_General_Reference

Later Keep material also references quick-reference/information categories such as:

- REFERENCE_Move_to_GDrive
- REFERENCE_Quick_and_Available
- contact_info
- mental_health
- potentially_useless_leftovers

Interpretation:

These describe the information-handling mode of the item, not necessarily a physical context. Some should cause material to leave the actionable system and enter durable reference storage.

## Unique-to-Dave

Historical vocabulary includes:

- do_not_get_stuck
- family_council
- goals_and_tracking
- to_pray_for
- be_on_the_lookout
- chip_away_little_by_little
- mental_health
- tickler_file
- description_needs_work
- done_from_Jessi_thanks
- Jessi_Pseudo_Deadline
- craigs_furnace_etc
- more_info_on_paper

Some of these are likely obsolete, person-specific, historical, or better represented by another mechanism. **Do not silently delete them.** Review explicitly when implementing.

## Time Available

Historical vocabulary:

- on_the_order_of_seconds
- at_least_05_minutes
- at_least_15_minutes
- at_least_30_minutes
- at_least_45_minutes
- at_least_60_minutes
- about_2_hours
- so_long_action_needs_splitting

Interpretation:

A filter for whether an action is realistically available in the present time window.

## Energy Available

Historical vocabulary:

- at_least_alive
- at_least_1 through at_least_9
- up_to_11

Interpretation:

A filter for whether an action is realistically available at the present energy level.

The exact scale may be simplified later, but preserve the concept and historical vocabulary for now.

## People

Historical/general vocabulary includes:

- Doctors
- therapist/provider-specific entries
- Various_Family
- Friends
- Work_Acquaintances
- Itineraries / People_with_Meetings
- Amazon
- named-person placeholders

Historical family-specific patterns include:

- Anastasia
  - with_Anastasia
  - connected_to_Anastasia
  - with_Anastasia_physically
- Julie
  - with_Julie
  - connected_to_Julie
  - with_Julie_physically
- Russian_parents
  - with_Russian_parents
  - connected_to_Russian_parents
  - at_house_of_Russian_parents
  - with_Russian_parents_physically
- American_Parents
  - with_American_Parents
  - connected_to_American_parents
  - at_house_of_American_parents
  - with_American_Parents_physically

Interpretation:

Dave has historically distinguished between:

- being physically with someone;
- merely being connected/able to contact them;
- being at a person's house/location.

That distinction can be useful and should not be collapsed automatically.

## Places

Historical examples include:

- home
- Church building
- FamilySearch Library
- work site
- other/named places

The specific historical work-site label in the old card is obsolete as a current location. Preserve the category logic rather than blindly reusing obsolete place names.

## Organizations

Historical examples include:

- Kindex
- Amazon
- Church-related organizations/units
- named-organization placeholders

Interpretation:

Use an organization context when an action is available only through, with, or in relation to that organization.

---

# Reusable Checklists as a First-Class Concept

A major current design requirement is **reusable checklists**.

The missing primitive Dave keeps encountering is:

> Template checklist → instantiate a working copy → complete items → archive/reset without damaging the template.

Examples may include:

- project creation;
- morning routine;
- application submission;
- medical/admin procedure;
- paper/research preflight;
- other recurring procedures.

A reusable checklist is not necessarily itself a project.

It is a repeatable procedure that may be instantiated inside or alongside a project.

Do not force reusable procedures into ordinary project/task structure if doing so destroys the reusable-template semantics.

Dave may write his own helper tooling if existing software does not support the workflow adequately.

---

# Implementation Principles for Asana

## Preserve semantics; change syntax

Keep used hashtags because Keep needed hashtags.

Asana should use whatever native mechanisms are most appropriate.

Potential Asana mechanisms include:

- project names;
- task names;
- task descriptions;
- tags;
- sections;
- assignees;
- due dates;
- subtasks;
- native status/completion state;
- search/filtering.

Do not add hash characters simply to imitate Keep.

## Avoid premium dependency

Do not design the core system around:

- Custom Fields;
- Timeline;
- other trial/premium-only features.

If a premium feature is convenient, the system should still have a functioning free-plan representation.

## Contexts should filter availability

Contexts are not merely metadata decoration.

Their main purpose is to answer:

> What can I realistically do now, given my location, people access, tools, time, energy, and current constraints?

## Real deadlines versus pseudo-deadlines

A real external deadline should be represented clearly.

Pseudo-deadlines are a distinct concept used to create useful temporal structure without pretending an external deadline exists.

Do not silently turn every desired completion date into a hard deadline.

## Next actions must be physical/visible

Avoid vague actions such as:

- "work on resume";
- "deal with paper";
- "figure out doctor stuff."

Prefer a next visible action such as:

- open the resume and rewrite the first experience bullet;
- email the provider asking for the missing form;
- read the methods section and annotate the first unresolved claim.

---

# What Was Useful in the Older 3×5 Documents

From `Setting_Up_New_Project_-_3x5`:

- short recognizable project title;
- optional short description;
- explicit next visible physical action;
- explicit "DoneLooksLike";
- strong instruction to establish these when clearing/moving out of inbox;
- context categories rather than one undifferentiated tag pile;
- optional color semantics.

From `Context_List_3x5`:

- separating foundational, tech, information, unique-to-Dave, time, energy, people, places, and organizations;
- distinguishing priority from urgency;
- distinguishing contact with a person from physically being with them;
- treating available time and energy as actual action-selection contexts;
- retaining "action needs splitting" as a useful state, not just another duration;
- explicitly recognizing information-handling states such as review, implementation, learning, and reference transfer.

These are useful semantics to preserve even if the exact historical tag names are modernized.

---

# Open Design Questions for the Next Chat

Do not answer all of these abstractly before testing. They are prompts for small implementation experiments.

1. What Asana-native mechanism should represent **contexts** on the free plan?
   - Tags?
   - Sections?
   - Task-name conventions?
   - Some hybrid?

2. How should **project outcome / DoneLooksLike** be represented?
   - Project description?
   - A dedicated task?
   - Another native field?

3. Where should the **current Next Action** live?
   - Ordinary task in the project?
   - A dedicated section?
   - Convention plus tag?

4. How should reusable checklists be instantiated without damaging the template?

5. Which historical contexts are still useful, obsolete, redundant, or better represented by a native feature?

6. What is the minimum viable context vocabulary that preserves the power of the old system without recreating a giant tag-management project?

7. How should real deadlines and pseudo-deadlines be represented distinctly?

---

# Immediate Next Steps

1. **Do not redesign the entire system.**

2. Inspect Asana's currently available free/native structures only as much as necessary.

3. Decide how to represent the **project-creation checklist** as a reusable checklist/template workflow.

4. Decide on a first-pass native representation for the existing **context list**, preserving its semantics.

5. Pick a **very small number of real current items** across perhaps two to four domains:
   - job applications;
   - medical/admin;
   - upskilling/portfolio;
   - RMMFB/NTEC or other research.

6. Run each through the full flow:
   - capture;
   - clarify;
   - determine project/outcome if needed;
   - identify next visible action;
   - attach useful contexts;
   - retrieve based on a real current situation;
   - act/review.

7. After the first real test, adjust the structure based on actual friction rather than theoretical elegance.

---

## Continuation Rule

The new chat should treat this file as authoritative current context, while recognizing that the project is deliberately still in an experimental implementation phase.

The next chat should **continue**, not restart.

