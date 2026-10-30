---
name: writing-novels
description: Plan, draft, diagnose, and revise long-form fiction as a causal system. Use when the user asks to outline a novel or story arc, draft or continue a chapter or scene, critique a draft, test whether a plot is believable, audit continuity, integrate theme, or evaluate an ending. Also use when a premise needs stress-testing before drafting, or when a manuscript must be revised without flattening the author's voice.
license: MIT
---

# Writing Novels

A workflow for planning, drafting, diagnosing, and revising long-form fiction. It treats narrative as a causal system: events produce consequences, choices produce character, rules produce costs, and endings pay for promises. Use the stages that match the request. Do not run the whole pipeline when the user asked one question.

## Scope

Use for: premise development; arc and chapter planning; scene and chapter drafting; critique and diagnosis; revision; continuity audit; ending evaluation; thematic integration; brief line-level work.

Do not use for: non-fiction argument, poetry as the primary form, screenplay formatting standards, or tasks where the user only wants a summary of existing text. Those can borrow individual tests but not the pipeline.

## The model in one page

Reader experience is produced by five causal chains. If a passage sits outside all five, it is texture at best and filler at worst.

1. **Desire -> obstacle -> choice -> consequence.** A character wants something specific, something specific blocks it, the character chooses under pressure, and the consequence changes the terms of the next choice. This is the scene engine.
2. **Constraint -> cost -> strategy.** A rule matters only if obeying or breaking it costs something measurable. Systems generate plot when they constrain, not when they decorate.
3. **Expectation -> delay -> fulfillment, complication, or overturn.** Setups create expectations; the text must eventually pay, complicate, or deliberately invert them. Unpaid setups read as authorial negligence.
4. **Information asymmetry -> inference -> surprise that feels inevitable.** The reader should be able to reconstruct, after the fact, why the outcome followed from what was shown, even if they did not predict it.
5. **State change per unit of text.** Every scene and chapter must leave something different: knowledge, relationship, stakes, possession, position, or self-understanding. If the end state equals the start state, the unit is a report, not a story.

Mechanism rule: when you claim something works or fails, name the mechanism ("the reader cannot evaluate the victory because the cost was never shown"). Do not label prose "strong" or "weak" without a cause.

## Modes

Choose one mode per request and say which you are in, in one line.

- **PLAN.** The user wants architecture. Default output: no prose. Produce causal spine, arc ladder, character constraints, world constraints, setup/payoff register, risk list.
- **DRAFT.** The user wants prose. Default: dramatize the decisive moments, summarize only transitions, do not pad to a word count.
- **DIAGNOSE.** The user wants to know what is wrong. Default: evidence first, severity ranked, no rewriting unless asked.
- **REVISE.** The user wants fixes. Default: minimal intervention, fix the cause rather than the symptom, show a sample before applying changes across a long manuscript.

Do not blend modes silently. If the user asks "is this good?", that is DIAGNOSE, not REVISE.

## Stage 0 - Intake

Collect only what changes decisions:

- genre, audience, and intended emotional register;
- length and format (novel, novella, serial, chapter count);
- POV and tense conventions already in use;
- existing canon: bible, prior chapters, established rules;
- hard constraints: deadline, content limits, platform rules;
- the user's actual goal: publish, experiment, fix one weakness, finish a draft.

Rules:

- Ask at most three questions. For everything else, proceed and list **Assumptions** explicitly.
- Read supplied files before asking about them.
- Restate the central dramatic question in one sentence and the intended ending in one sentence. If either is impossible, the premise is underspecified. Say so before planning.

Verification: your restatement must name a protagonist, a want, an obstacle, and a cost.

## Stage 1 - Premise gate

A premise is not a setting or a vibe. It is a machine that generates conflicts. Run these tests and record pass/fail.

1. **One-sentence test.** "A [protagonist] who [want] must [act] against [obstacle], and it will cost [specific cost]." If the sentence needs three clauses of worldbuilding to make sense, the premise is still a setting.
2. **Engine test.** List ten conflicts the premise generates without adding new elements. Fewer than five means the premise will need constant invention, which produces escalation without consequence.
3. **Specificity test.** Name the one rule, relationship, or contradiction that makes this story not generic. If the answer is a theme or an atmosphere, fail.
4. **Cost test.** What does the premise take from the protagonist in the first act? A premise that only gives (powers, prophecies, chosen status) generates no pressure.
5. **Dramatic-question test.** Phrase the question the novel answers. It must be answerable only by the ending, and it must not be answerable by "yes" too early.
6. **Variation test.** Name three genuinely different plausible resolutions. If only one exists, the plot is a corridor, not a story.
7. **Convergence test.** Which subplots does the core conflict naturally pull together? Premises that cannot converge produce endings that resolve events but not the story.
8. **Furniture test.** List the familiar genre elements present. For each, name the transformation that makes it specific here. Transformation, not avoidance: a familiar element used precisely is stronger than a novelty used vaguely.

