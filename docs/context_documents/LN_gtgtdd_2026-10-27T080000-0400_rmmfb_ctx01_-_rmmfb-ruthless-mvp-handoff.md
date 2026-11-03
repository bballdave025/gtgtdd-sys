*BEGIN: Context Document Header*

# CONTEXT DOCUMENT — Continuation

## Project

**Name:**  
RMMFB / Reused Manuscript Fragments in Bindings

**Description:**  
Research and engineering work for identifying, classifying, and retrieving
reused manuscript material in historical book bindings, including dataset
preparation, computer-vision experiments, explainability, provenance,
historical experiment reconstruction, AWS / SageMaker execution, and
preparation of a minimum-publishable paper for *Fragmentology*.

---

## Continuation Metadata

**Snapshot-family timestamp:**  
2026-10-27T080000-0400

This file is part of the coordinated Boston→Bountiful boundary snapshot. The
shared timestamp is a snapshot-family identifier, not a claim that this file
was physically authored at exactly 08:00.

**Continued from chat:**  
`RMMFB_ruthless_MVP_after_JD_thru2026-10-27T080000-0400`

**Primary source remoulded for this snapshot:**  
`LN_rmmfb_2026-10-17_ctx-try-02_-_keith-reconstruction-and-staged-transfer-addendum.md`

**Repository version of the October 17 addendum, preserved at the historical
commit where it was added:**  
`docs/context_documents/LN_rmmfb_2026-10-17_-_keith-reconstruction-and-staged-transfer-addendum.md`

**Also involving:**

- Eightfold Way execution
- historical Keith Prisbrey experiment reconstruction
- recovered 622-image historical dataset
- prospective 709 / 1000 / 1000 difficulty staging
- provenance-aware train/validation/test grouping
- canonical 3,331-image dataset
- filename/source-family archaeology
- e-codices provenance conventions
- closed ePaveldas sanity check
- ontology and historical filename tokens
- ResNet-50 / 224 baseline
- Guided Grad-CAM / guided backpropagation
- AWS / SageMaker smoke test
- wild-corpus retrieval
- ruthless scope control

---

## Author / Source

**User (GitHub):**  
@bballdave025

**User (ChatGPT):**  
KaMMA / ChatGPT

---

## Intent for This Context

Resume RMMFB without reconstructing decisions that have already been made.

This is the **system-level RMMFB handoff for `gtgtdd-sys`**, not a replacement
for all project-specific technical documentation in `fhtw-paper-code-prep`.
Its purpose is to let a fresh chat understand what RMMFB is, what is already
settled, what exact artifacts and identifiers matter, what the current
experimental trunk is, and what should happen next.

The project has moved beyond broad planning and provenance archaeology into
execution of the agreed Eightfold Way.

The immediate scientific goals remain:

1. finish the group-aware split contract for the canonical 3,331-image corpus;
2. preserve and characterize the recovered 622-image historical Keith dataset;
3. use the deliberately simple prospective progression

```text
622
1331 = 622 + 709
2331 = 1331 + 1000
3331 = 2331 + 1000
```

without pretending the later stages reconstruct historical collection order;
4. run the first real RMMFB model experiments rather than doing more runway
   work.

---

## Usage Instructions

- Treat this document as **authoritative snapshot state** unless newer explicit
  evidence supersedes it.
- Continue with **minimal re-derivation**.
- Reinterpret only when explicitly requested.
- Distinguish clearly among:
  - completed work;
  - current paper work;
  - optional pickups;
  - future/deferred work.
- Do **not** replace the existing Eightfold Way with a newly invented plan.
- Do **not** reopen completed filename/provenance archaeology without a concrete
  scientific blocker.
- Do **not** silently rename or normalize historical filenames.
- Do **not** turn every interesting branch into a requirement.
- Preserve historical mistakes/oddities when they document how the dataset was
  really created.
- Give exact shell commands in small executable batches during interactive
  work.
- Preserve exact URLs, file IDs, repository paths, branch names, and filenames.
  Do not paraphrase them away.
- When a source artifact contains an unresolved historical detail, preserve it
  as unresolved rather than replacing it with recollection.

