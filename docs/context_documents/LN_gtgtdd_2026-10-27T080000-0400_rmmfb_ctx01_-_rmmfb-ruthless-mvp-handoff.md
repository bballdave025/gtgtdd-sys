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
CodexRestitutus fragments should be conservatively grouped by reconstructed
historical codex rather than separated merely because current institutional
holdings differ.

## 5.4 Preserve historical filenames

Do not rename frozen files merely to simplify parsing.

Adapt the parser.

Historical filename mistakes can be evidence.

The old note:

```text
Yes, two 15s, oops
```

is worth preserving because it demonstrates that certain e-codices numeric
fields were practical local identifiers, not guaranteed source ordinals.

## 5.5 Keep provenance claims cautious

Supportable claim:

> RMMFB does not merely return isolated positive images. Its retained source
> identifiers and object-level grouping permit candidate detections to be
> traced back to host volumes and neighboring observations for expert
> investigation.

Do not claim every image has:

- a persistent verified source URL;
- normalized shelfmark metadata;
- complete physical metadata;
- complete codicological description;
- expert-reviewed provenance;
- complete neighboring image coverage.

## 5.6 Run the real pipeline

After split freeze:

- use TRAIN-only images for the smoke test;
- prove S3/SageMaker/JPEG/preprocessing/ResNet/output flow;
- then run real RMMFB stages.

Do not use CIFAR again merely because it is familiar.

## 5.7 Keep exact run records

For each real run, preserve enough to reproduce:

- dataset/stage;
- split manifest/hash;
- preprocessing;
- model state;
- training settings;
- metrics;
- output artifact locations;
- relevant environment metadata.

This is experiment evidence, not optional prose.

# 6. Operating Rules

## 6.1 Ruthless search policy

Working rule:

```text
expected step time <= ~3 minutes:
    probably do it

expected step time > ~3 minutes:
    stop
    explain expected utility
    decide together
```

Especially avoid:

```text
"Let's just search everything."
```

The recovered 622 cohort substantially lowers the scientific value of broad
historical search.

## 6.2 Historical filenames are provenance artifacts

Preserve filenames.

Adapt parser.

Derive `group_id`.

Move on.

## 6.3 e-codices rule

Numeric fields in e-codices-derived filenames are not always literal
source-system ordinals.

An old note explicitly uses:

```text
My Enumeration (continue beginning, change the later ones)
```

Some e-codices-derived filenames also lack the literal token:

```text
ecod
```

An old extraction note explicitly warned:

```text
doesn't take care of missing 'e-cod's
```

Therefore:

> Do not determine e-codices provenance solely from presence of `ecod`.

## 6.4 Cambridge filename rule

Example:

```text
Cambridge_MS-ADD-10139-000-00001_orc.jpg
```

The old parser expected an underscore before the five-digit identifier.

Cambridge uses hyphenation.

Adapt the parser. Do not rename the file.

## 6.5 CodexRestitutus grouping rule

Examples:

```text
CodexRestitutus-ecod-003_-_BibliaTheodulfi_...
CodexRestitutus-ecod-004_-_FuldaLegendary_...
CodexRestitutus-ecod-005_-_BibliaAlcuini_...
```

Group by reconstructed historical codex rather than present-day institution.

Conservative over-grouping is preferable to leakage.

## 6.6 ePaveldas is closed

The final grep returned:

```text
no matches
```

Do not reopen ePaveldas provenance unless a concrete scientific blocker
appears.

## 6.7 Stage selection must be pre-outcome

Current progression:

```text
Stage A:  622
Stage B: 1331 = 622 + 709
Stage C: 2331 = 1331 + 1000
Stage D: 3331 = 2331 + final 1000
```

Interpretation:

```text
622:
historical/easy cohort

1331:
prospective first expansion

2331:
prospective second expansion

3331:
full corpus / later final expansion
```

The additional examples must be selected/frozen before performance results
influence selection.

## 6.8 Low-resolution baseline is fixed

Use:

```text
ImageNet-pretrained ResNet-50
224 x 224 input
frozen pretrained backbone
trained binary RMMFB head / linear probe
```

