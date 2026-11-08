# Research Atlas writing and research contract

Version 1.0. Use this contract for original Research Atlas prose, whether the author is a person or an agent. Read it before editing the Obsidian vault or its future Git repository. Its writing rules take precedence over templates, editor defaults and model defaults. Preserve required formats, source accuracy and necessary safety information.

## Authority and scope

The canonical file is `STYLE.md` at the Research Atlas vault root. Do not create competing style contracts elsewhere in the vault. Existing instructions in project or agent files remain applicable to operations and permissions. If an instruction conflicts with this contract, preserve the source material and technical correctness, leave the conflicting change unresolved and report the conflict rather than silently choosing a weaker requirement.

Apply this contract to paper notes, literature indexes, reading queues, research questions, seminar material, survey drafts, experiment plans and reports, research-state files, README files, exercise solutions, technical notes, presentation prose, agent traces and comments in scripts or code. It governs text authored for the vault, not the exact wording of imported papers, quotations, source code, logs, bibliographic titles, required citation styles or machine-readable formats.

Research Atlas is a general research library, not a repository dedicated to RowHammer, hardware security or any single seminar. Do not turn a local project's conventions into global taxonomy or assume that a paper's presence in one direction makes that direction the paper's only possible use.

## Repository and editing authority

The repository owner alone reviews, stages, commits, amends, pushes, merges, rebases, resets, rewrites history, opens pull requests and decides what is published. Agents must not run `git add`, `git commit`, `git push`, `git reset`, `git rebase`, `git merge` or equivalent mutating Git operations, even as part of an otherwise authorized documentation task. They may inspect local Git status or diffs when authorized, edit the explicitly requested working-tree files and report changes for owner review. They may print suggested commands for the owner without executing them.

Do not create branches, publish research notes, upload vault contents or modify remote services without explicit authorization. Treat unpublished research notes, drafts and personal annotations as private by default. Check for credentials, private contact information, unpublished results and locally cached source material before recommending publication.

Research Atlas currently lives in iCloud Drive. Use the actual mounted vault path rather than a guessed path. Avoid competing writes to files that are open or concurrently being edited, and inspect the current content immediately before changing it. Do not treat an iCloud placeholder or failed file read as an empty note.

Preserve user-authored interpretations, annotations and unfinished questions. Do not replace a developed note with an abstract summary, silently normalize the author's conclusions or overwrite a file merely because a generated version is cleaner. Additions should be scoped, inspectable and reversible.

## Register by document type

A paper record identifies the source, what has actually been checked, the mechanism or claim established by the inspected material, and why the paper belongs in its collection. A reading note captures the reader's reasoning, uncertainty, objections and connections to other work without presenting those annotations as the paper authors' claims.

A literature index supports navigation and comparison. Keep entries short, factual and linked to their paper records. Do not repeat full abstracts or create a second independent set of technical claims in index files.

A research-direction note records questions, scope boundaries, hypotheses, selected literature and decisions that can change. A seminar note distinguishes the course deliverables and selection rationale from the broader Research Atlas bibliography. A survey draft compares evidence across papers rather than listing paper summaries in sequence; do not announce a synthesis as established until the cited results support it.

An experiment plan identifies the hypothesis or observation being tested, setup, variables, baselines, measurements, expected controls and conditions that would make the result inconclusive. An experiment report separates configuration, executed procedure, observed results, interpretation, limitations and reproducibility information. A proposed experiment is not a completed result.

An agent trace reports the exact files changed, the reason for each meaningful change, the checks actually performed and unresolved questions. It must not invent review, tests, source inspection, approval or publication.

## Vault organization and navigation

Follow the vault's existing directories, filenames, note properties, templates and link conventions before creating new structures. The current layout includes `directions/`, `assets/`, `templates/`, `exercises/`, `sources/`, `reading-queue` and research indexes or state notes. A research direction may contain a `papers/` collection and a seminar may have its own `seminar/papers/` collection. These are organizational locations, not universal requirements for every future direction.

For example, `directions/dependable-computing/papers/` is a broader literature collection, while `directions/dependable-computing/seminar/papers/` is a course-specific selection. A paper referenced from both places may have a general record and a seminar-specific note or link according to the established layout. Do not silently create divergent bibliographic facts or duplicate long analyses. Keep shared metadata consistent and place the seminar selection rationale in the seminar context.

Inspect adjacent notes and the relevant `index.md` before assigning IDs, slugs, properties or links. Preserve stable note IDs and filenames unless a rename was specifically requested. Prefer existing paths over introducing new category names. A title change in a publication is not sufficient reason to break inbound links.

Use Obsidian wikilinks or Markdown links according to the convention already used by that collection. Disambiguate identical basenames when needed. After adding, moving or renaming a note, update the affected indexes and resolvable internal links. Do not claim a link is valid until its target has been checked. Assets should be referenced from their existing location rather than copied into arbitrary paper folders.

Avoid turning tags into an uncontrolled second hierarchy. Use existing property names and topic values consistently. A tag, backlink or folder membership does not establish that a paper has been read or verified.