### Ruthless sprint rule

If a proposed search, analysis, recovery operation, or other step is likely to
take more than approximately **3 minutes**, stop first and discuss its expected
scientific utility with Dave.

Do not casually enter:

```text
15-minute research holes
100-minute archaeology holes
large backup hunts
large historical-data reconstruction projects
```

The default is execution.

Governing scope rules:

> **Capture the branch. Stay on the trunk.**

> **Stop improving the runway. Take off.**

> **Paper first. Evidence second. Portfolio for free. Cool new research only
> if it hitchhikes.**

And now:

> **The gun has gone off. Run the experiment.**

*ENDOF: Context Document Header*

# 1. Role of This Chat

This chat is the **RMMFB ruthless-MVP conductor** for the current publication
push.

Its job is to move the already-developed RMMFB research into a defensible,
minimum-publishable experimental result without restarting years of dataset,
ontology, provenance, architecture, or infrastructure design.

The chat owns, or must preserve:

- the current paper-level experimental contract;
- the distinction between historical reconstruction and current experimental
  design;
- the Eightfold Way;
- group-aware split and test-vault semantics;
- current low-resolution ResNet-50 baseline/fine-tuning choices;
- the bounded attribution plan;
- AWS/SageMaker execution logic;
- the boundary between useful provenance work and archaeology;
- the current sequence from split → smoke test → 622 → 1331 → 2331 → possible
  3331 → fine-tuning → attribution → richer-label experiment → wild retrieval.

The paper objective is not to build the globally optimal RMMFB system.

It is to turn the large amount of existing scientific work into a defensible,
publishable experiment.

The sunk foundation already includes:

- years of image discovery;
- manually curated positives and negatives;
- custom binding-reuse ontology;
- provenance-preserving naming;
- fake-outs and counterexamples;
- heterogeneous repositories;
- source reconstruction work;
- historical model experiments;
- preprocessing infrastructure;
- explainability infrastructure;
- a large wild corpus.

That foundation now needs to produce results.

The paper should contain a strong scientific spine without expanding into a
general-purpose manuscript-fragment AI platform.

# 2. Authority and Boundaries

## 2.1 This chat owns RMMFB experiment semantics

This chat is authoritative for the **current RMMFB MVP scientific plan**:

- what counts as historical evidence;
- what is current prospective design;
- what is frozen versus still unresolved;
- what must happen before model results are viewed;
- what constitutes test leakage;
- which experiment branches are mandatory, optional, or parked;
- how far Keith reconstruction should go;
- what the wild-corpus stage can legitimately claim.

## 2.2 uGTgtdD owns cross-project action orchestration

The sibling uGTgtdD/system-conductor context should own:

- whether RMMFB is active versus parked in the whole-life system;
- Asana scheduling/activation;
- cross-project priority;
- the leaving-Boston snapshot map;
- whether a stale task date should be moved or cleared.

Expected sibling file:

[`LN_gtgtdd_2026-10-27T080000-0400_ugtgtdd_ctx01_-_system-conductor-handoff.md`](./LN_gtgtdd_2026-10-27T080000-0400_ugtgtdd_ctx01_-_system-conductor-handoff.md)

Do not ask the RMMFB chat to reprioritize Dave's entire life.

## 2.3 The project repository remains the technical home

Primary repository:

```text
bballdave025/fhtw-paper-code-prep
```

Repository URL:

https://github.com/bballdave025/fhtw-paper-code-prep

Primary branch:

```text
main
```

The system-level `gtgtdd-sys` file is a continuation/handoff layer. The
project's durable code, experiments, dev notes, and project-specific context
documents belong in `fhtw-paper-code-prep`.

## 2.4 Supporting repositories have bounded roles

### Classification / ontology support

Repository:

```text
bballdave025/congenial-chainsaw-rmfb-html
```

Repository URL:

https://github.com/bballdave025/congenial-chainsaw-rmfb-html

Relevant current file:

```text
classifier.param
```

Direct URL:

https://github.com/bballdave025/congenial-chainsaw-rmfb-html/blob/main/classifier.param