A stock 1000-way ImageNet classification head is not the meaningful baseline.

The actual baseline is:

```text
ImageNet representation
+
RMMFB-trained binary head
```

## 6.9 Fine-tune the same model before changing model family

Keep:

```text
ResNet-50
224 x 224
same split
same preprocessing
same dataset stage
```

Then fine-tune.

Metrics:

- accuracy;
- precision;
- recall;
- F1;
- confusion matrix.

Recall is especially important for discovery use.

## 6.10 Attribution is bounded

Use the existing selected lineage:

```text
Guided Grad-CAM
guided backpropagation
Grad-CAM-related code
```

Do not start an attribution-method survey.

Attribution means:

> regions influential to the model's decision

not:

> proof that the network reasons like a manuscript scholar.

## 6.11 Wild-corpus stage is retrieval, not population benchmark

Run a frozen useful model over approximately:

```text
41,790 wild candidate images
```

Save at minimum:

```text
source identifier
model score
rank
predicted class / threshold result
```

Potentially:

```text
review status
expert note
```

Goal:

> Surface plausible previously unreviewed reused-manuscript candidates for
> expert investigation.

## 6.12 Smoke test is TRAIN-only

After split freeze:

```text
sample 32–64 random TRAIN images
```

Use no validation or final-test images for the plumbing run.

Purpose:

```text
S3
→ SageMaker
→ JPEG decode
→ preprocessing
→ ResNet-50 path
→ output artifact
→ S3
```

The smoke test answers:

> Does the real RMMFB pipeline work?

It does not need meaningful performance.

## 6.13 AWS/SageMaker must remain lean

Current plan:

- one AWS region;
- S3 for durable inputs/artifacts;
- SageMaker working storage/cache for active runs;
- Managed Spot for meaningful training when convenient;
- tiny on-demand job acceptable if it removes friction from the smoke test;
- ordinary SageMaker checkpoint support if useful;
- no custom recovery platform.

Potential checkpoint path:

```text
/opt/ml/checkpoints
```

with:

```text
checkpoint_s3_uri
```

if/when training duration warrants it.

## 6.14 Preprocessing contract

Main model input:

```text
224 x 224
```

Use preprocessing associated with the selected TorchVision pretrained
ResNet-50 weights.

Do not invent a bespoke normalization scheme without evidence.

Historical source preprocessing broadly included:

- normalization of source web formats;
- PDF rendering/extraction;
- conversion through PNG in some workflows;
- later JPEG encoding;
- RGB-compatible representation;
- consistent treatment of curated and wild corpora where practical.

## 6.15 Historical input resolution remains unresolved unless cheaply recovered

Recollection:

```text
175 x 175
```

Do not convert that recollection into fact.

If actual value is cheap to recover, recover it.

Otherwise:

```text
record as unresolved historical implementation detail
use 224 for current experiment
continue
```

# 7. Immediate Next Actions

The next chat should not ask what project to do.

The project is known.

The experiment is known.

The historical anchor exists.

## 7.1 Preserve the recovered 622 cohort

Record:

```text
Drive folder
exact file count
directory structure
class counts
```

Do not perform broad archaeology.

If a cheap filename manifest can be generated, save it.

## 7.2 Finish `group_id` logic for the canonical 3,331

Every image needs a defensible host-level grouping key.

No filename renaming.

## 7.3 Create group-aware train/validation/test split

Use:

```text
SEED = 137
```

Check:

- group leakage;
- overall partition counts;
- binary class balance;
- obvious giant groups.

Then freeze.

## 7.4 Hash the split manifest

Record:

```text
manifest filename
SHA-256
partition counts
class counts
```

Then:

```text
TEST = VAULT
```

## 7.5 Freeze the prospective expansion schedule

Use:

```text
622
1331
2331
3331
```

Document how the 709 and +1000 subsets are selected **before** performance is
used to choose them.

## 7.6 Run TRAIN-only SageMaker smoke

Use:

```text
32–64 TRAIN images
```

Prove the real pipeline.

## 7.7 Run the 622 experiment

This is both:

- historically meaningful;
- experimentally easy/obvious.

Reconstruct Keith only as far as cheap evidence permits.