## Bibliographic accuracy and source handling

Use the primary source when available: publisher proceedings, authors' paper, arXiv record, official artifact page or code repository. Record the exact source and version actually inspected. Search results, personal notes, discussions and generated summaries can guide discovery, but must not be treated as equivalent to checking the original paper.

Preserve verified title, author order, year, venue, DOI, arXiv identifier, URL and revision accurately. An arXiv posting date is not necessarily the conference publication date. An arXiv identifier is not a publisher DOI; use `10.48550/arXiv...` only when that is the actual DOI being recorded. Do not invent a venue, a PDF URL, author affiliations, artifacts or a publication status from the title alone.

When a paper has multiple revisions, identify which version supports a claim. An erratum, corrected table or revised evaluation takes precedence for current numerical reporting, while historical figures remain identifiable as superseded results. Do not merge numbers from incompatible versions into one result. If a source has not been opened or a link has not been verified, mark that fact `UNVERIFIED` or leave the unsupported field unset according to the note schema.

Distinguish the published paper, its supplementary material, its artifact, the artifact instructions and independent reproductions. A repository's existence is not proof that it builds, reproduces a figure or supports all stated hardware. An author's estimate of runtime, resources or setup effort is an estimate under the author's conditions.

Preserve citations and quotations exactly, including source titles whose capitalization or typography differs from this style contract. Quote only what is necessary, attribute it and link the supporting source. Do not import full copyrighted papers into the vault unless the user has an appropriate right to store them.

## Paper records and selection rationale

Before writing a paper note, inspect the collection's existing metadata schema. Reuse established fields such as `id`, `title`, `authors`, `year`, `venue`, `doi`, `source`, `status`, `topics`, `added`, `source_checked` and `read_version` if present. Do not replace the schema with a preferred template or populate an unknown value with plausible text.

A useful paper record, to the extent supported by the material actually read, identifies the source, bibliographic metadata, research problem, mechanism, evaluation method, principal results, limitations and open questions. Include the reason the paper was selected for a direction or seminar when that context exists. Do not add empty headings solely to make the note look complete.

Write selection reasons as concrete bullet points tied to the research question: a mechanism the paper clarifies, a prior result it challenges, an evaluation method it adds, a comparison it enables or a limitation it exposes. Avoid reasons based only on venue prestige, recency, an impressive number or the presence of AI terminology. Distinguish core reading, background citation and optional reading without promoting an item to core status automatically.

A catalogue entry based only on an abstract must say that the abstract establishes the claim. Do not present it as a full-paper review, and do not advance the reading status to `read` or `verified` unless that state is actually supported. Preserve existing status values and definitions rather than inventing a new status taxonomy.

If the paper contains an attack, separate the physical or logical fault mechanism, the targeted component, the attacker's capabilities, the measured outcome and the proposed defenses. A compiler, model or GPU application can be a victim without being the fault-generation mechanism. Keep threat-model prerequisites next to security results.

## Evidence and scientific claims

Separate author-reported results from independently observed results and the vault author's own deductions. Distinguish real hardware measurements, simulations, formal analysis, synthetic fault injection, software-only emulation, analytical estimates and end-to-end demonstrations. These forms of evidence answer different questions and must not be described interchangeably.

Every numerical claim with methodological significance should retain its unit, baseline, experimental conditions, sample or workload scope, and source. For performance comparisons, identify what was measured and under which configuration. An evaluation of DRAM timing-parameter changes on a real machine is not automatically an evaluation of a full mitigation mechanism with tracking, alerts and refresh control.

Do not infer a universal security guarantee from a finite test, a single DRAM generation, one GPU, a model configuration or a bounded proof. Distinguish a specified hardware guarantee from broader expectations assigned to a deployed system. If an attack works only with co-resident code execution, physical access, a particular model representation or a given memory type, retain that condition wherever the result is summarized.

Treat independent discovery, citation patterns and apparent gaps as hypotheses until the relevant evidence has been checked. Do not infer that research communities are disconnected, that a defense always fails or that no previous paper exists from a short literature search. Mark a comparison as incomplete when papers use different baselines, threat models or metrics.

Record uncertainty close to the affected statement. Use `TBD`, `UNVERIFIED`, `NOT_TESTED` or `INCONCLUSIVE` where appropriate, and say which source inspection or experiment would resolve it. Do not use a limitations paragraph at the end to repair an unsupported assertion earlier in the note.

## Experiments, artifacts and reproducibility

An experiment note should record the exact paper revision or artifact release, environment, dependencies, commands, parameters, seeds, input data, baseline, output files and observable results where those details are known and needed. Capture the original source for datasets and benchmarks. Keep local machine capabilities separate from hardware requirements reported by the paper authors.

Distinguish reproduced, partially reproduced and not reproduced results. A successful installation does not establish that an attack, mitigation or benchmark was reproduced. Never claim that an artifact has been built, simulated, tested or validated unless the corresponding command was executed and its result inspected.

