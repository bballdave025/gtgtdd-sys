# RMMFB Project Retrospective: How the Work Actually Developed

This is a coherent journal-style reconstruction of what the surviving project materials show about how RMMFB developed: what I was trying to accomplish, what methods I built, what I simplified, what I checked, and where the project trajectory actually went.

One of the reassuring things about reconstructing the project from scattered notes, shell logs, diagrams, Google Docs, spreadsheets, classification helpers, and directory snapshots is that the overall trajectory is visible even when no single document tells the whole story. The pieces show a consistent pattern: I identified a real retrieval problem, built increasingly serious data infrastructure around it, repeatedly overbuilt some parts, then simplified them when necessary, and eventually created something that could support actual experiments rather than remaining an indefinitely expanding collection project.

## The central research problem stayed recognizable

The original motivation was practical and domain-driven: reused manuscript material appears in historical bindings and related documentary contexts, but the relevant evidence is distributed across enormous digitized collections. Human experts cannot inspect everything manually. The project therefore became a machine-learning retrieval problem: identify images worth human inspection while preserving enough interpretability and provenance that discoveries could be examined, cited, and eventually published.

As the project matured, the goal became more specific. The useful operating point is not generic “high accuracy.” The system is meant to favor **high recall**, accepting reduced precision because missed manuscript-reuse candidates are more costly than sending additional false positives to human review. This is also why the difficult negative or “fake-out” cases matter so much: they help define what a useful retrieval system must learn to distinguish without suppressing real positives.

The long-term vision is substantially larger than the MVP paper. It includes very large-scale retrieval, more principled treatment of fake-outs, eventual integration with NTEC-style signal-existence reasoning, and richer expert interpretation. But those later goals do not have to be completed before the first defensible RMMFB paper exists.

## The dataset became the real research asset

The 3,331-image dataset was not created by simply gathering a convenient folder of positives and negatives. It emerged from a long process of searching, source discovery, acquisition, classification, relabeling, ontology development, and deliberate stopping.

The surviving project notes show an important turning point: I explicitly recognized that continuing to improve the dataset indefinitely would prevent publication. The pseudo-deadline documents contain language such as “dataset is as it will be used – No fixing!!” and later allow remaining contradictions to be treated as “Good Enough.” That shows an explicit shift from collection perfectionism toward experimental readiness.

The final dataset plan also became structurally ambitious. The same 3,331 images were intended to support eight individual yes/no classification tasks corresponding to specific reuse classes, a broader reuse/no-reuse task, original-resolution data, resized versions at 128, 224, 448, 896, and 1792 pixels, and stratified splitting for model development and evaluation.

This multi-resolution design was tied to a scientific concern: small but important visual features can disappear when full document images are aggressively resized. That concern later became especially relevant to the planned comparison between ordinary ResNet-scale inputs and higher-resolution architectures.

## The ontology was built, then repeatedly simplified until it became usable

The classification system went through a recognizable cathedral-to-lean-to cycle.

At one stage I built a fairly elaborate HTML/XML classification environment. That implementation was eventually abandoned, but the underlying ontology survived and was distilled into smaller tools: compact classification helpers, printable decision sheets, and the `1-or-2-pg` class descriptions that now function as the mature operational version.

This simplification did not mean abandoning rigor. The shorter documents still preserve class definitions, boundary conditions between similar categories, positive and negative examples, specific visual decision rules, multi-label handling, explicit uncertainty categories, fake-outs and important counterexamples, and deliberate collapsing of distinctions that I did not believe I could classify reliably.

That last point is methodologically important. Instead of pretending that a detailed taxonomy automatically implied reliable ground truth, I reduced some distinctions when my own expertise was not strong enough to support them. That is better science than forcing false precision into the labels.

The ontology work also shows a human-centered design skill that is easy to overlook. There was a difference between the full conceptual ontology and the interface that a person could actually use while labeling hundreds or thousands of images. The project repeatedly moved toward the latter without throwing away the scientifically important structure.

