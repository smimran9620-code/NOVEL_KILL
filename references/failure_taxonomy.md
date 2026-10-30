# Failure Taxonomy

Twenty-two failure patterns, ordered from structural to line-level, plus four critic-side failures and four AI-specific tells. Each entry gives the signal, the mechanism of damage, the usual cause, a concrete fix, and a prevention rule. Evidence marked "Invisible Dragon" is from the failure reference analysed in references/comparative_analysis.md; quotes are short and chapter-numbered.

Use this file in DIAGNOSE mode: identify patterns, rank by severity, and cite evidence. Do not list every pattern that could apply; list the ones that do.

## Severity scale

1 cosmetic; 2 local irritation; 3 damages belief in a scene; 4 damages belief in an arc; 5 damages the story's foundation.

---

## F01 - Premise without an engine

**Signal.** The premise is a setting, a tone, or a power. Conflict must be imported from outside it; each new chapter adds a new element to stay interesting.
**Damage.** The middle cannot generate its own events, so the author invents escalation instead of consequence. Reader interest depends on novelty, which decays.
**Cause.** Starting from an image or a genre rather than from a protagonist's want under a specific constraint.
**Evidence.** Invisible Dragon: a dragon that wins everything (ch. 1-3) has no obstacle, so the text must invent a stronger foe every few chapters (ch. 12, 14, 15, 23, 25, 49) and each is cancelled by the next.
**Fix.** Rewrite the premise as protagonist + want + obstacle + cost. Then list ten conflicts it generates without new elements. Keep the premise only if five are usable.
**Prevention.** Premise gate, tests 1-5 (SKILL.md Stage 1).

## F02 - Causality by convenience

**Signal.** An event happens because the plot needs it. The text supplies a motive after the fact, or a character happens to be present, or a rule happens to apply.
**Damage.** The reader stops modelling causes and starts waiting for the author. Suspense collapses because outcomes are not implied by prior choices.
**Cause.** Writing from the desired scene backwards without planting the cause forwards.
**Evidence.** Invisible Dragon: the hero survives a universe-ending explosion via "selfdestroction dodge", a skill introduced in the same paragraph with a weakness never used again (ch. 29); a new ultimate skill appears mid-duel (ch. 50).
**Fix.** For each convenient event, write the causal chain that should have produced it and plant the earliest link one arc earlier, in a named scene. If the event cannot be planted, cut it. State the fix as cause + placement + changed scene, with one mechanism only.
**Prevention.** Causal spine joined by "therefore/but". Delete test on every beat.

## F03 - Character acts against established motive

**Signal.** A character who has been ruthless is merciful, or a coward is brave, at exactly the moment the plot requires it, with no scene that changes them.
**Damage.** The reader's model of the character breaks; later decisions stop carrying weight because the character is not a stable object.
**Cause.** Plot outline written before character logic, or a scene imported from another draft.
**Fix.** Add the turning scene, or change the plot to fit the character. Prefer changing the plot: it is usually cheaper and always more surprising.
**Prevention.** Decision rule: motive x available information x pressure. If the chain cannot be reconstructed, do not write the choice.

## F04 - Repetitive event structure

**Signal.** The same scene shape recurs: arrive, be underestimated, demonstrate power, be praised; or negotiate, be betrayed, retaliate. New nouns, same machine.
**Damage.** Predictability replaces suspense; the reader begins skimming because the shape is known.
**Cause.** A reliable unit that worked once and was never varied; serial production pressure.
**Evidence.** Novel A itself shows the risk at scale: its arena-to-asset conversion loop recurs with cosmetic variation across hundreds of chapters, and two contest arcs run the same procedure.
**Fix.** Track the last five scene types. Replace one with a structurally different unit (aftermath, preparation, failure, ritual, institutional scene).
**Prevention.** Scene-type rotation; vary stakes, not just costumes.

## F05 - Scenes that repeat information without changing the situation

**Signal.** The change statement is "they learn what the reader already knew", or "the argument continues". The scene could be deleted without altering the next.
**Damage.** Pacing dies; the reader feels managed.
**Cause.** The author is reassuring themselves that the point landed, or padding to a word count.
**Fix.** Cut, or convert the information into a decision with a cost. One scene per revelation.
**Prevention.** Scene change statement mandatory before drafting.

## F06 - Summary substituting for drama

