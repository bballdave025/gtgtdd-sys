# Context Documents

This directory contains **continuation-ready context documents** for the  
*gtgtdd-sys* project.

These are not polished documentation. They are:

- structured snapshots of design state
- handoff-ready summaries for continuing work in a new session
- “lab notebook” entries for architecture decisions and progress

---

## Purpose

Each document is designed to answer:

> “If I had to resume this work in a fresh environment, what would I need to know?”

They preserve:

- current architecture
- naming decisions
- design constraints
- next-step execution plans
- important non-obvious insights

---

## Format

All context documents follow a consistent header:

- project name + description
- timestamp (machine + human readable)
- originating chat/session
- author attribution

This allows:

- chronological tracking
- reproducibility of thinking
- easy copy/paste into new AI sessions

Specifically: 

```text
CONTEXT DOCUMENT for continuation of the "[**INSERT-PROJECT-NAME-AND-1-TO-3-SENTENCE-DESCRIPTION**]" project

DOCUMENT PREPARED FOR CONTINUATION: 

[**TIMESTAMP NOT IN CODE BLOCKS BUT CONTAINING THE INFO AS IF RETURNED FROM THE FOLLOWING BASH COMMAND**]

date +'%s_%Y-%m-%dT%H:%M:%S%z'  # use current Boston, MA time zone

CONTINUED FROM CHAT ENTITLED:
[**INSERT-CHAT-TITLE**]
ALSO INVOLVING
`([**INSERT-OTHER-CHAT-SUBJECTS**]|no other subjects specified)`

FROM USER 
  (ChatGPT) usually-omit
  (GitHub) @bballdave025
```

---

## Naming Convention

```text
LN_{short-project-marker}_YYYY-MM-DD_{very-optional-tag}_-_{short-slug}.md
```

Example: the first one I'm doing (the one for the first trip where I set this up) here will be named 

```text
LN_gtgtdd_2025-05-16_ctx01_-_trajectories_career_resumes_etc.md
```

(`LN` is for Lab Notebook, my name for these files since undergrad, even when working in industry.)

(`gtgtdd` is for uGTgtdD system.)

Something like `ctx01` for the optional tag is probably a good idea to use if I'm almost certain that I will be doing at least one more of these context (`ctx`) documents for this repo, today.

Other tags could be `submitted-addenda`, `pr-for-k-prisbrey`, or `parked`, but it's almost always better left blank.

---

## Retrieval Tip

If unsure where to resume:

1. Sort by filename (date)
2. Open the most recent `LN_*` file
3. Follow its "Immediate Next Steps" or similar section

---