## Human-in-the-loop collection became a reproducible process

The FamilySearch portion of the project is especially revealing because the surviving documents show not just image collection, but an operational workflow for other people.

The process included identifying candidate collections, constructing survey and summary sheets, locating DGS/film identifiers, recording catalog and collection metadata, selecting films for inspection, tracking work status, generating direct FamilySearch film URLs, preserving DGS identifiers while browsing, saving a consistent set of binding/front-matter images, and renaming files immediately using provenance-rich conventions.

The helper instructions are unusually concrete. They explain how to choose the next DGS, mark it as in progress, preserve the displayed DGS rather than waypoint metadata, save the cover plus several opening images and a final image when identifiable, and tolerate uncertain extra images rather than turning acquisition into another perfectionist bottleneck.

That means the dataset was not merely “manually collected.” A reproducible human acquisition protocol was designed around it.

## The FamilySearch sampling was intentionally biased, but not arbitrary

The surviving sampling documents show a method that can reasonably be described as **targeted enrichment with randomized selection within the enriched candidate frame**.

Older materials were intentionally oversampled because earlier records were more likely to contain manuscript reuse. Different starting centuries were given different numbers of opportunities in the sampling frame, and randomized selections were then drawn from the combined candidate pool. Geographic and catalog surveys were also used to broaden the source population.

The process was not pristine statistical sampling, and the documents do not pretend otherwise. They record incomplete surveys, pragmatic cutoffs, tactical changes, and places where I stopped gathering more because continued sampling had diminishing value.

That honesty is a strength. The dataset was designed to be useful for finding a rare historical phenomenon, not to claim that it was a uniformly random sample of all digitized historical books.

## Provenance was built into the file system

The information-dense filenames were not just a personal naming quirk. They became a lightweight metadata system.

A filename could encode source institution, manuscript or collection identifier, DGS or digital-object identifier, image number, folio/page information where available, and classification labels or annotation state.

That made the files easier to trace back to their original sources and preserved information that would later matter for citation, permissions, and provenance reconstruction.

The same feature creates an intellectual-property consideration: a complete list of these filenames can serve as a reconstruction key for a dataset that took years to assemble. Open-science release therefore needs to be deliberate rather than accidental. The project can ultimately be transparent while still distinguishing between private provenance records, reviewer/collaborator material, and intentionally released public data.

## The acquisition scripts show source-aware engineering rather than one generic scraper

Different repositories required different acquisition strategies.

The surviving shell scripts include, for example, IIIF image retrieval and repository-specific export downloads. These scripts interleave individual `wget` requests with substantial `sleep` intervals.

That does not by itself prove compliance with every institution’s terms of use, but it does show that the collection tooling was designed with deliberate throttling rather than maximum-speed scraping.

The broader pattern is more important than any one script: the project adapted to heterogeneous digital-library systems while trying to preserve source identity and avoid unnecessary load on remote services.

## The QA work was more serious than I remembered

The shell logs show that the dataset was not simply classified and trusted.

One surviving audit begins with 869 classified JPEGs and then performs filename-pattern checks, manual exception review, stripping of classification suffixes, and duplicate underlying-image detection.

The logic matters:

1. Count all classified image files.
2. Check whether filenames match the expected annotation schema.
3. Separate exceptions for manual inspection.
4. Remove classification suffixes to recover the underlying image identity.
5. Search for the same underlying image appearing in more than one classification location.
6. Investigate and correct genuine duplicates.
7. Recount and verify the cleaned result.

A later stage in the same audit checks another invariant: images that had already been classified should not remain in the unclassified input pool. The logs compare input and output identities, generate a removal list, remove overlaps, and check for failures.

This is strong dataset-engineering evidence because the checks were not only conceptual. They were implemented with shell tooling and left behind reproducible logs.

The tools used include ordinary but powerful Unix building blocks such as `find`, `grep`, `sed`, `awk`, `comm`, `wc`, generated `.lst` files, directory-tree snapshots, Bash loops, and timestamped audit artifacts.

