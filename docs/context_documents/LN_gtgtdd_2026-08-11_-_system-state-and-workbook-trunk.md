*BEGIN: Context Document Header*

# CONTEXT DOCUMENT — Continuation

## Project

**Name:**
uGTgtdD / gtgtdd-sys

**Description:**
A deliberately minimal personal implementation of David Allen's _Getting
Things Done_ (GTD), adapted to Dave's ADHD and executive-function needs. The
system is intended to reduce repeated decisions and working-memory burden so
that more attention goes toward doing the things Dave has already decided
matter.

---

## Continuation Metadata

**Prepared at:**
1786462200_2026-08-11T11:30:00-0400

Generated via:

```bash
date +'%s_%Y-%m-%dT%H:%M:%S%z'
```

(Boston, MA time)

**Continued from chat:**
Current ChatGPT conversation; exact UI chat title was not available to the
assistant when this document was prepared.

**Also involving:**
- GTD Workbook implementation
- Google Keep, Asana, and Google Drive roles
- therapy discussion with Gerry about priority, urgency, and salience
- MLU Math final / LatentForge recommender idea as a captured branch

---

## Author / Source

**User (GitHub):**
@bballdave025

**User (ChatGPT):**
Dave / D. Black

---

## Intent for This Context

Enable a fresh conversation or later work session to continue uGTgtdD without
re-deriving its philosophy, current decisions, or immediate next steps. This
is a checkpoint file for thinking, not polished documentation and not a
comprehensive set of GTD notes.

---

## Usage Instructions

- Treat this document as **authoritative project state**.
- Continue with **minimal re-derivation**.
- Reinterpret only when explicitly requested.
- Prefer doing GTD actions over producing comprehensive notes about GTD.
- Apply: **Capture the branch. Stay on the trunk.**
- Apply: **Lean-to, not cathedral.**

*ENDOF: Context Document Header*

# Current State

uGTgtdD is intended to be a practical GTD implementation rather than a
productivity-system hobby.

The system's purpose is to make it easier for Dave to do what he has already
decided matters while reducing:

- working-memory load,
- repeated prioritization,
- activation cost,
- and the number of possibilities that must be considered at once.

Two governing metaphors are active:

> **Capture the branch. Stay on the trunk.**

When a valuable new idea appears during focused work, preserve enough of it
in an appropriate durable place that it will not be lost, then return to the
current objective. The branch is captured, not followed.

> **Lean-to, not cathedral.**

The system should be sufficient to support action. It does not need to become
an elaborate intellectual object in its own right.

A therapy discussion with Gerry on 2026-08-11 provided useful confirmation
about the direction of the system. Gerry also endorsed the GTD Workbook as a
good way to work through GTD in practice.

The important distinction established afterward is:

> **The workbook contains the procedure. The GTD system contains the
> product.**

Dave does not need a second, comprehensive version of the workbook. The goal
is to do the workbook's actions and preserve the results of those actions.

# Current Tool / Information Architecture

The current broad flow is:

**Capture**
→ get the thing safely out of working memory

**Clarify**
→ determine what it is and whether it is actionable

**Projects / Next Actions**
→ actionable material belongs in the GTD/task system

**General Reference**
→ durable non-actionable information belongs in Google Drive

Current likely tool roles:

- **Asana** — primary candidate for projects, next actions, waiting-fors, and
  other actionable GTD material.
- **Google Keep** — quick temporary capture, partial prompts, links, and notes.
  Old Keep syntax should not be preserved merely because it once existed.
- **Google Drive / `__General_Reference`** — durable General Reference.
- **`__General_Reference/_INBOX_SCANS`** — incoming source material that still
  needs processing, not a permanent home for processed project-state
  documents.

The implementation should preserve useful behaviors from the old system
without mechanically reproducing historical punctuation, tags, or hacks.

# GTD Contexts

"Context" is used primarily in David Allen's GTD sense: a place, state,
person, object, or circumstance necessary for, or especially conducive to, a
next action.

The useful operational question is:

> **Given the circumstances I am in right now, what work is actually
> available to me?**

Old Google Keep notation included forms such as:

```text
#CONTEXT@obj_phone
#CONTEXT@obj_any_computer
#CONTEXT@ppl_Anastasia
#CONTEXT@plc_home
```

The literal syntax is not important.

Old context families included:

- `obj` — required object/tool/device
- `plc` — place
- `ppl` — person or people
- `org` — organization/group
- `info` — information-related mode/activity
- `idea` — special opportunity/idea contexts
- `phelp` — old category whose intended meaning is currently uncertain

People contexts remain especially promising. Before calling, seeing, or
visiting somebody, Dave should be able to see what has accumulated to ask,
give, discuss, remember, or do while that opportunity exists.

Examples of device/place contexts that have real consequences include:

- any phone,
- any computer,
- work laptop,
- home tower,
- home,
- parents' house.

NTEC and RMMFB are examples of work that may become especially actionable at
the home tower because relevant hardware, data, and attached storage are
there.

# Time and Energy as ADHD-Relevant Filters

The old system used a separate `#CONTEXT~...` notation for dimensions such as
time and energy. The notation itself does not need to survive.

## Time

Useful time buckets previously included approximately:

- seconds,
- at least 5 minutes,
- at least 15 minutes,
- at least 30 minutes,
- at least 45 minutes,
- at least 60 minutes,
- about 2 hours,
- and "so long that the action probably needs to be split."

The key question is:

> **I have 15 minutes. What useful things actually fit into 15 minutes?**

A useful category is:

> **chip away little by little**

This is for work that advances during otherwise awkward fragments of time
without becoming the day's main project.

Examples already discussed include:

- Google Drive archaeology during a short bus ride,
- gradually identifying and annotating digitized family photographs.

## Energy

The old energy scale ran roughly from:

- barely alive,
- 1 through 9,
- up to eleven.

The exact psychometrics do not matter.

The useful question is:

> **Given the energy I actually have, what can I successfully do?**

Examples:

- eating breakfast can happen at "barely alive";
- scanning incoming paper/mail should be low-energy work;
- difficult RMMFB implementation or serious research writing may require
  high energy.

The desired behavior is to select meaningful work that fits current capacity
rather than selecting a theoretically important task whose cognitive demands
make successful initiation unlikely.

Time and energy are promising filters, but they have not yet been implemented
consistently enough to claim that they are already proven useful in practice.

# Priority, Urgency, and Salience

This remains the largest conceptual and therapeutic question.

The old system had:

- priority levels 1–4,
- urgency levels 1–5.

There is no current reason to preserve those exact scales.

The unresolved problem is not defining the words "priority" and "urgency."
It is making operational judgments in real life.

Important distinctions include:

> **Important**
>
> versus
>
> **feels important right now**

and

> **Urgent**
>
> versus
>
> **my brain is treating this as urgent**

Questions to continue working on with Gerry and through actual system use:

1. How important is this?
2. How urgent is this?
3. What evidence supports those judgments?
4. Is emotional/salience information useful here?
5. Is salience distorting the decision?
6. What should happen next because of the answer?

Desired external rules should reduce decision burden without becoming rigid.
An important goal is to protect genuinely important, non-urgent work from
being continually displaced by whatever generates the strongest immediate
signal.

# Minimal Project Creation

Current preferred first-pass project creation is deliberately small:

1. Create a project title.
2. Put it on the project list.
3. Add a short description if needed.
4. Identify the next action.
5. Give a first-pass description of what "done" looks like.
6. Add useful contexts.
7. Add color/collaborators only if relevant.

The "done looks like" description may be imperfect and explicitly marked as
needing refinement.

Governing rule:

> **Define it well enough to move. Improve the definition later if
> necessary.**

Project creation must not become a large metadata form with its own activation
cost.

# GTD Workbook Working Rule

The workbook should be used as the source of steps and exercises.

The collaboration pattern with ChatGPT should normally be:

