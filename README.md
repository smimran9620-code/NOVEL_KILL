# Writing Novels: a portable narrative-engineering skill

A reusable skill for planning, drafting, diagnosing, and revising long-form fiction. It was built from a comparative study of two novels — one strong, one weak — and then tested on fresh tasks. It is not a template for either novel and does not imitate their voice.

## What it does

The skill gives an AI writer or editor:

- a causal model of why fiction works (five chains, ten laws, fifteen dimensions);
- a staged workflow from premise to ending;
- operational tests with thresholds, not adjectives;
- checklists for scenes, chapters, continuity, and manuscript revision;
- a catalogue of failure patterns with fixes and prevention rules;
- guard rails against the standard failure modes of AI-generated fiction;
- a working protocol that prefers diagnosis over rewriting and preserves the author's voice.

## Contents

    writing-novels/
      SKILL.md                          Main instructions: model, modes, stages, hard rules, rubric
      README.md                         This file
      LICENSE
      references/
        craft_principles.md             Why the mechanisms work; dimension table; exception list
        failure_taxonomy.md             22 failures + 4 critic failures, with signals and fixes
        comparative_analysis.md         The evidence base from the two reference novels
        scene_and_dialogue.md           Expanded scene, dialogue, action, and pacing technique
        platform_compatibility.md       Verified Claude formats; adaptation to other AI systems
      checklists/
        premise_evaluation.md           Eight-test premise gate with scoring
        scene_audit.md                  Per-scene audit and repair ladder
        chapter_review.md               Chapter-level causal and information check
        continuity_ledger.md            Living ledger templates and reconciliation protocol
        revision_audit.md               Four-level manuscript audit (scene, chapter, arc, whole)
      examples/
        weak_vs_strong.md               Ten original weak/strong contrasts with mechanism notes
      tests/
        evaluation_prompts.md           Ten fresh tests with criteria
        validation_report.md            What was actually run, results, and limits

## Quick start

**Claude Code.** Unzip into ~/.claude/skills/ so the path is ~/.claude/skills/writing-novels/SKILL.md.

**claude.ai.** Zip the writing-novels folder (the ZIP must contain the folder, not loose files) and upload it through Settings > Features. Requires a plan with code execution enabled.

**Claude API.** Upload the bundle with POST /v1/skills, then pass the returned skill_id in the container parameter with type "custom", alongside the code execution tool.

**Other systems.** Paste SKILL.md as a standing instruction and attach the reference files the task needs. See references/platform_compatibility.md for a table of adaptations and a condensed single-document mode.

## How to use it

The skill triggers on requests to plan, draft, critique, revise, or audit fiction. It runs in one of four modes: PLAN, DRAFT, DIAGNOSE, REVISE. It will say which mode it is in.

Useful requests:

- "Stress-test this premise before I outline." (premise gate)
- "Build a five-chapter grid where each chapter is caused by the last." (architecture)
- "Diagnose this scene; do not rewrite it." (scene audit)
- "Audit continuity across these chapters." (ledger)
- "Does this ending answer the question the book asked?" (ending contract)
- "My draft feels flat. Find the level where the problem starts." (revision ladder)

## Design decisions

- **Mechanism first.** Every rule names the reader effect it produces, so the model can reason when the rule does not apply.
- **Tests over adjectives.** "Does the next scene become impossible without this one?" is usable; "make it compelling" is not.
- **Minimal intervention.** Diagnosis precedes rewriting; the smallest change at the right level is preferred.
- **Voice preservation.** The skill includes a style-preservation test and a rule against imposing literary uniformity on genre fiction.
- **Honest limits.** The comparative evidence is two translated serials; the validation is small and uses AI judges. Both are reported, not hidden.

## Evidence and validation

The comparative study read the full 2,334-chapter reference novel through a programmatic pass over every chapter plus more than fifty full chapter reads across all arcs, and read the 50-chapter failure reference in full. Findings, quotations, and chapter citations are in references/comparative_analysis.md.

Validation used seven fresh tasks (not derived from the reference novels), each run with and without the skill, and scored blind against fixed criteria by a judge that did not know which output was which. Results, including where the skill did not help or hurt, are in tests/validation_report.md.

## Limitations

- Automatic triggering depends on the host platform and the request's wording.
- The skill cannot check facts about a manuscript it has not been given.
- Two reference texts cannot establish general laws of literature; the laws are well-supported hypotheses.
- The tests are small-sample and AI-judged; they show direction, not statistical proof.
- The skill is a craft instrument, not a taste substitute. Content boundaries, register, and genre conventions remain the author's decisions.

## Future improvements (after real use)

1. **Human validation.** Blind rating by editors, with agreement scores, on paired outputs; the current judges are AI.
2. **Long-form test.** Plan and draft three consecutive chapters (6,000+ words) with and without the skill, measuring causal-link density, scene-type variety, continuity errors, and repetition.
3. **Revision-at-scale test.** A real 3,000-word chapter with planted faults; measure detection recall, false positives, and voice preservation.
4. **Genre packs.** Optional reference files for romance, mystery, horror, and literary fiction, each with genre-specific promise, pacing, and payoff conventions.
5. **Continuity tooling.** A small script that parses a ledger and flags new chapters against it, replacing the manual table pass.
6. **Cost measurement.** Tokens and time per task, so users can decide when the process overhead is worth it.
7. **Cross-model tests.** Different model families as writer and judge; the current evidence is single-family.

## Customising

- Add genre-specific rules as a new file under references/ and link it from the SKILL.md reference map.
- Tighten the rubric thresholds in SKILL.md if you are using the skill for professional editing.
- Replace the examples with your own; the mechanisms matter, not the sample sentences.
- Keep SKILL.md under 500 lines. Move detail into references/.

## License

MIT. The analysis summarises and briefly quotes two published works for criticism; no substantial portions are reproduced. The illustrative examples are original.

## Credits

Created by Imran. Licensed under the MIT License (see LICENSE).