## 7.8 Run 1331

Use the prospectively fixed expansion.

## 7.9 Run 2331

Use the next prospectively fixed expansion.

## 7.10 Decide later whether full 3331 is needed immediately

Possible answer:

```text
yes
```

if cheap and useful.

Possible answer:

```text
leave the final 1000 untouched until the first paper results exist
```

Do not solve this prematurely.

# 8. Cross-Chat Dependencies

## 8.1 uGTgtdD / system conductor

Expected sibling:

[`LN_gtgtdd_2026-10-27T080000-0400_ugtgtdd_ctx01_-_system-conductor-handoff.md`](./LN_gtgtdd_2026-10-27T080000-0400_ugtgtdd_ctx01_-_system-conductor-handoff.md)

uGTgtdD should know:

- RMMFB is a protected active research/portfolio priority;
- the next scientific move is not "research more" but split/freeze/smoke/run;
- stale "week-to-submit" wording should not become an invented deadline;
- technical decisions belong here, not in the action system.

Relevant Asana capture from the system conductor:

```text
RMMFB — week-to-submit
```

The task is a project-level outcome, not proof of a literal due date.

## 8.2 Job Hunt

Expected sibling:

[`LN_gtgtdd_2026-10-27T080000-0400_jobhunt_ctx01_-_job-search-conductor-handoff.md`](./LN_gtgtdd_2026-10-27T080000-0400_jobhunt_ctx01_-_job-search-conductor-handoff.md)

RMMFB contributes to Dave's job-search positioning through:

- computer vision;
- dataset curation;
- provenance;
- difficult negatives;
- error analysis;
- experiment design;
- reproducibility;
- explainability;
- research writing.

But job-search needs should not rewrite the scientific protocol.

"Portfolio for free" means that good scientific execution naturally produces
portfolio evidence.

## 8.3 Interview Prep

Expected sibling:

[`LN_gtgtdd_2026-10-27T080000-0400_interviewprep_ctx01_-_interview-preparation-handoff.md`](./LN_gtgtdd_2026-10-27T080000-0400_interviewprep_ctx01_-_interview-preparation-handoff.md)

RMMFB examples may support interview stories about:

- segmentation/computer vision;
- data provenance;
- annotation;
- difficult negatives;
- scientific measurement;
- test leakage;
- experimental discipline.

Do not pause RMMFB merely to create interview-demo polish unless a concrete
interview requires it.

## 8.4 FP↑ / upskilling collaboration work

Expected sibling:

[`LN_gtgtdd_2026-10-27T080000-0400_upskillingcollabs_ctx01_-_fort-point-upskilling-collabs-handoff.md`](./LN_gtgtdd_2026-10-27T080000-0400_upskillingcollabs_ctx01_-_fort-point-upskilling-collabs-handoff.md)

Do not let collaboration scaffolding consume the RMMFB execution window.

## 8.5 Future project-level RMMFB LN

This `gtgtdd-sys` handoff should eventually point to a same-snapshot project
LN committed inside `fhtw-paper-code-prep`.

That project-level LN can carry more technical state, exact commands, experiment
artifacts, and repo history.

This system-level handoff should remain the concise bridge from whole-system
state into the technical project.

# 9. Known Risks / Things Not to Re-derive

## 9.1 Do not reopen the 3,331 reconciliation

It is done.

Canonical inventory:

```text
consistentized_3331_dataset.txt
```

File ID:

```text
1c2BVTQ9Fgt81FhpLG806d1r4ge5aJ4ZC
```

SHA-256:

```text
4d84562384261999c6bbe81a90d0f922e9e2ab57132fef72d7f7e304985110d4
```

## 9.2 Do not re-run provenance archaeology without a concrete blocker

The filename audit is sufficiently complete for host-level grouping.

ePaveldas is closed.

e-codices local enumerations are understood well enough.

Cambridge is a source-specific naming exception.

CodexRestitutus needs conservative grouping.

## 9.3 The 622 are history; 709 is arithmetic

Remember:

> The 622 are real history.

> The 709 is arithmetic, not archaeology.

> The +1000 stages are current experimental design.

