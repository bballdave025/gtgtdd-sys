# Boston→Bountiful Continuation Map

Snapshot family: `2026-10-27T080000-0400`

This is the front door for Dave BLACK's coordinated October 27, 2026
Boston→Bountiful checkpoint. The timestamp identifies the shared snapshot
family; the files were assembled and edited later. The point is to preserve a
usable cross-section of active systems and materially relevant projects at the
boundary, not to pretend that the documentation itself was finished before
Dave left Boston.

Use this file to choose the **smallest authoritative context** needed for the
next piece of work. Do not read every linked document before acting.

## 1. Restart from here

- For cross-project priorities, Asana state, waiting-for items, or "what should
  happen next?", start with
  [uGTgtdD / system conductor](./LN_gtgtdd_2026-10-27T080000-0400_ugtgtdd_ctx01_-_system-conductor-handoff.md).
- For applications, job fit, employer events, application materials, or
  candidate positioning, start with
  [Job Hunt](./LN_gtgtdd_2026-10-27T080000-0400_jobhunt_ctx01_-_job-search-conductor-handoff.md).
- For role-specific interview preparation, talking points, or Sonari
  post-interview preparation evidence, start with
  [Interview Prep](./LN_gtgtdd_2026-10-27T080000-0400_interviewprep_ctx01_-_interview-preparation-handoff.md).
- For Fort Point collaboration launches, questionnaires, mentor/learner access,
  or bespoke collaboration repositories, start with
  [FP↑ / Upskilling Collaborations](./LN_gtgtdd_2026-10-27T080000-0400_upskillingcollabs_ctx01_-_fort-point-upskilling-collabs-handoff.md).
- For the RMMFB scientific/publication program, start with
  [RMMFB ruthless MVP](./LN_gtgtdd_2026-10-27T080000-0400_rmmfb_ctx01_-_rmmfb-ruthless-mvp-handoff.md),
  then descend into the project repository only as needed.
- For a technical project not represented by one of those system contexts,
  use the project/repository summary below and then open the repository or its
  project-level context document.

## 2. System-level contexts

### uGTgtdD / system conductor

**Status:** ACTIVE — orchestration layer

[Open the system-conductor context](./LN_gtgtdd_2026-10-27T080000-0400_ugtgtdd_ctx01_-_system-conductor-handoff.md)

This is the canonical cross-domain action/orchestration handoff. It preserves
Asana as canonical actionable state, Drive as durable evidence/artifact
storage, GitHub as code/project truth, and domain chats as owners of their
semantic decisions. It also records the known October 27 reconciliation gaps,
including Sonari's post-interview state and Amazon Req. 10552991's role
closure. General Capture remains intentionally loose; it is not a mandate to
organize every captured branch. The governing rules are "Capture the branch.
Stay on the trunk." and "Lean-to, not cathedral." A replacement conductor
should use this file to decide what is active, waiting, parked, or merely
captured, then open only the relevant sibling context.

### Job Hunt

**Status:** ACTIVE — employment pipeline and candidate strategy

[Open the job-search context](./LN_gtgtdd_2026-10-27T080000-0400_jobhunt_ctx01_-_job-search-conductor-handoff.md)

This document owns fit assessment, application treatment, employer-specific
positioning, evidence selection, and the semantic meaning of hiring events.
It records the October 26 Sonari conversation as encouraging but explicitly
not an offer, with possible consulting still only a discussion. It preserves
the evidence-backed submitted pipeline, actual closed outcomes, meaningful
leads, and exact role/evidence links. It also separates application activity
from project/research evidence: applications distribute existing evidence,
while completed experiments can strengthen that evidence. Detailed departure,
benefits, and Amazon administrative material stays here rather than becoming a
general uGTgtdD narrative. A replacement job-hunt chat should execute from the
current pipeline rather than rebuild Dave's career history.

### Interview Prep

**Status:** WAITING / REUSABLE — Sonari interview complete; assets ready

[Open the interview-preparation context](./LN_gtgtdd_2026-10-27T080000-0400_interviewprep_ctx01_-_interview-preparation-handoff.md)

This document owns concrete interview preparation, role-to-experience mapping,
spoken-answer capture, correction of claims, and reusable talking-point
artifacts. Its completed case is Sonari: the October 26 conversation occurred,
Dave reports that it went well, and no offer exists. Twenty likely questions,
talking cards, detailed contribution references, and a reusable evidence
collection were already created. The preparation process is intentionally
bounded: retrieve relevant evidence, produce usable cues, practice enough to
speak naturally, then stop. It should not become a second job-search tracker
or manufacture technical projects merely because unused preparation material
exists. The next substantive work depends on a real debrief request or a new
interview.

