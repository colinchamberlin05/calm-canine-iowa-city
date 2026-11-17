# Calm Canine Iowa City: headline A/B plan

Prepared November 17, 2026, before any response collection. The pre-November-9 deadline was missed. The repository records the true timestamp of this late prospective plan and the frozen assignments in `ab-test-assignments.csv`.

## Hypothesis and versions

B will increase YES contact intentions among simulated anxious-dog-owner visitors because its headline directly names their concern. A uses "Daycare that helps dogs settle in." B uses "A calmer first daycare visit for your anxious dog." All other visible text and design stay identical.

[A](https://colinchamberlin05.github.io/calm-canine-iowa-city/) and [B](https://colinchamberlin05.github.io/calm-canine-iowa-city/index-ab-b.html) were published November 17 at about 12:10 pm America/Chicago in [commit 0346ae8](https://github.com/colinchamberlin05/calm-canine-iowa-city/commit/0346ae899f58ec84e9bd3ede808e21f9a81ee57c). Source files and SHA-256:

- `index.html`: `b0dfa1e3895d3ccaf8885213f680ab0ac15aaa296f5cf1f64b7eca9d1f18e096`
- `index-ab-b.html`: `83f965c8922416dc9799ad348f5b5d11588750401b079a963866900f458694ae`

B is noindex, canonical to A, and absent from the sitemap. Frozen full visible-body inputs, local experiment files `page-A.txt` and `page-B.txt`, accompany the experiment data, not public page URLs. Only their H1 differs.

## Model controls

Use the verified ChatGPT web selection **GPT-5.6 Sol**, **Medium** reasoning; composer label **5.6 Medium**. Before each prompt, verify a fresh empty **Temporary** chat, **Unpersonalized** on, and no tools/files attached. The UI says Unpersonalized ignores memory, plugins, and custom instructions. Keep this configuration throughout. Backend build, temperature, top-p, and sampling seed are not exposed; do not invent them. Pause and log unavailable controls instead of switching. Save settings evidence. Internal alias changes and dependence between model responses remain limitations.

## Exact prompt

Replace only `{{PAGE_TEXT}}` with the assigned snapshot, without a version label:

> You are an Iowa City dog owner choosing daycare for an anxious adult dog that has never attended group care. You want a patient introduction and clear information before choosing a facility. Read the entire page below. This is a fictional classroom business; evaluate only whether the concept, if operating as described, would make you want to contact it. Do not browse, follow links, or contact anyone. Based only on this page, would you contact this business to ask about a first visit? Answer YES or NO on the first line, then one sentence explaining your choice. Do not assume facts not stated on the page.
>
> <PAGE>
> {{PAGE_TEXT}}
> </PAGE>

## Assignment, outcomes, and stopping

Complete 100 responses, 50 per arm, November 17-21: 20 daily, 10 A/10 B. The frozen CSV preserves five shuffled blocks using `random.Random(20261117)`; this seed assigns versions, not model outputs. Follow its sequence without regeneration. Record actual times separately. Document delays or changes in a dated amendment before further collection.

Primary outcome: first nonempty line, trimmed, matches case-insensitive YES with optional terminal punctuation (`.`, `!`, `?`) = 1; NO = 0. Other completed responses = 0, flagged malformed and retained. Never replace or regenerate completed responses. No-response technical failures have blank outcomes; log every attempt and retry the same ID/version in a fresh configured chat. Unresolved failures mean incomplete collection. Do not stop early or add trials based on outcomes.

## Analysis and evidence

After all 100 responses, compare B minus A YES proportions using two-sided Fisher exact testing, alpha .05. Positive difference and p < .05 supports this hypothesis within this model/persona only. Report counts, proportions, percentage-point difference, 95% interval, p-value, malformed responses, and failures regardless of result; non-significance does not establish equivalence.

Preserve one row per trial, exact prompts, raw outputs, timestamps, model/settings captures, attempts/errors, A/B screenshots, and publication/plan commits. Unrun observations remain blank. Keep private analytics evidence, credentials, and local computer paths out of public files. Freeze snapshots and prompt during collection. AI intentions are not human behavior, search clicks, sales, or SEO effects; generate no artificial traffic.