> The 3331 did not exist as a completed corpus in 2024.

> The final 3331 was the Fall 2025 "stop collecting and publish" hammer.

Do not create a false historical narrative around the later stages.

## 9.4 Do not require the failed 14-TB drive

The project can proceed without it.

Backups may exist.

That does not make searching them the trunk.

## 9.5 Do not substitute architecture shopping for model execution

Current baseline/fine-tuning path is ResNet-50 / 224.

Do not replace it with transformers, EfficientNet, Hi-ResNet, or a broad model
comparison before current experiments run.

## 9.6 Do not leak final-test information

No repeated final-test:

- error inspection;
- image inspection;
- attribution-map inspection;
- special-case mining

during model development.

## 9.7 Do not confuse attribution with scholarly reasoning

Grad-CAM-style maps are model-influence visualizations, not proof that the
model "sees what a manuscript scholar sees."

## 9.8 Do not overclaim wild-corpus metrics

The wild corpus is not comprehensively labeled.

Way 8 is retrieval/discovery.

## 9.9 Do not resurrect `suh`

Historical `_suh` tokens remain in frozen filenames.

The current label is deprecated.

## 9.10 Do not spend a sprint proving irrelevant image-conversion trivia

Check exact historical conversion details only if they materially affect the
Methods claim.

## 9.11 Do not let the new snapshot overwrite exact identifiers

This system-level reorganization must preserve exact:

- URLs;
- Drive file IDs;
- filenames;
- repository names;
- repository paths;
- branch names;
- local filesystem paths;
- hashes.

A cleaner outline is not permission to lose retrieval anchors.

## 9.12 Do not import post-snapshot repo changes into October 27 state

The repository now contains later October 29 work.

This snapshot is anchored to October 27.

Use later repo state only to recover or verify identifiers, and label it
explicitly if mentioned.

# 10. Handoff to the Next Chat

A replacement RMMFB chat should start like this:

1. Read this handoff once.
2. Open the October 17 source only if more historical detail is needed.
3. Do **not** begin with general provenance archaeology.
4. Verify/preserve the 622 cohort cheaply.
5. Finish `group_id`.
6. Create/freeze/hash the group-aware split using seed 137.
7. Vault the test set.
8. Run the 32–64 TRAIN-image real-pipeline SageMaker smoke test.
9. Run the 622 baseline.
10. Expand prospectively to 1331 and 2331.
11. Decide later whether to expose the final 1000 immediately.
12. Continue the Eightfold Way.

The continuation anchor is:

> Group the data.

> Freeze the split.

> Run the smoke test.

> Run 622.

> Expand prospectively.

> Get results.

The runway has been documented enough.

**Run.**

# 11. Exact Identifier and Retrieval Ledger

**The subject, _Exact Identifier and Retrieval Ledger_, would fit well inside
§4, but it currently exists at §11 so the shared §§1–10 first-draft spine
remains intact.**

This ledger exists specifically to prevent exact retrieval anchors from being
lost during summarization.

## 11.1 Primary source filenames

Uploaded source used for this remoulding:

```text
LN_rmmfb_2026-10-17_ctx-try-02_-_keith-reconstruction-and-staged-transfer-addendum.md
```

Source-preserved suggested filename:

```text
LN_rmmfb_2026-10-17_-_eightfold-way-keith-reconstruction-and-ruthless-sprint.md
```

Repository filename actually added October 17:

```text
docs/context_documents/LN_rmmfb_2026-10-17_-_keith-reconstruction-and-staged-transfer-addendum.md
```

## 11.2 Primary repository

```text
bballdave025/fhtw-paper-code-prep
```

```text
main
```

```text
docs/context_documents/README.md
```

Repository URL:

https://github.com/bballdave025/fhtw-paper-code-prep

October 17 commit:

```text
5496291dc8dad4081d5fc4f6ba33112ea008e829
```

Commit URL:

https://github.com/bballdave025/fhtw-paper-code-prep/commit/5496291dc8dad4081d5fc4f6ba33112ea008e829

Historical commit-pinned addendum URL:

https://github.com/bballdave025/fhtw-paper-code-prep/blob/5496291dc8dad4081d5fc4f6ba33112ea008e829/docs/context_documents/LN_rmmfb_2026-10-17_-_keith-reconstruction-and-staged-transfer-addendum.md

Earlier context filenames:

```text
LN_rmmfb_2026-09-09_-_minimum-publishable-paper-plan.md
LN_rmmfb_2026-09-18_-_mvp-scaffold-closed-and-execution-plan.md
LN_rmmfb_2026-10-10_-_provenance-aware-split-and-mvp-execution-state.md
```

## 11.3 Canonical dataset

```text
/cygdrive/d/ds/rvc3331
```

```text
consistentized_3331_dataset.txt
```

```text
1c2BVTQ9Fgt81FhpLG806d1r4ge5aJ4ZC
```

```text
4d84562384261999c6bbe81a90d0f922e9e2ab57132fef72d7f7e304985110d4
```

## 11.4 Historical dataset-preparation evidence

```text
dataset_preparation_examples.zip
```

```text
1Eo6j4JhOdnFQc73kUstCwJybZrUQcCLC
```

## 11.5 Recovered Keith cohort

```text
https://drive.google.com/drive/folders/1dlm2fumV5O-m0qJYmtRv9dj2BsBWNxU0
```

```text
Original_doc_names_for_Keith_01_-_First-Yes_No-sent-successfully-to-keithprisbrey68-wetransfer.pdf
```

```text
My Drive
>> __General_Reference
>> P
>> P2_2025_RMFB_Portable
>> P2_Dir_Tree_2025-02-05T104100-0700.txt
```

```text
BigDatasetReuse_<date>
Yes_Reuse
No_Reuse
Not_Reuse
```

## 11.6 Filename/provenance examples that must not be normalized away

```text
Cambridge_MS-ADD-10139-000-00001_orc.jpg
```

```text
CodexRestitutus-ecod-003_-_BibliaTheodulfi_...
CodexRestitutus-ecod-004_-_FuldaLegendary_...
CodexRestitutus-ecod-005_-_BibliaAlcuini_...
```

## 11.7 Split / AWS exact technical identifiers

```text
relative_path,binary_label,group_id,split
```

```text
137
```

```text
/opt/ml/checkpoints
```

```text
checkpoint_s3_uri
```

## 11.8 Experiment scaffold

```text
structure.sh
```

URL:

https://github.com/bballdave025/fhtw-paper-code-prep/blob/main/structure.sh

## 11.9 Supporting repository identifiers

```text
bballdave025/congenial-chainsaw-rmfb-html
```

https://github.com/bballdave025/congenial-chainsaw-rmfb-html

```text
classifier.param
```

https://github.com/bballdave025/congenial-chainsaw-rmfb-html/blob/main/classifier.param

```text
bballdave025/rib-wrist-in-bin-din
```

https://github.com/bballdave025/rib-wrist-in-bin-din

# 12. The Eightfold Way

**The subject, _The Eightfold Way_, would fit well between §3 and §5, but it
currently exists at §12.**

This is the agreed experimental spine.

Do not replace it.

## 12.1 Way 1 — Lock Claim and Experimental Contract

Freeze:

- binary task;
- metrics;
- grouping/leakage rule;
- dataset stages;
- preprocessing;
- resolution;
- completion criteria.

Most conceptual work is complete.

Remaining execution is chiefly:

```text
group_id
→ split
→ freeze/hash
→ vault test
```

## 12.2 Way 2 — Reconstruct Keith's Historical Experiment

Historical dataset recovered:

```text
https://drive.google.com/drive/folders/1dlm2fumV5O-m0qJYmtRv9dj2BsBWNxU0
```

```text
622 images
```

Cheaply recover, when available:

- 622 filenames;
- positive/negative directory structure;
- exact counts by class;
- old model code;
- old resize/input size;
- split behavior;
- whether host-related images crossed partitions;
- reported result;
- later "fouled up" cohort if it happens to be easy to find.

Do **not** require reconstruction of every historical intermediate dataset.

## 12.3 Way 3 — Freeze Difficulty Progression