### FP↑ / Upskilling Collaborations

**Status:** ACTIVE — real launches underway; process still being tested

[Open the FP↑ context](./LN_gtgtdd_2026-10-27T080000-0400_upskillingcollabs_ctx01_-_fort-point-upskilling-collabs-handoff.md)

FP↑ is the collaboration-launch system for turning reusable teaching
scaffolds into private, participant-specific repositories. By the checkpoint,
the public organization hub existed, the Rubric Attribution Lab had a private
bespoke repository, and verified default ZIP/checksum packages existed for
Rubric Attribution Lab, JabberVec-l2v, and Roman Numeral Word Lab. Several
questionnaires and participant launches were still waiting on sending,
response, invitation acceptance, or repository creation. The important
boundary is between process and participant movement: a useful launch outranks
more template/platform design. Learners are normally outside collaborators
with `Write`, private by default, and public release requires an explicit
privacy/IP/provenance review. Once a bespoke repo exists, algorithmic and code
work moves to that project rather than staying in the FP↑ conductor.

### RMMFB ruthless MVP

**Status:** ACTIVE / PROTECTED — primary research/publication project

[Open the RMMFB system handoff](./LN_gtgtdd_2026-10-27T080000-0400_rmmfb_ctx01_-_rmmfb-ruthless-mvp-handoff.md)

RMMFB is large enough to remain a substantial system-level context rather than
a thin pointer to a repository. At the checkpoint, the canonical 3,331-image
corpus had been reconciled, the filename/provenance audit was closed, and the
historical 622-image Keith cohort had been recovered. The scientific trunk was
already fixed: derive/freeze group-aware splits, vault the test set, run a
TRAIN-only SageMaker smoke test, establish the 622 baseline, then expand
prospectively to 1331 and 2331 before deciding whether to expose the final
1000. The current model family remains ImageNet-pretrained ResNet-50 at 224×224
with a frozen-backbone binary-head baseline followed by fine-tuning; Guided
Grad-CAM/guided backpropagation is the bounded attribution lineage. The
historical/prospective distinction is crucial: 622 is real history, while 709
and the +1000 stages are current experimental design. The next useful act is
execution, not another provenance expedition or architecture survey.

## 3. Project / repository snapshots

These entries are deliberately shorter than full project lab notebooks. A
project-level LN should be added in the project repository when one already
exists or when further technical continuation would otherwise require
re-derivation. The summaries below are anchored to repository state at or
before the October 27 snapshot boundary; later editorial decisions affect
priority/navigation, not the historical project state.

### RMMFB / `fhtw-paper-code-prep`

**Snapshot status:** ACTIVE / PROTECTED

**Repository:** https://github.com/bballdave025/fhtw-paper-code-prep

**System context:** [RMMFB ruthless MVP](./LN_gtgtdd_2026-10-27T080000-0400_rmmfb_ctx01_-_rmmfb-ruthless-mvp-handoff.md)

**Closest project checkpoint at the boundary:**  
https://github.com/bballdave025/fhtw-paper-code-prep/blob/5496291dc8dad4081d5fc4f6ba33112ea008e829/docs/context_documents/LN_rmmfb_2026-10-17_-_keith-reconstruction-and-staged-transfer-addendum.md

RMMFB is Dave's primary model/research project in the current portfolio and
publication push. It combines original research questions, the manually
curated 3,331-image dataset, a custom binding-reuse ontology, provenance
reconstruction, difficult negatives/fake-outs, historical collaboration with
Keith Prisbrey, and a larger ~41,790-image discovery corpus. By the boundary,
the 3,331 inventory was reconciled exactly and the historically meaningful
622-image Keith cohort had been recovered. The remaining pre-model work had
narrowed to group-aware splitting, manifest freezing/hashing, and a strict
test-vault contract. The Eightfold Way then calls for a real RMMFB pipeline
smoke test, a frozen-backbone ResNet-50 binary baseline, fine-tuning, bounded
attribution, one richer-label experiment, and wild-corpus retrieval. The
project should not be expanded into an architecture bake-off, backup-recovery
program, or generalized manuscript-AI platform before those results exist.
Its system-level importance comes from both publication value and its role as
strong evidence of Dave's research, CV, dataset, provenance, and experimental
judgment.

### NTEC / `nyquist-text-existence`

**Snapshot status:** ACTIVE RESEARCH — preregistered; exploratory/addendum work ongoing