This repository supports the classification/ontology history. It is not the
main current experiment runner.

### Earlier project / vision lineage

Repository:

```text
bballdave025/rib-wrist-in-bin-din
```

Repository URL:

https://github.com/bballdave025/rib-wrist-in-bin-din

This repository contains older RMMFB/RMFB project vision and protocol lineage.
It can support historical/contextual reconstruction but should not displace the
current `fhtw-paper-code-prep` execution path.

## 2.5 Boundaries of historical reconstruction

The 622-image Keith cohort is a real historical anchor.

The later 709 / 1000 / 1000 additions are **current experimental staging**.

Do not rewrite prospective stages as historical facts.

Do not require recovery of:

- every historical intermediate dataset;
- every WeTransfer package;
- every old source manifest;
- every failed-drive artifact;
- every historical training detail

before current model execution can begin.

## 2.6 Boundaries of provenance claims

Keep distinct:

### Digital / host provenance

```text
repository
collection
shelfmark
host volume
page / folio / image locator
digital source
download/acquisition convention
```

### Earlier fragment history

```text
where manuscript was written
when manuscript was written
original textual context
discard/reuse history
binding date
movement between institutions
historical geographic origin
```

Filename provenance should not be used to smuggle in historical-origin claims.

# 3. Current State

## 3.1 Current state in one paragraph

The canonical 3,331-image RMMFB dataset has been reconciled exactly, the
ontology is stable enough for publication work, and the filename/provenance
audit is closed. Source-specific exceptions including e-codices, Cambridge,
CodexRestitutus, and ten miscellaneous naming forms have been documented well
enough to derive host-level grouping without rewriting historical filenames.
The final ePaveldas grep returned no matches and that result has been
documented; no further ePaveldas archaeology is needed. A major Way-2
breakthrough also occurred: the actual historical dataset sent to Keith
Prisbrey and associated with the successful early experiment was recovered in
Google Drive. It contains **622 images** and represents the easier/obvious-reuse
historical cohort. Rather than spending time reconstructing every intermediate
historical collection state, the current plan is to retain 622 as the true
historical anchor and create prospective difficulty stages of +709, +1000, and
+1000, reaching 1331, 2331, and 3331 images. The final 1000 may initially be
left untouched. The next work should be executable model work, not another
marathon of archaeology.

## 3.2 Canonical 3,331-image dataset — complete

Canonical local curated tree:

```text
/cygdrive/d/ds/rvc3331
```

Canonical Google Drive inventory:

```text
consistentized_3331_dataset.txt
```

Google Drive file ID:

```text
1c2BVTQ9Fgt81FhpLG806d1r4ge5aJ4ZC
```

Inventory comparison:

```text
Drive canonical list: 3331 unique entries
live curated filesystem: 3331 unique entries
normalized comparison: identical
```

SHA-256:

```text
4d84562384261999c6bbe81a90d0f922e9e2ab57132fef72d7f7e304985110d4
```

Conclusion:

> The 3,331-image inventory is reconciled.

Do not reopen this question absent concrete contradictory evidence.

## 3.3 Historical Keith dataset — recovered

Recovered folder:

```text
https://drive.google.com/drive/folders/1dlm2fumV5O-m0qJYmtRv9dj2BsBWNxU0
```

The recovered historical cohort contains:

```text
622 images
```

This is the successful early/easy cohort associated with the first
well-performing RMMFB experiment.

The source document's historical interpretation is that the first cohort
contains visually obvious reuse.

Keith later joked approximately that the first set worked fine/looked great
until Dave sent the second folder with the "fouled up" material.

"Fouled up" means harder/subtler, not corrupted:

- smaller reused regions;
- less visually dominant reuse;
- harder examples;
- more difficult classification conditions.

A PDF/email artifact relating to the successful WeTransfer delivery is:

```text
Original_doc_names_for_Keith_01_-_First-Yes_No-sent-successfully-to-keithprisbrey68-wetransfer.pdf
```

An old directory tree contains the exact path:

```text
My Drive
>> __General_Reference
>> P
>> P2_2025_RMFB_Portable
>> P2_Dir_Tree_2025-02-05T104100-0700.txt
```