```text
Stage A:  622
Stage B: 1331 = 622 + 709
Stage C: 2331 = 1331 + 1000
Stage D: 3331 = 2331 + final 1000```

Do not describe 1331 or 2331 as reconstructed historical milestones.

## 12.4 Way 4 — Frozen-Backbone ResNet-50 Baseline

```text
ImageNet-pretrained ResNet-50
224 x 224 input
frozen pretrained backbone
trained binary RMMFB head / linear probe
```

## 12.5 Way 5 — Fine-Tune Same Model

```text
ResNet-50
224 x 224
same split
same preprocessing
same dataset stage
```

Metrics:

- accuracy;
- precision;
- recall;
- F1;
- confusion matrix.

## 12.6 Way 6 — Attribution

```text
Guided Grad-CAM
guided backpropagation
Grad-CAM-related code
```

Useful final examples may include:

- true positive;
- true negative;
- false positive;
- false negative;
- obvious reuse;
- subtle reuse.

## 12.7 Way 7 — One Richer-Label Experiment

Run **one** controlled richer-label experiment using the existing ontology.

Do not turn this into a taxonomy benchmark project.

## 12.8 Way 8 — Wild-Corpus Retrieval

Run frozen useful model against:

```text
41,790 wild candidate images
```

Save:

```text
source identifier
model score
rank
predicted class / threshold result
```

Potentially:

```text
review status
expert note
```

This is candidate discovery, not comprehensive closed-set evaluation.

# 13. Historical Versus Prospective Staging

**The subject, _Historical Versus Prospective Staging_, would fit well between
§3 and §6, but it currently exists at §13.**

The recovered **622-image set** is historically meaningful.

It is the successful early dataset sent to Keith and associated with the first
well-performing RMMFB experiment.

The later numbers **709** and **1000** are **not reconstructed historical
cohorts**.

The value `709` was chosen simply because:

```text
622 + 709 = 1331
1331 + 1000 = 2331
2331 + 1000 = 3331
```

The final 3,331-image corpus did not yet exist in 2024.

The `3331` corpus was a Fall 2025 stopping point intended to enforce:

> Stop collecting. Finish classification. Build models. Publish.

Reasonable current progression:

```text
622   historical Keith/easy cohort
1331  622 + 709
2331  +1000
3331  final +1000, initially left untouched
```

The post-622 stages are **prospective experimental staging choices**.

They are not claims about:

- historical acquisition order;
- historical discovery order;
- what was sent to Keith next;
- what images existed by a particular 2024 date.

It is currently unknown how many members of the eventual 3,331 had actually
been discovered by the end of February 2024.

Do not invent that history.

Leaving the final:

```text
1000
```

temporarily untouched is a pragmatic anti-scope-drift choice, not a sacred
principle.

# 14. Provenance and Grouping Decisions

**The subject, _Provenance and Grouping Decisions_, would fit well between §4
and §6, but it currently exists at §14.**

## 14.1 e-codices

Historical working documents show that Dave sometimes:

- preserved obvious early image sequence numbers;
- manually counted grid positions;
- retained source folio/page names;
- assigned compact local identifiers to later images of interest;
- created source mapping tables with display URLs/download URLs;
- preserved earlier names.

Old note:

```text
My Enumeration (continue beginning, change the later ones)
```

Historically useful line:

```text
Yes, two 15s, oops
```

Preserve the `oops`.

Some e-codices-derived filenames lack:

```text
ecod
```

Old extraction warning:

```text
doesn't take care of missing 'e-cod's
```

## 14.2 Cambridge

Example:

```text
Cambridge_MS-ADD-10139-000-00001_orc.jpg
```

Adapt parser. Do not rename.

## 14.3 CodexRestitutus

```text
CodexRestitutus-ecod-003_-_BibliaTheodulfi_...
CodexRestitutus-ecod-004_-_FuldaLegendary_...
CodexRestitutus-ecod-005_-_BibliaAlcuini_...
```

Group by explicitly reconstructed historical codex.

## 14.4 Provenance claim

Supportable:

> RMMFB does not merely return isolated positive images. Its retained source
> identifiers and object-level grouping permit candidate detections to be
> traced back to host volumes and neighboring observations for expert
> investigation.