1. Dave opens or reads the next small workbook section/exercise.
2. Dave may provide a screenshot, a short excerpt, or his own description of
   the exercise.
3. ChatGPT should default to helping **perform the exercise**, not summarizing
   the workbook page.
4. Preserve the outputs of the actions:
   - captures,
   - clarified next actions,
   - projects,
   - contexts,
   - waiting-fors,
   - decisions,
   - and perhaps a tiny progress bookmark when useful.
5. Do not build a shadow workbook or comprehensive set of notes about the
   workbook itself.

If OCD/completion pressure creates an urge to make comprehensive notes,
distinguish between:

- capture needed to support action or continuation, and
- duplicated reference material that already exists in the workbook.

The trunk is:

> **Complete the workbook by doing the actions.**

Not:

> Construct a comprehensive representation of having read the workbook.

# General Reference / Scan-Inbox Decision

`GDrive > __General_Reference > _INBOX_SCANS` is for incoming material that
still needs processing.

Appropriate examples include:

- scans or photos of paper/mail,
- screenshots or exports of old GTD / Google Keep material not yet clarified,
- other temporary source material captured for later processing,
- the 2026-08-11 therapy-prep PDF, if retained as source/reference.

Processed uGTgtdD decisions and living context/project-state documents should
not permanently live in `_INBOX_SCANS` merely because they are documents.

# Success Criteria

The system should make questions like these easier to answer:

> I have 15 minutes on this bus. What could I advance?

> I'm exhausted. What worthwhile thing can I still do?

> I unexpectedly have two hours and good cognitive energy. What important
> work should get that scarce resource?

> I'm about to talk with Anastasia. What have I been waiting to discuss with
> her?

> I'm going to my parents' house. Is there anything I can only/easily do
> there?

> I'm at the home tower with the big drive connected and I have high energy.
> Which research next action becomes available?

> This feels incredibly urgent. **Is it?**

> This is genuinely important but has no deadline. How do I keep it from
> disappearing for six months?

Success is not perfect organization or perfect metadata.

Success is more time spent doing what matters, with less repeated cognitive
effort deciding what to do.

# Captured Branch — MLU Math Recommender × LatentForge

**Out of Scope / Not Yet Part of This Repository**

Dave wants to connect the end of the MLU Math final project
(matrix-factorization book recommender) with synthetic reviewer/book data from
LatentForge.

The material Dave shared establishes that the MLU final contest metric is
straight **Mean Squared Error (MSE)** on a hidden holdout set of 1–5 ratings.
The provided notebook uses a local train/validation split and permits repeated
leaderboard submissions. It suggests controlled experiments involving such
things as latent-feature count, learning rate, epochs, initialization, early
stopping, scaling, data split choices, regularization, prediction clamping,
and an SVD-like extension.

For 2026-08-11, the contest closes at 23:59:59 UTC, i.e. 19:59:59 EDT.

Current branch decision:

- first objective is a valid submission before the deadline;
- preserve the baseline score;
- controlled improvements may follow if time remains;
- do not make `MSE ≈ 0.38` a magical career threshold;
- re-enrollment is worth considering only if it enables a bounded
  learning/portfolio experiment rather than endless decimal polishing.

A later useful experiment may be:

1. preserve/reproduce the course baseline,
2. make a small number of principled improvements,
3. apply the matrix-factorization structure to LatentForge's synthetic
   reviewer/book data,
4. investigate how known latent structure affects recovery and generalization.

This branch is worth preserving but should not expand the active uGTgtdD
scope.

# Active Questions

- What is the smallest workable Asana implementation?
- Which old contexts are still useful enough to recreate?
- What is the minimum useful representation for time?
- What is the minimum useful representation for energy?
- How should importance and urgency be operationalized without false
  precision?
- What external rules can protect important, non-urgent work without becoming
  rigid?
- Should `phelp` be recovered at all, or allowed to disappear unless a use
  case reappears?
- Where should living uGTgtdD context/decision documents permanently live in
  Google Drive?

# Immediate Next Steps

When uGTgtdD work resumes:

1. Open the GTD Workbook at the current/next exercise.
2. Do the exercise rather than summarize it.
3. Capture only the outputs and decisions needed by the system.
4. Refine the minimum viable Asana/tool structure only when a workbook
   exercise or real use case requires it.
5. Test context/time/energy filters in actual life before adding more
   taxonomy.

For the next system-design decision, prefer a real example from current life
over an abstract taxonomy discussion.

# Continuation Guardrails

- Search for existing implementations/features before building new machinery.
- Preserve useful behaviors, not historical punctuation.
- No comprehensive GTD rewrite.
- No comprehensive workbook notes.
- No metadata field unless it earns its keep in actual use.
- A useful captured idea does not become the current project merely because it
  is interesting.
- **Capture the branch. Stay on the trunk.**
- **Lean-to, not cathedral.**

---

---

---

# Making sure all gathered things are here

Yes. The things I was still holding onto as gathered/captured material, rather than considering them disposed of, were:

GTD Workbook — actually work through it, doing the actions rather than producing comprehensive notes about it.

Asana minimum viable implementation — figure out the smallest workable structure when actual use/workbook exercises require it.

Old Google Keep GTD material — mine it for useful behaviors and structures, not necessarily its old syntax.

Old contexts — determine which are still worth carrying forward, including object/device, place, people, organization, information/mode, and possibly idea.

phelp — we don't remember what it meant; recover it only if that becomes worthwhile rather than doing archaeology merely to satisfy completeness.

People-context material — especially things accumulated to ask/give/discuss/do with Anastasia, parents, etc.

Time-required contexts — seconds, 5m, 15m, 30m, 45m, 60m, ~2h, and “this needs splitting”; exact buckets still negotiable.

Energy-required contexts — the old “barely alive” through “up to eleven” idea; exact scale still negotiable.

Priority — needs an operational meaning, rather than blindly restoring old Priority 1–4.

Urgency — same; don't blindly restore Urgency 1–5.

Importance vs. felt importance and urgency vs. felt urgency — specifically something to keep developing with Gerry and through actual use.

Protection for important/non-urgent work — something the eventual system needs to accomplish.

chip away little by little — preserve this useful category/concept for work that fits small scraps of time.

Google Drive archaeology — example of chip-away work.

Family-photo identification/annotation/history project — another chip-away candidate.

Scanning incoming paper/mail — low-energy work and part of getting paper into the digital/reference system.

_INBOX_SCANS processing — incoming scans/source material goes there; it isn't supposed to become permanent storage merely because something arrived there.

General Reference organization — processed durable reference belongs under __General_Reference; exact permanent home for living uGTgtdD context/decision documents was still an open question.

Minimal project-creation procedure — title → project list → description if needed → next action → provisional “done” → useful contexts → optional color/collaborators.

NTEC/RMMFB home-tower context — some actions become available there because of the classifier, 14 TB drive, image collection/storage, etc.

MLU recommender × LatentForge — explicitly captured as a branch, not uGTgtdD work: submit the MLU recommender today, preserve baseline MSE, then potentially do bounded controlled improvements and later use the matrix-factorization structure with LatentForge's synthetic book/reviewer data.

The ~0.38 MSE idea — worth investigating as an experimental target, but not to be promoted into a magical career threshold or justification for endless optimization.

Re-enrollment — possible if it buys a bounded learning/portfolio experiment; not simply to polish the leaderboard decimal.


And there are a few things I was deliberately not holding as obligations: reproducing all the old Keep notation, recovering every historical category, making comprehensive GTD notes, making comprehensive Workbook notes, or deciding the complete Asana architecture before we actually need it.

Most importantly, I think the Context Document you just committed is now the durable handoff for essentially this whole bundle. Its Active Questions explicitly preserves the Asana/context/time/energy/priority/phelp/Drive loose ends.

So I don't need to keep a parallel secret armful of these things anymore. They've been gathered into the basket. That 075fcb6 commit is a rather satisfying point at which we can stop relying on conversational working memory for them.