Historical directory structures included names such as:

```text
BigDatasetReuse_<date>
Yes_Reuse
No_Reuse
Not_Reuse
```

The original 14-TB drive containing important historical datasets and a large
wild corpus has failed.

Do not make recovery from that physical drive a prerequisite.

## 3.4 Historical dataset-preparation evidence

Historical preparation material is preserved separately, including:

```text
dataset_preparation_examples.zip
```

Google Drive file ID:

```text
1Eo6j4JhOdnFQc73kUstCwJybZrUQcCLC
```

This material can support Methods/history reconstruction when useful.

It is not a reason to pause model execution.

## 3.5 Curated and wild corpora

Curated corpus:

```text
3331 manually classified images
```

Characteristics:

- heterogeneous digital repositories;
- positive binding reuse;
- difficult/subtle reuse;
- deliberate negatives;
- fake-outs;
- provenance-bearing filenames;
- multiple observations from some host objects;
- custom physical-role ontology.

Recovered/deduplicated wild candidate corpus:

```text
~41,790 distinct images
```

The wild corpus is not comprehensively labeled.

Therefore Way 8 is:

```text
retrieval / discovery
```

not ordinary benchmark evaluation.

Historically, an earlier inaccessible 14-TB drive also held roughly 50,000
in-the-wild images. Copies may exist elsewhere, but recovery is not currently
allowed to become a backup-search project.

## 3.6 Ontology state

Current important binding-reuse codes include:

```text
orc  Outside_Cover_Reuse
ucr  Under_Cover_Reuse
spr  Spine_Protection_Reuse
fmr  Front-back_Matter_Reuse
obr  One_Behind_Reuse
cwa  Cover_Wraparound_Reuse
tbr  Tiny_Background_Reuse
scg  Connecting_or_Guard_Reuse
abg  Across_Book_Gutter_Reuse
wpr  Wrapper_Reuse
gni  General_Not_In_Situ_Reuse
```

Additional meta/negative codes include:

```text
mcl  Multiple_Classes
mbr  Multiple_Binding_Reuse_Classes
mmx  Multiple_Mixed_But_All_Not_Binding
fko  Fake_Out
iac  Important_as_Counter_Example
nbr  No_For_Binding_Reuse
oic  No_Binding_Reuse_but_Other_Interesting_Classes
noi  Nothing_Interesting
dnu  Do_Not_Use
```

Historical:

```text
suh  Somewhat_Uneasy_with_Classification_or_Hard
```

is deprecated.

Rules:

- `suh` may remain in historical filenames.
- `suh` is not an active current label.
- `pasteboard` is not an ontology class.
- `wpr` remains a meaningful ontology concept even though no current marked
  examples appear in the frozen 3,331.
- historical filename labels are evidence, not cleanup targets.

Bounded `suh` audit:

```text
28 filenames containing _suh
4 also containing _fko
0 hard contradictions
1 reviewed mbr case
```

The ontology is sufficiently settled.

The supporting `congenial-chainsaw-rmfb-html` repository has explicit October
3, 2026 commits documenting the `suh` deprecation. Do not reopen this merely to
make the ontology prettier.

## 3.7 Filename/provenance audit — closed

Initial parser:

```text
3227 matched
104 unmatched
```

The 104 were accounted for as:

```text
75 e-codices family
19 Cambridge family
10 miscellaneous
----------------
104
```

The parser originally expected a five-digit `_NNNNN` identifier before the
classification suffix.

The audit established that this is not a universal source convention.

Governing rule:

> Historical filenames are provenance artifacts, not strings to beautify.

Therefore:

```text
preserve filenames
adapt parser
derive host-level group_id
move on
```

## 3.8 ePaveldas sanity check — closed

Final explicit search:

```bash
find . -type f -iname '*.jpg' -printf '%P\n' |
grep -Ei 'e.?pav|paveldas'
```

Result:

```text
no matches
```

No additional ePaveldas recovery is required for the current grouping work.

# 4. Canonical Systems and Artifacts

## 4.1 Primary repository and snapshot-boundary Git state

Primary repository:

```text
bballdave025/fhtw-paper-code-prep
```

URL:

https://github.com/bballdave025/fhtw-paper-code-prep

Primary branch:

```text
main
```

Context-document convention:

```text
docs/context_documents/README.md
```

Important earlier context documents:

```text
LN_rmmfb_2026-09-09_-_minimum-publishable-paper-plan.md
LN_rmmfb_2026-09-18_-_mvp-scaffold-closed-and-execution-plan.md
LN_rmmfb_2026-10-10_-_provenance-aware-split-and-mvp-execution-state.md
```

GitHub URLs for those documents:

https://github.com/bballdave025/fhtw-paper-code-prep/blob/main/docs/context_documents/LN_rmmfb_2026-09-09_-_minimum-publishable-paper-plan.md

https://github.com/bballdave025/fhtw-paper-code-prep/blob/main/docs/context_documents/LN_rmmfb_2026-09-18_-_mvp-scaffold-closed-and-execution-plan.md

https://github.com/bballdave025/fhtw-paper-code-prep/blob/main/docs/context_documents/LN_rmmfb_2026-10-10_-_provenance-aware-split-and-mvp-execution-state.md

The October 17 addendum was added in commit:

```text
5496291dc8dad4081d5fc4f6ba33112ea008e829
```

Commit URL:

https://github.com/bballdave025/fhtw-paper-code-prep/commit/5496291dc8dad4081d5fc4f6ba33112ea008e829

Commit message:

```text
Steps for starting AWS in new context document.
```

The exact repository path added by that commit was:

```text
docs/context_documents/LN_rmmfb_2026-10-17_-_keith-reconstruction-and-staged-transfer-addendum.md
```

Historical commit-pinned URL:

https://github.com/bballdave025/fhtw-paper-code-prep/blob/5496291dc8dad4081d5fc4f6ba33112ea008e829/docs/context_documents/LN_rmmfb_2026-10-17_-_keith-reconstruction-and-staged-transfer-addendum.md

As of the October 27 snapshot boundary, this October 17 commit is the last
relevant `fhtw-paper-code-prep` commit observed in the repository history
before later October 29 work. Do not import October 29 changes into this
October 27 snapshot merely because they are now visible on `main`.

The source document also preserved this suggested filename:

```text
LN_rmmfb_2026-10-17_-_eightfold-way-keith-reconstruction-and-ruthless-sprint.md
```

Do not silently collapse the distinction among:

- the uploaded source filename;
- the source's suggested filename;
- the filename actually committed on October 17.

## 4.2 Experiment scaffold

Current scaffold script:

```text
structure.sh
```

Current direct URL:

https://github.com/bballdave025/fhtw-paper-code-prep/blob/main/structure.sh

Current `structure.sh` supports:

```text
./structure.sh <ROOT_DIR> <tag1> [tag2 ...]
WITH_NB_STUBS=1 ./structure.sh <ROOT_DIR> <tag1> [tag2 ...]
./structure.sh --check <ROOT_DIR> <tag>
```

It creates experiment directories including:

```text
notebooks
datasets
models
logs
visualizations
scripts
outputs/csv_logs
outputs/gradcam_images
```

and files patterned as:

```text
README_${TAG_NAME}.md
__init__.py
scripts/__init__.py
scripts/py_build_model_${TAG_NAME}.py
scripts/py_train_model_${TAG_NAME}.py
scripts/py_inference_${TAG_NAME}.py
scripts/py_utils_${TAG_NAME}.py
notebooks/00_data_exploration_${TAG_NAME}.ipynb
notebooks/01_model_build_${TAG_NAME}.ipynb
notebooks/02_training_${TAG_NAME}.ipynb
notebooks/03_inference_quick_explore_${TAG_NAME}.ipynb
```

The proving-ground infrastructure has done its job. Do not create another
scaffolding project before real RMMFB execution.

## 4.3 Supporting ontology repository

Repository:

```text
bballdave025/congenial-chainsaw-rmfb-html
```

URL:

https://github.com/bballdave025/congenial-chainsaw-rmfb-html

Main classification parameter file:

```text
classifier.param
```