Do not turn retained provenance into a claim of fully normalized scholarly
cataloguing.

# 15. Model, Attribution, and AWS Contract

**The subject, _Model, Attribution, and AWS Contract_, would fit well between
§6 and §7, but it currently exists at §15.**

## 15.1 Baseline

```text
ImageNet-pretrained ResNet-50
224 x 224 input
frozen pretrained backbone
trained binary RMMFB head / linear probe
```

## 15.2 Fine-tuning

```text
ResNet-50
224 x 224
same split
same preprocessing
same dataset stage
```

## 15.3 Attribution

```text
Guided Grad-CAM
guided backpropagation
Grad-CAM-related code
```

## 15.4 Smoke path

```text
S3
→ SageMaker
→ JPEG decode
→ preprocessing
→ ResNet-50 path
→ output artifact
→ S3
```

## 15.5 Checkpointing if warranted

```text
/opt/ml/checkpoints
```

```text
checkpoint_s3_uri
```

Do not build a custom recovery platform.

# 16. Parked Branches and Explicit Non-Goals

**The subject, _Parked Branches and Explicit Non-Goals_, would fit well between
§9 and §10, but it currently exists at §16.**

## 16.1 Higher-resolution branch — parked

Scientifically interesting because small reused fragments can disappear under
aggressive global downsampling.

Bounded future candidate:

```text
672 x 672 image
→ 3 x 3 non-overlapping 224 tiles
→ ordinary ImageNet-pretrained ResNet-50 per tile
→ simple predeclared aggregation
```

Other captured possibilities:

```text
448 whole-image ResNet
672 whole-image ResNet
896 whole-image ResNet
Hi-ResNet
larger tiling schemes
```

Rule:

> 224 first.

## 16.2 Hi-ResNet — parked

Working understanding from prior inspection:

```text
added high-resolution front end:
new/randomly initialized

surviving ResNet-50 trunk:
ImageNet pretrained

task head:
newly trained
```

Do not spend time checking repository history unless Hi-ResNet is promoted into
the experiment.

## 16.3 NTEC — parked

```text
Nyquist Text Existence Criterion
```

Potential descriptors:

- scale-space;
- Fourier information;
- gradients;
- entropy;
- regional measurements.

Useful conceptual formulation:

> Given this measurement of this region, is enough writing-specific
> information recoverable that NTEC cannot disqualify the region as text?

Not needed for the current RMMFB paper.

## 16.4 Explicit non-goals

Do not currently:

- search every external drive;
- recover the failed 14-TB drive;
- reconstruct every historical dataset version;
- prove exactly how many eventual 3331 images existed in February 2024;
- recreate missing acquisition chronology;
- rebuild every WeTransfer package;
- reconstruct every e-codices download;
- reopen ePaveldas provenance;
- rename frozen files;
- redesign the ontology;
- resurrect `suh`;
- build rare-subtype stratification machinery;
- inspect final-test attribution during development;
- replace ResNet-50;
- introduce transformers;
- run architecture bake-offs;
- implement NTEC;
- build Hi-ResNet;
- solve GitHub integration mechanics;
- overengineer SageMaker;
- clean all repository history;
- polish documentation instead of running models.

# 17. Current Main Research Sequence

**The subject, _Current Main Research Sequence_, would fit well immediately
after §7, but it currently exists at §17.**

```text
622 historical cohort secured
        ↓
freeze group_id + split
        ↓
freeze 622 / 1331 / 2331 / 3331 staging
        ↓
32–64 TRAIN-image SageMaker smoke
        ↓
reconstruct only cheap Keith details
        ↓
622 frozen-backbone ResNet-50 baseline
        ↓
1331
        ↓
2331
        ↓
decide whether/when to expose final 1000
        ↓
fine-tune same model
        ↓
quantitative evaluation
        ↓
Guided Grad-CAM / guided backprop
        ↓
one richer-label experiment
        ↓
freeze useful model
        ↓
~41,790-image wild retrieval
        ↓
expert review
        ↓
paper
```

The final rule remains:

> **We have documented the runway. Keep flying.**

---

*END: Context Document*