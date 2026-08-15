## RMMFB — résumé / interview bullet candidates from dataset-method reconstruction

- Designed and curated a domain-specific computer-vision research dataset of 3,331 historical-document images, including a custom annotation ontology for multiple manuscript-reuse structures and difficult negative/fake-out cases.

- Built scripted dataset-integrity and QA checks in Bash/Linux, including filename-schema validation, duplicate underlying-image detection, label-consistency checks, and verification that classified examples were removed from unclassified candidate pools.

- Developed provenance-preserving filename conventions that encoded source institution, collection/manuscript identifiers, image identifiers, and classification metadata to support reproducibility, citation, and later source recovery.

- Designed an intentionally enriched sampling procedure for large FamilySearch collections, combining geographic/catalog surveys, age-weighted candidate selection, randomized selection within the enriched frame, and documented human-review procedures.

- Created human-in-the-loop acquisition workflows and detailed collection instructions enabling collaborators to gather consistently selected binding images while preserving DGS/source identifiers and provenance.

- Built reproducible preprocessing plans for the same 3,331-image corpus at original resolution plus 128, 224, 448, 896, and 1792 px, supporting controlled experiments on the effect of resolution on detection of small visual features.

- Constructed and reconciled large candidate-image inventories from heterogeneous digital-library sources; recovered a deduplicated pre-e-codices in-the-wild corpus of 41,790 distinct candidate images from multiple historical collection snapshots.

- Developed repository-specific acquisition tooling for heterogeneous digital-library systems, including IIIF and export-based sources, with explicit request throttling and source-aware naming/provenance preservation.

- Iteratively simplified a detailed annotation/classification system into practical human-facing decision aids while retaining the scientifically important distinctions—an example of translating a research ontology into an operational labeling workflow.

- Treated annotation uncertainty explicitly rather than forcing artificial ground truth, including dedicated uncertain, fake-out, and counterexample handling and deliberate collapse of distinctions that could not be annotated reliably.

### Particularly useful interview themes

**Dataset engineering:** this was not “download images and label them”; it included sampling design, acquisition, provenance, ontology design, human annotation procedures, QA, deduplication, preprocessing, and experimental-readiness checks.

**Research judgment:** repeatedly narrowed overly elaborate systems to operational versions, froze a good-enough dataset rather than indefinitely polishing it, and documented known limitations instead of disguising them.

**Human-in-the-loop ML:** designed both the ontology and the procedures/tools through which other humans could apply it consistently.

**Linux/data tooling:** substantial shell-based inspection and QA over large image collections, including `find`, `grep`, `sed`, `awk`, `comm`, generated manifests, and reproducible audit logs.

**Open-science / provenance thinking:** preserved enough source identity to reconstruct citation and permissions while recognizing that release of the full reconstruction key should be an intentional publication/IP decision.