**Repository:** https://github.com/bballdave025/nyquist-text-existence

**Preregistration:**  
https://github.com/bballdave025/nyquist-text-existence/blob/6af2f705a498b858ba54f1782e932cea0d7d9429/PREREGISTRATION_NTEC_2026-03-02.md

NTEC asks a different question from OCR or recognition: whether
writing-specific evidentiary signal still exists in a sampled image at all.
The preregistration distinguishes text existence from recognition, model
uncertainty from information-theoretic absence, and recoverable from
unrecoverable signal. Its core predictions include abrupt failure under
downsampling, model-agnostic failure after signal loss, and human–machine
parity once the relevant evidence is gone. The preregistration also defines
Image B as an anchor case and specifies deterministic crop-selection and
falsification logic rather than allowing outcome-driven crop substitution.
By early October, the repository had added examples emphasizing regional and
measurement dependence plus an additional BnF manuscript addendum. This
project should remain separate from RMMFB even though the two inform each
other: RMMFB is a classifier/discovery program, while NTEC is a
model-agnostic boundary/measurement claim. The next work should preserve the
locked theoretical distinctions and move the observable/confirmatory program
forward without turning every exploratory descriptor into a preregistered
claim.

### JabberVec-l2v

**Snapshot status:** ACTIVE / BOUNDED COMPLETION

**Repository:** https://github.com/bballdave025/jabbervec-l2v

JabberVec-l2v is a deliberately small character-level language-model and
embedding-geometry laboratory with a playful literary-nonsense framing. By the
boundary, the repository had installation/run instructions, a tiny training
path, text generation, PCA visualization, and planned low-rank/SVD
experiments. The smallest useful portfolio path was already clear: run the
tiny corpus, generate a few strings, produce one embedding PCA plot, and
explain what it makes visible. A concrete bug was identified in the generation
path: `generate_text` initializes `hidden = None` and feeds
`x[:, -1:]`, so a multi-character prompt conditions the first generated token
only on its final character even though the full prompt is displayed. That
makes prompt-conditioning repair a good bounded issue/PR-sized completion
rather than a reason to redesign the model. After the fix, a tiny reproducible
run, generation examples, and an embedding visualization would make the repo
substantially easier to evaluate. Larger arbitrary-mapping and rank-research
ideas remain optional branches.

### Bilingual Boundary Lab / `bilingual-boundary-lab`

**Snapshot status:** USABLE ARTIFACT / HOLD SCOPE

**Repository:** https://github.com/bballdave025/bilingual-boundary-lab

**Existing project context:**  
https://github.com/bballdave025/bilingual-boundary-lab/blob/05baaa4ecac559b6c053b9097577e2e4c3e2ced8/docs/context_documents/LN_bbl_2026-10-19_ctx01_-_experiment-00-prefix-zoom.md

Bilingual Boundary Lab is a visualization-first experiment using the
Russian/French text of *War and Peace* to see what deliberately simple
statistical language models reveal about script/language boundaries and local
persistence. By October 19, the corpus had been recovered, Experiment 00
produced canonical run data and logarithmic boundary visualizations, and the
repository recorded 6,370 script-class runs across 450,660 normalized tokens.
The Python suite passed 19 tests, the PowerShell scaffold safety check passed,
and the prefix-detail visualization path had been validated. The repo already
had an explicit continuation document and a reproducible corpus builder, so it
was beyond "idea only" status. Planned follow-ups included a guiding notebook,
a general text generator, and a longer generated-versus-real comparison, but
the context explicitly warned against endless polish and asked Dave to bring
other projects to concrete-artifact level. For job-search purposes, this repo
already had usable experimental results and does not need automatic scope
expansion before it can be shown.

### Latent Forge / `latent-forge`

**Snapshot status:** PARKED / NEXT MODEL-DEVELOPMENT CANDIDATE

**Repository:** https://github.com/bballdave025/latent-forge

Latent Forge is a lean recommender-system experiment organized around a simple
measurement rule: improve holdout MSE through small, interpretable changes
rather than through architecture shopping. The repository's trunk is to
reproduce a course rank-1/item-mean baseline, add global/user/item bias
structure, then try low-rank latent factors under the same validation
protocol. The "Dave Rule" requires every change to state which assumption it
changes, why it should help, how success will be measured, and whether the
added complexity is justified. At the checkpoint, the repository was
well-framed but had not accumulated October execution comparable to BBL or
JabberVec; its latest boundary commit was August 13. That makes it a good
later model-development priority rather than a current emergency. When
reactivated, the first useful milestone is a measured baseline and one
justified comparison, not a large recommender-system feature expansion. The
project is valuable precisely because it can demonstrate experimental
discipline on a standard quantitative objective.