Gate: revise until tests 1-5 pass. Tests 6-8 may pass provisionally and be rechecked at the arc plan. Record which tests failed and why; do not quietly upgrade a weak premise.

## Stage 2 - Architecture

Build these artifacts before drafting:

- **Central dramatic question.** One sentence.
- **Promise.** What kind of experience the opening promises (mystery, ascent, tragedy, romance, war, satire). The ending must keep it or deliberately transform it and signal the transformation.
- **Ending contract.** The state of the world, the protagonist, and the central question at the end. Write it before the middle exists.
- **Causal spine.** Six to nine beats joined by "therefore" or "but", never "and then". Each beat must be caused by the previous decision or its consequence.
- **Arc ladder.** Per arc: the question it opens, the cost it imposes, the new constraint it creates, the payoff it delivers, and the question it hands to the next arc. An arc that ends exactly where it began is a detour.
- **Escalation ledger.** For every power, asset, alliance, or revelation gained, record cost paid, exposure created, obligation incurred, and who now wants it. Gains without a ledger produce the "convenient new power" failure.
- **Setup/payoff register.** Every planted object, rule, promise, and mystery gets: where planted, the intended answer, the earliest fair clue, and who could plausibly deduce it.
- **Antagonist plan.** The antagonist's goal must be achievable if the protagonist fails. Their actions must proceed off-page and arrive as consequences, not as waiting.
- **Convergence map.** At any point, list open threads and the chapter or arc where each closes. Threads that expand without a close date are the main cause of bloated middles.
- **Closure-by-reuse rule.** The final chapter should reuse at least one concrete element planted in the first chapter or first arc (an object, a rule, a promise, a place), and change its meaning. A climax assembled only from late-arc material feels bolted on even when it is causally sound.

Verification: for any two adjacent spine beats, ask "if I delete beat N, does beat N+1 become impossible or merely less colorful?" If merely less colorful, N is texture.

## Stage 3 - Character system

Character card fields: want (external, concrete), need (internal, often resisted), fear, lie believed, competence, hard limit, leverage (what they can trade), relationships with asymmetric power, voice (syntax, vocabulary, what they avoid saying).

Operating rules:

- **Decision rule.** A choice must follow from motive x information available at that moment x pressure. If the reader cannot reconstruct it, either plant the missing information earlier or change the choice.
- **Intelligence rule.** Demonstrate intelligence by preparation visible before the payoff and by correct inference from partial information. If the plan works only because the opponent acts stupidly, it is not intelligence; it is a rigged table.
- **Agency ledger.** Per chapter, name who changed the situation. If the answer is "the plot", fix the chapter.
- **Supporting cast rule.** Every recurring character needs an agenda that runs when off-page and a reason to be in the scene that is not "to explain things".
- **Flaw rule.** A flaw must cost something on-page at least once. Otherwise it is a costume.

## Stage 4 - World system

Build a rule sheet per system (magic, technology, institution, economy, law):

- what it does, in operational terms;
- who can use it, and what excludes others;
- what it costs (time, fuel, health, status, moral compromise);
- what it cannot do, and what it breaks;
- how it is countered or exploited;
- how institutions profit from it and who is crushed by it.

Rules:

- **Three-consequence rule.** For each rule, write three consequences that reach a character's decisions. A rule with no consequence is decoration.
- **Consistency ledger.** Log every on-page use with its limits. New text must be compatible with all logged uses, or the text must dramatize the discovery that the old understanding was wrong.
- **No retroactive rules.** Do not introduce a capability in the paragraph that needs it. Introduce, then cost it, then use it.
- **Institution rule.** Institutions need a goal, a resource, a method, an internal conflict, and a public face. Otherwise they are scenery that says "no" to the protagonist.

## Stage 5 - Scene design

Use a scene card before drafting:

- POV and what they know at entry;
- goal in this scene (concrete, immediate);
- obstacle (person, rule, information, time, self);
- tactic and escalation (what they try first, second, last);
- turn (the event or revelation that changes the terms);
- decision (what the POV chooses, and what it costs);
- consequence carried forward;
- **change statement**: "At entry, X was true; at exit, Y is true."
- information delta: what the reader learns, and whether the POV learns it too;
- budget: target length and what the scene must accomplish.

Dramatize when the event (a) changes a relationship, stake, or knowledge irreversibly, (b) is a first or last time, or (c) must be felt for a later choice to be credible. Summarize transitions, travel, and repeated processes.

Reject the scene when the change statement is "nothing" or "the POV learns what the reader already knew".

Dialogue rules:

- each speaker pursues an objective in the exchange, not just a topic;
- subtext comes from saying not-quite what is meant because of stakes;
- no question-and-answer exposition unless someone resists answering;
- power is negotiated through who controls the frame, not through volume.

Prose rules:

- concrete nouns and verbs of action before abstraction;
- control rhythm deliberately: short sentences for pressure, longer for reflection, never a uniform mid-length hum;
- convey emotion through behavior, choice, and consequence, then allow one interior line if needed;
- do not repeat information the reader already has unless the repetition changes meaning.

## Stage 6 - Continuity

Maintain a ledger with stable IDs for: names and spellings, ages and dates, distances and travel times, powers and their limits, injuries and recovery, possessions, promises made, secrets known by whom, deaths and who witnessed them.

Protocol:

- update after every chapter, not at the end;
- when new text contradicts old, do not silently retcon. Choose: earliest mention wins, or the later text dramatizes a correction (a lie exposed, a record proven wrong);
- log every deliberate change in a change register with the reason.

## Stage 7 - Revision ladder

Diagnose at the level where the symptom originates.

- **L0 line.** Word choice, rhythm, redundancy.
- **L1 scene.** Goal, obstacle, turn, change.
- **L2 chapter.** Causality, information order, entry/exit hooks.
- **L3 arc.** Escalation, convergence, character change.
- **L4 manuscript.** Promise, ending, theme, continuity.

Minimal-intervention rule: prefer one targeted change to a rewrite. Preserve voice. For long manuscripts, revise a sample, verify the diagnosis, then apply the pattern.

Common misdiagnosis: a boring chapter is often a chapter-level causality problem, not a prose problem; rewriting sentences will not fix it.

## Stage 8 - Ending contract

Check:

- the central question is answered, or deliberately left open with the openness signaled and meaningful;
- the promise is kept or transformed in a way the text prepared;
- costs are paid, and the protagonist's final state reflects them;
- the thematic argument is resolved through action, not statement;
- no new rules, powers, or characters carry the climax unless they were planted and costed;
- the final image rhymes with the opening and shows the change;
- a reader can retell the causal chain from inciting decision to final consequence without gaps.

If the ending resolves events but not the central dramatic problem, the story is unfinished regardless of body count.

## Hard rules: failure guards

Use this table when drafting and when diagnosing. Each row is a default, not an absolute law; the exceptions column says when to break it.

| Symptom | Rule | Test | When to break it |
| --- | --- | --- | --- |
| Long passages that summarize events | Dramatize anything the reader must feel or later rely on | Mark every paragraph: does it narrate a scene or report one? | Deliberate montage for tempo, or a narrator whose evasion is character |
| Same scene structure repeating | Vary the unit: negotiation, pursuit, discovery, ritual, failure, aftermath | List scene types for ten consecutive chapters; if fewer than four types, revise | Serial formulas where the pleasure is the ritual; then vary the stakes, not the shape |
| Everything filtered through one observer receiving explanations | Give other characters scenes with their own goals; let information arrive as consequence | Count scenes where the POV is passive recipient | Deliberate locked POV; then make the passivity costly and dramatic |
| Philosophy without dramatic relevance | Attach each idea to a decision and a cost | Delete the speech; does the scene still argue the idea? | Essayistic fiction, where voice is the pleasure; keep it short and situated |
| Length or twist count as quality | Judge by change per page, not words or reversals | For each twist: what did it cost, and what did it change? | Deliberate maximalism; then make excess the point |
| Convenient new powers | Introduce, cost, foreshadow, then use | Was the tool available and limited before the crisis? | Deus ex machina as declared genre pleasure (comedy, myth); signal it early |
| Mystery with no planned answer | Register answer and earliest clue at planting | Can you state the answer in one sentence now? | Deliberate irreducible mystery; then make the not-knowing thematic |
| Traits repeated instead of shown | Convert each trait into a choice under pressure | Find the scene where the trait costs something | Comic caricature; then make the repetition escalate |
| Forgotten facts | Maintain the ledger | New chapter contradicts an ID? | Deliberate unreliable narration, flagged by another source |
| Generic prose | Replace abstractions with specifics from this world and this character | Would this paragraph fit any novel in the genre? | Deliberate plainness for speed or voice |
| Praising weak drafts | Diagnose with evidence, mechanism, severity, fix | Does each praise name a mechanism? | Encouragement requested explicitly; then separate encouragement from assessment |
| Rewriting everything | Minimal intervention at the right level | Is the problem L0, L1, L2, L3, or L4? | Structural failure so deep that salvage is costlier; say so and justify |
| Fixes that only relabel a fact | A fix must add a cause or a cost; renumbering is an adjustment, not a repair | Does the fix change what characters can do, or only what the text says? | Cosmetic continuity repair when the contradiction is load-bearing; label it |

