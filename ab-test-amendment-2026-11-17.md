# Headline experiment amendment - November 17, 2026

This amendment is recorded after trial 001 and before trial 002. It changes model controls, the fixed sample size, and trial 001's primary-analysis eligibility. The hypothesis, persona, exact prompt, frozen page text, outcome rules, and analysis method remain unchanged from [the original plan, commit a16333b](https://github.com/colinchamberlin05/calm-canine-iowa-city/commit/a16333b569c54a1fec73f2b3c7366f4f27f290aa). The [site source, commit 0346ae8](https://github.com/colinchamberlin05/calm-canine-iowa-city/commit/0346ae899f58ec84e9bd3ede808e21f9a81ee57c), is unchanged. Further collection begins only after this amendment and amended assignments are committed. The original November 9 deadline remains missed.

## Why the protocol changed

Trial 001 received B and answered YES. Its fresh Temporary, Unpersonalized chat displayed GPT-5.6 Sol / 5.6 Medium before submission, but the model selector showed GPT-6 after the response. The visible evidence does not establish the backend model that produced the answer. Preserve the completed response, exact prompt, screenshots, and model-check trace without regeneration or replacement.

Exclude 001 from the primary analysis because the selected model was not consistent before and after the response, not because its answer was YES. This quality-control decision was made after one outcome was known. The amended experiment is therefore not a wholly preregistered new study, and 001 is not retroactively relabeled a pilot. Report that limitation and include the response in the full-data sensitivity analysis.

## Model controls for remaining trials

Use the web interface's default selection **GPT-6**, **Medium**. Start every trial in a new empty Temporary chat with Unpersonalized on and no attached tools or files. Verify and capture the selected GPT-6 label and Medium setting both before submission and after the completed response. Describe passing records as **UI-consistent**, not backend-model-verified. Backend build, temperature, top-p, and sampling seed remain unexposed. Keep the original no-browsing, no-links, and no-contact instructions.

Any further mismatch requires a pause and dated issue log before further collection. Do not automatically exclude or replace that completed response, add trials, or switch models. Resolve the issue explicitly before resuming.

## Fixed assignments and analyses

Keep original assignments 001-100 unchanged. Append 101 = B and 102 = A to November 21, batch 5, making 22 scheduled that day and **102 total, 51 per arm**. Before trial 002, one Python `SystemRandom` shuffle of one A and one B produced B, A at **2026-11-17T18:48:51.132034+00:00**. This was an unseeded system-random draw, not a retrospectively chosen seed.

If trials 002-102 all pass the UI checks, the primary dataset will contain **101 responses: 51 A and 50 B**, excluding 001 only. Also report the original outcome comparison using all 102 completed responses, **51 A and 51 B**, labeled **model-mixed sensitivity analysis** (potentially mixed, because 001's actual model is unresolved). Use the original two-sided Fisher exact test, alpha .05, and report counts, proportions, B-minus-A difference, uncertainty, malformed responses, and errors for both datasets.

Stop after ID 102 regardless of the results. Do not run interim outcome comparisons, increase the sample, or regenerate completed responses. Unrun observations stay blank. No-response technical failures may be retried under the same ID with every attempt logged. An unresolved failure or model-control issue must be reported, not presented as a completed clean experiment. These remain simulated AI intentions, not human conversion or SEO evidence.