### Standard RNN vs. LSTM / `compare-std-rnn-w-lstm`

**Snapshot status:** PARKED / BACKLOG

**Repository:** https://github.com/bballdave025/compare-std-rnn-w-lstm

This project is a notebook-first PyTorch comparison of manually written
vanilla-RNN and LSTM recurrent cells on a manageable sample of Amazon Reviews
2023. Its educational value is explicit implementation of hidden-state
updates, gates, tensor shapes, and comparable evaluation rather than reliance
on `nn.RNN` or `nn.LSTM`. The planned dataset is roughly 10,000 reviews with
binary classification and common train/validation/test splits, but the repo
explicitly states that no cleaned dataset, trained model, or result was yet
claimed at the boundary. Several data-design decisions therefore remain real
work: rating mapping, category/quota selection, sampling seed/revision,
duplicate/missing-text handling, and split construction. The repo is a useful
learning/portfolio candidate but should not be activated merely because its
scaffold exists. If promoted later, the first milestone is to settle the
dataset contract and obtain one honest RNN/LSTM comparison result. Until then,
it belongs behind the projects that already have live research or nearly
finished artifacts.

### Pocket Cocktail Party / `pocket-cocktail-party`

**Snapshot status:** PARKED / BACKLOG; useful mentoring predecessor

**Repository:** https://github.com/bballdave025/pocket-cocktail-party

Pocket Cocktail Party explores blind source separation through a deliberately
interpretable progression from synthetic geometry-derived mixtures to messier
family recordings. The repo begins with a five-source, five-microphone
pentagon model, classical FastICA, known synthetic sources/mixing coefficients,
and recoverability metrics before moving toward real recordings with drift,
AGC, motion, and noise. It also contains an explicit ethics/consent boundary
for identifiable human recordings, including recordings involving a minor.
By the checkpoint, the mathematical/geometry framing and project skeleton were
substantive, but the README's first implementation milestones still remained
unchecked: source generation, mixing matrix, FastICA, recovery scoring, and
real-recording analysis. That makes it a valuable backlog/mentoring project,
not a claim of completed source-separation results. Its earlier scaffolding
helped shape FP↑ conventions such as runnable infrastructure plus intentional
learner work and clear failure for unfinished functions. If reactivated, the
right next step is the smallest synthetic end-to-end FastICA result, not a
jump directly to complicated real-audio modeling.

## 4. Editorial decisions for this snapshot family

These decisions were made after the first-draft linkage pass. They govern the
navigation structure; they do not move the historical snapshot date.

1. **Amazon departure/travel:** uGTgtdD keeps a short actionable consequence;
   detailed departure/benefits evidence stays in Job Hunt.
2. **Amazon Req. 10552991:** uGTgtdD keeps a concise explicit reconciliation
   block because the role closure changes canonical actionable state; Job Hunt
   retains the detailed evidence and semantics.
3. **Continuation-map topology:** this file is primarily a **one-way hub**.
   System/domain/project files do not need an all-to-all link mesh. A child
   file may link to its governing context when that materially aids
   continuation.
4. **RMMFB size:** the substantial system-level RMMFB handoff stays substantial.
   A future same-snapshot repo-level LN supplements it; it does not force the
   system handoff to become a thin pointer. Later deduplication is optional
   only when it improves navigation without demoting the project.

## 5. Scope and exclusions

This snapshot intentionally does **not** catalog every GitHub repository,
course notebook, historical idea, archived experiment, or routine life-admin
item.

Projects were included here because they were active, materially relevant to
the job/research strategy, or close enough to a concrete artifact that future
continuation would otherwise require meaningful re-derivation.

Examples intentionally not promoted into individual map entries in this pass
include older/smaller portfolio repos and unfinished coursework that were not
part of the current project-priority discussion. Their omission is not a
judgment that they have no value.

Private coursework and MOOC notebooks should not be counted as public
portfolio demonstrations merely because they exist in an authenticated GitHub
inventory.

## 6. How to extend this map

When a project gets a same-snapshot project-level LN in its own repository:

1. add the exact project-LN link to that project's entry;
2. keep the 5–10 sentence summary here short enough to remain navigational;
3. do not copy the entire project LN into this map;
4. use the project repository as technical authority;
5. use the relevant system context for cross-project priority/semantics.

The point is a checkpoint that helps Dave **resume**, not a documentation
cathedral.