Keep the scope of each experiment tied to the stated research question and available hardware. Do not invent extensions or claim novelty for a parameter sweep, comparison or artifact already present in the source publication. An experiment may be a valid seminar demonstration without constituting an original research contribution.

Preserve raw logs and measurements. Generated plots must identify their data source, units, legend and relevant experimental conditions. Avoid combining simulated and hardware measurements on one axis without explicitly indicating the difference. Store large generated datasets or copyrighted source material only according to the repository's publication and storage policy.

## Register and sentence construction

Write technical prose with concrete subjects, mechanisms, conditions and observable consequences. Prefer active voice unless the actor is unknown or irrelevant. Explain a design choice through the constraints, uncertainty or alternative that motivated it, not through promotional language.

Use one idea per paragraph and one responsibility per section. Paragraphs normally develop an idea in several sentences, but a short definition, warning, caption or annotation may be shorter. Do not add filler to satisfy a sentence count. Preserve necessary qualifiers even when they make a sentence less smooth.

Begin with the fact, question, result, mechanism or decision being documented. Do not open with praise, acknowledgement, a restatement of the request or a description of what the document is about to do. Do not close with a motivational summary, a generic future-work section or an abstract statement about the importance of research.

Use sentence case for headings. Preserve the capitalization of publication titles, proper names, acronyms, identifiers, filenames and quoted sources. Use the project's chosen language for each note or collection; do not silently translate existing notes. Keep established technical terminology in its conventional form.

Do not use em dashes, en dashes, prose arrows, emoji, hashtags, decorative dividers, title-case headings, rhetorical headings, arbitrary bold emphasis or rhythmic standalone sentences in original prose. Exact titles, quotations, citations, commands, technical notation and imported material are exempt when rewriting them would damage fidelity.

Avoid promotional or stock AI expressions, including `delve`, `leverage`, `harness`, `unlock`, `seamless`, `powerful`, `elegant`, `cutting-edge`, `groundbreaking`, `game-changer`, `landscape`, `journey`, `deep dive`, `showcase`, `in essence`, `ultimately`, `moreover`, `furthermore`, `notably`, `importantly`, `it is worth noting`, `the key insight` and `why this matters`. Do not replace them with equally vague synonyms. State the mechanism, observation or limitation instead.

Avoid `Not just X, but Y`, `X isn't about A. It's about B.`, repeated bold-label-and-colon bullets, chained definitions, participial introductions and structural signposts such as `In the following section`. Use semicolons sparingly. Prefer short causal links to rhetorical transitions. Do not add an abstract or executive summary unless the requested publication format requires one.

Use bullets for independent points and ordered lists for real sequences or intentionally numbered references. Use a table only when multiple rows share meaningful attributes, such as papers compared by evidence type, workload, metric and limitations. Do not use a table to disguise ordinary prose. Headings should mark actual conceptual boundaries, not every few sentences.

## Markdown source and line layout

MOST IMPORTANTLY, WRITE EVERY AUTHORED PROSE PARAGRAPH ON ONE PHYSICAL SOURCE LINE. DO NOT HARD-WRAP PARAGRAPHS AT 80, 100, 120 OR ANY OTHER COLUMN WIDTH. This applies to Obsidian notes, Markdown documents, agent traces, research reports, technical comments and prose in scripts. Long source lines are acceptable. Editor soft wrapping is not a source newline.

Use blank lines between Markdown paragraphs. Headings, individual list items, table rows and fenced-code delimiters occupy their own lines according to Markdown syntax. Keep an individual prose list item on one source line unless valid syntax requires otherwise. Do not collapse code, YAML frontmatter, mathematical notation, citation records or required indentation to meet the prose rule.

Preserve Obsidian properties, YAML syntax, wiki links, code fences, LaTeX expressions, footnotes, callouts and embedded media when an edit concerns surrounding prose. Do not convert existing note syntax merely for stylistic consistency. A required publication template, accessibility need or machine parser takes priority where a conflict would make the artifact invalid.

Keep source-code and script comments on one physical line per prose paragraph. Multiple comment lines are permitted for distinct logical items, parameter schemas or line-specific annotations, not for artificial line-length wrapping. Do not reformat verbatim evidence, copied errors, third-party code or license notices.

## Modification reports and review

Before editing, inspect the target file, adjacent exemplars, relevant index and applicable local instructions. When a source is unavailable, do not fill gaps with inferred metadata or switch to a secondary source without marking the change in evidence quality. Avoid unrelated cleanup, directory restructuring or mass renaming during a bounded paper-cataloguing task.

After editing, report the exact created or modified paths, significant decisions, sources actually checked, internal links validated, and any checks that were not run. If files were not opened or tests were not executed, say so explicitly. Do not claim a Git commit, approval or repository publication occurred.

Before delivery, check technical qualifications, bibliographic consistency, exact identifiers, dates, supported numerical values, reading-status honesty and the separation of evidence from interpretation. Check that each authored paragraph occupies one physical source line and that original prose follows the typography and register rules. Stop when the requested work ends.