**Signal.** Important events are reported in one clause ("he trained for three million years"; "the war ended"); dialogue is avoided at moments of highest stakes.
**Damage.** The reader is told what to feel rather than made to feel it; later emotional payoffs have no accrued weight.
**Cause.** Fear of writing the difficult scene; word-count efficiency; AI default toward narration.
**Evidence.** Invisible Dragon: of 50 chapters, roughly 49 are pure summary; chapters 1-49 contain two speaker-tagged lines of dialogue, against 83 in the final chapter.
**Fix.** Identify the three scenes the novel's meaning depends on and dramatise them. Summarise only transitions.
**Prevention.** Dramatisation threshold: dramatise anything later choices depend on.

## F07 - Artificial dialogue / explaining what both parties know

**Signal.** Characters recite worldbuilding to each other; questions are asked only so answers can be delivered; everyone speaks in the same register; no one refuses to answer.
**Damage.** Illusion of real people collapses; exposition becomes visible as machinery.
**Cause.** The author using dialogue as a delivery pipe.
**Fix.** Give each speaker an objective that conflicts with the other's. Let information emerge through resistance, evasion, or cost. Cut any exchange where both parties already know the content.
**Prevention.** Dialogue test: what does each speaker want from the other in this exchange?

## F08 - Unconvincing intelligence

**Signal.** The narrator or other characters say the protagonist is brilliant; the plans work because opponents are stupid, information arrives free, or the plan is never shown being constructed.
**Damage.** The reader cannot verify the trait; admiration is demanded, not earned. Every later "genius" move is discounted.
**Cause.** Confusing complexity with intelligence; writing the reveal without the preparation.
**Evidence.** Invisible Dragon: the hero wins by being "super duper strong" and by enemies failing to see him; the text asserts superiority in place of a contest (ch. 22-23). Novel A, by contrast, shows the arithmetic: a 44% essence cap makes a contest unwinnable, so the protagonist abandons it for a different route (ch. 10, 17).
**Fix.** Show preparation before payoff: resources gathered, inferences made from partial information, contingencies. Let the opponent be competent.
**Prevention.** Intelligence test: reconstruct the reasoning from information available before the decision.

## F09 - Effortless victories and vanishing consequences

**Signal.** The protagonist wins without cost; enemies disappear; injuries heal off-page; political fallout never arrives.
**Damage.** Stakes deflate permanently. The reader learns that outcomes do not matter.
**Cause.** Escalation without a ledger; reluctance to write aftermath.
**Evidence.** Invisible Dragon: a single punch erases 600 universe lords (ch. 50); the hero recovers "in 0.03 secons" and then is dying three lines later.
**Fix.** After every victory, write the bill: cost paid, exposure created, obligation incurred, enemy made. Then use one of them in the next arc.
**Prevention.** Escalation ledger updated per arc.

## F10 - Arbitrary escalation / power inflation

**Signal.** Numbers and titles grow without new constraints; each threat is stronger than the last by declaration; the scale becomes comic.
**Damage.** Danger becomes unbelievable; the reader stops doing arithmetic; the climax has no measurable stakes.
**Cause.** Mistaking magnitude for tension; no constraint model.
**Evidence.** Invisible Dragon: 1/10^37 of power destroys 350,000 meteors (ch. 23); then 1/10^39, then a 52-digit superiority claim (ch. 49); then percentages (1%, 2%, 3%) that reset the scale again.
**Fix.** Replace magnitude with constraint: time, obligation, exposure, dependence, morality. A weaker character with fewer options can be in more danger.
**Prevention.** Escalate by narrowing options and raising costs, not by adding zeros.

## F11 - Inconsistent world rules

**Signal.** A rule holds until it is inconvenient; a power's limits change between uses; the same feat is impossible in chapter 5 and trivial in chapter 20 without explanation.
**Damage.** The reader cannot predict or evaluate; strategy becomes impossible, so victories feel arbitrary.
**Cause.** No rule sheet; invention in the moment.
**Evidence.** Invisible Dragon: invisibility is total (ch. 5, 10) but the narrative dwells on the hero's beauty being seen (ch. 9); the "mind's eye" solves invisibility (ch. 26) and is then forgotten until a villain teaches soldiers to see him (ch. 50).
**Fix.** Build a rule sheet with costs and limits; reconcile every prior use or dramatise the discovery that the old understanding was wrong.
**Prevention.** Consistency ledger of every on-page use.

## F12 - Continuity contradiction