The important skill is not memorizing those commands. It is using composable shell tools to state and test data invariants.

## The in-the-wild collection was already much larger than the labeled dataset

The five surviving `p2_*` directory listings contain 24,893, 2,172, 16,781, 20, and 18 images. Those lists overlap. After deduplication they produce 41,790 distinct candidate images.

A separate file named `sorted_uniq_list_of_all_pre_ecod_-_from_2024.txt` also contains 41,790 entries and corresponds effectively to the deduplicated union of those five directories, aside from a superficial filename-encoding difference involving an accented character.

This means the project already had a substantial in-the-wild corpus long before the eventual 100k-plus vision was complete.

That is important for both the paper history and the career story. The labeled 3,331 images are the curated experimental core, but they sit inside a much larger search-and-retrieval program.

## The project repeatedly moved between cathedral and lean-to

One of the clearest project-level patterns is not technical but behavioral.

I repeatedly built systems larger than were strictly necessary: a rich HTML classification environment, large directory structures, elaborate multi-resolution plans, multiple sampling frameworks, large-scale acquisition machinery, and increasingly detailed classification documentation.

But I also repeatedly recognized when those structures were blocking forward motion and simplified them.

The HTML classifier gave way to short printable instructions. Overly fine ontology distinctions were collapsed when I could not support them reliably. The 3,331 dataset was explicitly frozen instead of continually perfected. The experiment plan began moving from “everything scientifically interesting” toward a smaller set of models that can answer one publishable question.

That pattern is important because the project did not fail merely because it sometimes became too large. The trajectory shows repeated recovery.

The useful design principle now has a name:

> **Ruthlessly MVP RMMFB**

The criterion is not maximum RMMFB. It is the minimum defensible paper that answers an interesting question using the unusually valuable groundwork already completed.

## The work already demonstrates several applied-science skills

Seen as one coherent project, RMMFB shows more than “I trained a classifier.”

It demonstrates problem formulation from a real domain need; interdisciplinary research across ML, digital humanities, manuscript studies, and digital libraries; ontology design; dataset curation; sampling design; human-in-the-loop workflow design; provenance engineering; heterogeneous data acquisition; shell-based QA and data validation; handling of annotation uncertainty; multi-resolution experimental design; interpretability planning; large-corpus retrieval thinking; explicit management of asymmetric error costs; and willingness to document limitations rather than manufacture certainty.

This is why reconstructing the scattered evidence has felt surprisingly affirming. The skills I believed I was using are visible in the artifacts. The project did not merely contain ambitious intentions; many of those intentions became actual procedures, scripts, checks, datasets, and decision rules.

## The storyline, in one arc

The project began with a domain observation: manuscript reuse was visible in digitized historical bindings, but the scale of the collections made systematic human discovery impossible.

I turned that observation into a computer-vision retrieval problem.

I first built a modest labeled dataset and classifier, then discovered that the real difficulty was broader: the phenomenon had multiple visual forms, important evidence could be tiny, some negative examples were extremely convincing, and source provenance mattered if discoveries were ever going to be useful to scholars.

The project therefore expanded into ontology design, large-scale source discovery, dataset engineering, provenance-aware acquisition, and classification infrastructure.

Some of that infrastructure became too elaborate.

I simplified it.

The ontology became operational instead of encyclopedic. Human workflows became explicit. Sampling became documented. Acquisition was throttled and source-aware. File naming preserved provenance. Shell audits tested dataset invariants. The curated dataset was frozen at 3,331 images instead of being allowed to grow forever. A 41,790-image deduplicated in-the-wild candidate corpus survived as evidence of the larger retrieval program. Multi-resolution versions were planned to test the scientific concern that ordinary resizing may erase small but important features.

The project is therefore no longer waiting for a perfect dataset or perfect conceptual architecture.

The remaining question is much narrower:

**What is the smallest defensible experiment that turns this unusually rich groundwork into a publishable RMMFB result?**

That is where the project is now.