URL:

https://github.com/bballdave025/congenial-chainsaw-rmfb-html/blob/main/classifier.param

The repository documents the classification system and the deprecation of
`suh`.

## 4.4 Supporting older project/vision repository

Repository:

```text
bballdave025/rib-wrist-in-bin-din
```

URL:

https://github.com/bballdave025/rib-wrist-in-bin-din

This repository is useful as historical/vision lineage, but the current
publication execution belongs in `fhtw-paper-code-prep`.

## 4.5 Canonical data and Drive artifacts

Canonical local curated tree:

```text
/cygdrive/d/ds/rvc3331
```

Canonical inventory filename:

```text
consistentized_3331_dataset.txt
```

Google Drive file ID:

```text
1c2BVTQ9Fgt81FhpLG806d1r4ge5aJ4ZC
```

Canonical inventory SHA-256:

```text
4d84562384261999c6bbe81a90d0f922e9e2ab57132fef72d7f7e304985110d4
```

Historical preparation archive:

```text
dataset_preparation_examples.zip
```

Google Drive file ID:

```text
1Eo6j4JhOdnFQc73kUstCwJybZrUQcCLC
```

Recovered historical Keith folder:

```text
https://drive.google.com/drive/folders/1dlm2fumV5O-m0qJYmtRv9dj2BsBWNxU0
```

WeTransfer/evidence filename:

```text
Original_doc_names_for_Keith_01_-_First-Yes_No-sent-successfully-to-keithprisbrey68-wetransfer.pdf
```

Old directory-tree path:

```text
My Drive
>> __General_Reference
>> P
>> P2_2025_RMFB_Portable
>> P2_Dir_Tree_2025-02-05T104100-0700.txt
```

## 4.6 Group-aware split contract

Minimal manifest:

```text
relative_path,binary_label,group_id,split
```

Random seed:

```text
137
```

Priority:

> Prevent images from the same host object or closely related digitization
> sequence from appearing in multiple partitions.

Procedure:

```text
derive group_id
→ split groups
→ inspect counts
→ inspect binary balance
→ check obvious pathologies
→ freeze
→ hash manifest
→ vault test
```

Methods-language candidate:

> Images were partitioned using group-aware splitting to prevent images from
> the same source object or closely related digitization sequence from
> appearing in multiple partitions. Within those constraints, class
> distributions were balanced as closely as practicable.

Rare visual-subtype stratification is **not** an MVP requirement.

## 4.7 Test-set vault

Once the final test partition is designated:

> It becomes a vault.

Do not use final-test:

- errors;
- images;
- attribution maps;
- recurring visual patterns;
- special cases

to guide further model development.

Final paper attribution examples from the test set can be viewed after
model-selection/development choices are frozen.

Dave's prior exposure to images while constructing the dataset does not by
itself invalidate a model test.

The operational concern is post-split feedback into model decisions.

# 5. Responsibilities

A replacement RMMFB chat must continue the following responsibilities.

## 5.1 Keep the paper as trunk

The main deliverable is a defensible, minimum-publishable RMMFB experiment.

Do not convert RMMFB into:

- a general document-AI framework;
- an architecture benchmark;
- a provenance-normalization project;
- a storage-recovery project;
- a new ontology project;
- a gaze-tracking project;
- an NTEC implementation project;
- an AWS platform-engineering project.

## 5.2 Preserve the historical/prospective distinction

Historical:

```text
622-image Keith dataset
actual filenames in that recovered folder
actual Yes/No directory organization
actual model/code/settings if recovered
actual reported performance if recovered
actual later comments about harder/"fouled up" material
```

Prospective/current experimental design:

```text
+709 to reach 1331
+1000 to reach 2331
+1000 to reach 3331
group-aware split policy
seed 137
current ResNet-50 / 224 baseline
current fine-tuning experiment
current attribution protocol
current wild-corpus retrieval
```

Do not mix these categories in Methods/history narrative.

## 5.3 Protect group independence

Every image needs a defensible host-level `group_id`.

The important split constraint is leakage prevention.

Host-object leakage matters more than cosmetically perfect class balance.