**Signal.** Names change spelling; ages, dates, distances, counts conflict; a dead character reappears; a building is 63 storeys and 100 storeys in one sentence.
**Damage.** Trust erodes cumulatively; readers who notice stop investing.
**Cause.** No ledger; revision without propagation; translation or serialization noise mistaken for canon.
**Evidence.** Invisible Dragon: "a 63 story building no there was a building over 100 stories" (ch. 6); universes totalling 999, then 900, then "300... actually 399" (ch. 29, 34, 35, 43); a character named shana, shang-a, and Shang'a (ch. 44, 50).
**Fix.** Choose earliest mention or dramatise a correction; log every change.
**Prevention.** Continuity ledger with IDs, updated per chapter.

## F13 - Exposition dump / unintegrated worldbuilding

**Signal.** Blocks of history, rules, or politics arrive without a character needing them to act; the scene pauses while the narrator lectures.
**Damage.** Pacing stalls and the world feels like a manual.
**Cause.** Authorial pride in invented material; fear the reader will not understand.
**Fix.** Deliver information as a consequence, a conflict, or a decision: a rule that blocks an action, a custom that humiliates someone, a price that ruins a plan. Interleave in small doses at moments of pressure.
**Prevention.** Exposition test: does someone need this to act in the next page?

## F14 - Predictable twists and unearned revelations

**Signal.** The twist is the only option the text has excluded; or it depends on information withheld from the reader entirely; or it requires a character to have concealed a fact from their own interiority.
**Damage.** Surprise without inevitability feels like cheating; inevitability without surprise feels flat.
**Cause.** Designing backwards from the reveal without planting fair clues.
**Fix.** Plant two unobtrusive clues; make the reveal change the meaning of an earlier scene rather than merely add information.
**Prevention.** Fair-play register: answer, earliest clue, who could deduce it.

## F15 - Abandoned setups / dangling mysteries

**Signal.** A promised duel, a loaded object, a question, or a threat never returns. The text forgets what it made the reader remember.
**Damage.** The reader feels used; unresolved promises are experienced as negligence even when unintentional.
**Cause.** Organic drafting without a register; enthusiasm for new ideas over closure.
**Evidence.** Invisible Dragon: "the ultimade demon king god the master dragon" is announced and never appears (ch. 43); a "mistake" is named but never specified (ch. 34); a promised sequel and origin arc are abandoned (ch. 28, 46).
**Fix.** Either pay the setup, explicitly retire it (a character decides it no longer matters, with a cost), or cut the plant.
**Prevention.** Setup/payoff register with answer and chapter.

## F16 - Philosophical decoration

**Signal.** A character delivers a speech about fate, power, or humanity that the plot neither tests nor complicates. The ideas would survive the deletion of every scene.
**Damage.** The reader feels lectured; the theme loses weight because nothing was risked for it.
**Cause.** Wanting depth without designing dilemmas.
**Fix.** Convert the idea into a choice between two goods, with a cost either way. Let two characters embody rival answers and make both pay.
**Prevention.** Delete-the-speech test: what in the scene still argues the idea?

## F17 - Unearned emotion

**Signal.** "She felt immense sadness." A death lands in the same paragraph as the introduction. A love is declared after one conversation.
**Damage.** Emotion is asserted, not transferred; the reader resists being told what to feel.
**Cause.** Skipping the accrual scenes.
**Fix.** Build the relationship's ordinary texture and cost before the loss; let behaviour carry the feeling.
**Prevention.** Emotional accrual rule: invest before you spend.

## F18 - Manufactured cliffhangers

**Signal.** Chapters end on fake-out deaths, interrupted sentences, or revelations that are undone in the next chapter's first line.
**Damage.** The device trains the reader to distrust chapter endings; genuine tension is discounted.
**Cause.** Serial metrics; mistaking interruption for suspense.
**Evidence.** Novel A itself uses a life-tablet fake-out: a cliffhanger implies a character's death and is reversed shortly after, spending suspense for one turn.
**Fix.** End on a decision or a consequence, not on withheld information. If a cliffhanger is used, the next chapter must not simply deny it.
**Prevention.** Chapter-exit test: does the exit change the terms, or only hide them?

## F19 - Prose tics: repetitive syntax, empty intensifiers, uniform rhythm