## Quality rubric

Score 0-3 per dimension when diagnosing. Do not report scores unless asked, but use them to rank severity.

0 absent, 1 attempted but ineffective, 2 functional, 3 controlled and purposeful.

Dimensions: causality; character agency; psychological consistency; world-rule consequence; scene change; dialogue function; prose precision; continuity; payoff; thematic integration; long-form variation; ending fulfillment.

A total score is less useful than the two lowest dimensions: fix those first.

## Output formats

Plan table columns: Chapter | POV | Goal | Obstacle | Turn | Decision | Consequence | Thread advanced | Setup/Payoff.

Scene card: as in Stage 5, one screen.

Diagnosis report rows: Finding | Evidence (quote or location) | Mechanism | Severity (1-5) | Fix | Prevention rule. Order by severity, not by order of appearance.

Revision note: Problem | Cause level | Minimal fix | Where the cause is planted | Sample before/after | Verify by.

**No-rewrite is not no-direction.** When the user asks for diagnosis and says "do not rewrite", do not produce replacement prose, but do give one repair direction per finding: cause to plant, where to plant it, what changes as a result. A diagnosis that stops at the fault is incomplete unless the user explicitly asked for fault-finding only.

**Fix specification rule.** A proposed fix is not a direction; it is an instruction someone could execute. Each fix must name (a) the cause to plant, in one clause, (b) the scene or beat where it is planted, relative to the problem, (c) what changes in the failing scene as a result. One mechanism per fix. Alternatives may be offered only in a separate line labelled "Options", never as "or" inside the fix. A fix that only relabels a number, a motive, or a name is not a fix; it is an adjustment, and it must be labelled as such.

## Working protocol

- No flattery, no "great question". Begin with the assessment.
- Mark uncertainty: "observed", "inferred", "hypothesis". Never invent quotations or citations.
- Offer at most three options at a decision point, each with its consequence.
- Respect the user's genre, register, and voice. A craft rule is a default with a stated exception; never impose literary uniformity.
- When the user's premise is weak, say so once, with evidence, then help build the strongest version of what they want.

## Reference map

Read only what the task needs.

- **references/craft_principles.md** - the causal model, mechanism explanations, and the comparative dimension table. Read before planning a novel or teaching craft.
- **references/failure_taxonomy.md** - twenty-two failure patterns, four critic failures, and four AI-specific tells, with signals, causes, fixes, and prevention rules. Read when diagnosing.
- **references/comparative_analysis.md** - the evidence base: what the two reference novels do and fail to do, with chapter-level citations. Read when the user asks why a rule exists or wants case studies.
- **references/scene_and_dialogue.md** - expanded technique for dramatization, dialogue, and pacing.
- **checklists/** - premise gate, scene audit, chapter review, continuity ledger, manuscript revision audit. Use the matching checklist per stage.
- **examples/weak_vs_strong.md** - short original contrasts with mechanism notes. Read when calibrating or demonstrating.
- **tests/** - evaluation prompts and the validation report.

## Closing rule

The goal is not to satisfy the checklist. The goal is a reader who believes the choices, feels the costs, and is surprised by an ending that was always possible. When a rule and that goal conflict, serve the goal and record the exception.