**Signal.** Every paragraph is the same length; sentences begin the same way; abstractions stack ("a sense of overwhelming power"); intensifiers replace specifics ("incredibly", "absolutely", "super").
**Damage.** The reading experience flattens; emphasis stops registering because everything is emphasised.
**Cause.** Drafting by pattern completion; no read-aloud pass.
**Evidence.** Invisible Dragon: "the invisible dragon was super duper strong" recurs as a substitute for demonstration; 18 lines end on "awesome"; the name appears 247 times in 7,532 words.
**Fix.** Vary sentence length at turns; replace intensifiers with specifics; delete the sentence that explains the previous sentence.
**Prevention.** Read-aloud pass; count repeated sentence openings per page.

## F20 - Plotlines that expand without converging

**Signal.** New factions, mysteries, and subplots keep opening; old ones are neither closed nor deliberately abandoned; the middle grows.
**Damage.** The ending cannot resolve what it never gathered; the reader's investment is dispersed.
**Cause.** Improvisation without a convergence map.
**Fix.** For every open thread, assign a closing chapter now. Merge or cut threads that cannot converge by the planned climax.
**Prevention.** Convergence map reviewed at each arc boundary.

## F21 - Ending resolves events but not the question

**Signal.** The villain is defeated and the world is saved, but the central dramatic question (who is this person? what is worth sacrificing? can the system be escaped?) is unanswered.
**Damage.** The story feels unfinished despite closure.
**Cause.** The plot was planned; the question was not.
**Fix.** Answer the question in the final act through a choice that costs. If the answer is deliberately open, make the openness the answer and signal it earlier.
**Prevention.** Ending contract written before the middle.

## F22 - Intrusive narration or meta-commentary

**Signal.** The narrator summarises what the chapter will show, addresses the reader, apologises, or comments on the writing. Author notes inside chapters.
**Damage.** Immersion breaks; the story becomes a document about itself.
**Cause.** Uncertainty about whether the scene works; serial habits; AI defaults ("In this chapter, we will see...").
**Evidence.** Invisible Dragon: 19 of 50 chapters are author notes; the author argues with commenters inside the fiction (ch. 13, 16, 31, 42, 48).
**Fix.** Cut. If a frame narrator is intended, make the frame a character with stakes.
**Prevention.** First-line audit: does the chapter begin inside a situation?

---

## Critic-side failures (for AI editors)

## C1 - Praise instead of diagnosis

**Signal.** "This is strong writing." "The prose flows beautifully." No mechanism named, no evidence cited.
**Damage.** The writer learns nothing and cannot reproduce the effect; weak drafts ship.
**Fix.** Every evaluative sentence must name a mechanism and a location.
**Prevention.** Diagnosis report format: Finding | Evidence | Mechanism | Severity | Fix.

## C2 - Wholesale rewriting

**Signal.** The editor rewrites every paragraph when the problem is one structural beat.
**Damage.** Voice is flattened; the writer's ownership is lost; the actual cause survives the rewrite.
**Fix.** Diagnose the level (L0-L4) and intervene only there. Show a sample.
**Prevention.** Minimal-intervention rule.

## C3 - Invented evidence

**Signal.** Quotations or chapter references that do not exist; claims about a text not read.
**Damage.** Catastrophic loss of trust; analysis becomes fiction about fiction.
**Fix.** Cite only verified text; mark inference and hypothesis.
**Prevention.** Evidence labels: observed / inferred / hypothesis.

## C4 - Uniformity imposed as quality

**Signal.** Every genre is pushed toward the same literary register; deliberate stylisation is corrected as error.
**Damage.** The editor destroys what makes the work distinctive.
**Fix.** Ask what effect the author is buying. Judge execution against intent, not against a single house style.
**Prevention.** State the intended register before evaluating; list deliberate exceptions.

---

## AI-specific extra patterns

These are common in machine-generated drafts and worth checking explicitly.

- **A1 Firehose padding.** Length substituted for development: every beat restated in three registers (action, thought, summary). Fix: one register per beat.
- **A2 Symmetrical chapter shape.** Every chapter opens with weather, moves to dialogue, ends with a reflective line. Fix: vary entry and exit points; enter late, leave early.
- **A3 Hedge-prose.** "There was a mixture of X and Y in her expression"; "something shifted in the air". Fix: commit to one concrete observable.
- **A4 Recap openings.** "Previously..." or a summary of the last chapter in the first paragraph. Fix: begin in the middle of the new pressure; trust the reader.
