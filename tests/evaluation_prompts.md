# Evaluation Prompts

Tests for whether the skill improves narrative reasoning and drafting. They are independent of the two novels: none of the premises, scenes, or failures below is taken from the reference texts.

## Protocol

For each test, run two conditions:

- **Baseline:** the task prompt alone.
- **Skill-guided:** the same prompt plus: "Read the skill at <path>/SKILL.md and follow it, reading any file it directs you to."

Keep outputs under the stated word limit. Score with the rubric (0-3 per criterion). Where feasible, have a judge score anonymised outputs without knowing the condition. Record results in validation_report.md.

Do not use these prompts to tune the skill between runs without noting it; otherwise the comparison is contaminated.

## Test 1 - Detect weak causality

Prompt: "Diagnose the plot logic of this synopsis. Do not rewrite it. 250 words max."

Synopsis (planted failures: (a) the map is found because a stranger leaves it; (b) the guard changes sides because the hero is kind; (c) the army arrives without being sent for; (d) the villain's weakness is invented at the climax):

> Wren is a courier in a city under siege. One morning she finds a map of the aqueducts on her doorstep, left by a stranger. The map shows a route into the palace. She sneaks in, and a guard named Oris catches her. She shares her food with him, and he decides to help her because she is kind. Together they reach the throne room, where the chancellor is about to sign a treaty that will surrender the city. Wren argues with him, but he does not listen. Then the city's army arrives at the gates and surrounds the palace, because the army had been waiting for a signal. The chancellor panics and attacks. Wren remembers that the chancellor is allergic to silver, and she throws a silver inkwell at him. He collapses, and the treaty is stopped.

Criteria (0-3 each): identifies at least three of the four planted holes; names the mechanism (why the hole damages belief); ranks severity; proposes a direction of repair without rewriting; does not invent unrelated faults.

## Test 2 - Repetitive scene detection

Prompt: "These are summaries of four consecutive chapters. What is structurally wrong, and what is the most useful fix? 200 words max."

> Ch. 1: Sela comes to the guild, is underestimated by the guildmaster, and proves her skill with a demonstration.
> Ch. 2: Sela comes to the barracks, is underestimated by the captain, and proves her skill with a demonstration.
> Ch. 3: Sela comes to the court, is underestimated by the minister, and proves her skill with a demonstration.
> Ch. 4: Sela comes to the temple, is underestimated by the priest, and proves her skill with a demonstration.

Criteria: names the repeated unit; explains the cost to the reader (predictability, no escalation); proposes varying function (exposure, failure, consequence), not merely varying setting; keeps the useful ritual element if the genre wants it.

## Test 3 - Strategic protagonist (drafting)

Prompt: "Write a 400-word scene in which a protagonist outmaneuvers a rival. The protagonist must win through preparation or inference, not through a new ability. The rival must be competent. The win must cost something. Third person, past tense."

Criteria: plan reconstructable from information available before the decision; rival acts intelligently; no ability introduced in the scene; a cost is paid and visible; the scene turns on a decision, not on luck.

## Test 4 - Five-chapter causal grid

Prompt: "Using the premise 'A disgraced bridge engineer must sabotage her own bridge to stop an invading army, while the army's scout is the man she loves', produce a five-chapter grid in which each chapter is caused by the previous chapter's consequence. One line per chapter, with a column for 'what it costs'. 250 words max."

Criteria: each step caused by prior decision/consequence; escalation narrows options rather than inflating scope; no new characters or powers carrying the plot; the cost column is specific; the fifth chapter's question is set up by the first.

## Test 5 - Dramatise, don't summarise

Prompt: "Convert this summary into a 350-word scene: 'Mira confronts her brother about the missing money and he admits he gambled it away. She decides not to turn him in.' Do not add new plot events."

Criteria: a real scene (place, want, resistance, turn, consequence); the admission is earned by pressure rather than volunteered; the decision has a visible cost; concrete detail; no summary sentences carrying the emotional weight.

## Test 6 - Continuity audit

Prompt: "Here are the established facts, then a new scene. List every continuity conflict and propose a resolution for each that is better than 'change the number'. 200 words max."

Facts: (1) The pass is a three-day ride from the fort. (2) Ilan's left hand was crushed in chapter 2 and cannot grip. (3) The garrison has forty soldiers. (4) The enemy is expected after the first snow. (5) Mira knows nothing about the smuggling.

New scene: "Two days after leaving the fort, Ilan reached the pass. He counted the garrison: sixty men. Snow was already falling. Mira showed him the smuggler's ledger and explained the route. Ilan gripped the rope and hauled himself up the cliff."

Criteria: catches travel time, hand, garrison count, Mira's knowledge, snow timing (any four); resolutions are dramatised or ledgered, not hand-waved; distinguishes which facts matter to the plot from which are trivia.

## Test 7 - Theme through action

Prompt: "Write a 300-word scene that argues the idea 'mercy can be a form of control' without any character stating it and without a narrator explaining it. Two characters, one room, one decision."

Criteria: idea is enacted through a choice and a cost; no thesis statement; subtext legible; the "merciful" character's control is visible in behaviour; the scene does not resolve the idea as simply good or bad.

## Test 8 - Ending evaluation

Prompt: "Evaluate this ending in 200 words: 'The dragon was slain, the kingdom was saved, and Lira was crowned queen and ruled wisely. The question of whether she had become the thing she hunted was left unanswered.'"

Criteria: identifies that events are resolved but the dramatic question is not; explains the mechanism; distinguishes deliberate openness from evasion; proposes a concrete test for whether openness is earned.

## Test 9 - Style preservation

Prompt: "Improve the prose of this passage without changing its register. It is meant to be pulpy and fast. 150 words max of commentary plus a revised version of no more than 120 words."

> The door exploded inward. Kade rolled, came up shooting. Two men went down. A third grabbed him by the collar and he headbutted the bastard right in the teeth. Blood sprayed. Kade grinned. 'You picked the wrong night,' he said.

Criteria: preserves register and pace; fixes only real problems (repetition, unclear blocking); does not literary-ise; explains the trade-off.

## Test 10 - False-positive control

Prompt: "Diagnose this scene. If it is largely working, say so. 200 words max."

> The kitchen smelled of burnt sugar. Ana set the tray down harder than she meant to. 'You said you'd tell her.'
> Her mother did not look up from the dough. 'I said I'd think about it.'
> 'That's not what you said.'
> The rolling pin stopped. 'If I tell her, she leaves. If I don't, she finds out in the spring when the lease comes due and she leaves anyway. Which one would you like me to choose?'
> Ana wanted to argue. She found she could not, because her mother had done the arithmetic first, and the arithmetic was correct. She took the tray back. 'I'll tell her,' she said. 'You'll hate me for it.'
> 'I already do,' her mother said, and went back to the dough.

Criteria: recognises the scene works (goal, resistance, turn, consequence); identifies at most one genuine minor weakness; does not manufacture structural faults; does not rewrite.

## Scoring

For each test, 0-3 per criterion. Report per-test and aggregate. Also record:

- **False positives:** problems invented in Test 10.
- **Misses:** planted failures not found in Tests 1, 6.
- **Voice damage:** register lost in Test 9.
- **Over-writing:** word-limit violations, or rewriting when diagnosis was requested.

## Interpreting results

A skill that scores higher on detection but lower on Test 9 has over-corrected toward literary uniformity. A skill that scores higher on Test 3 but not Test 4 has improved local craft without improving architecture. Report both, not just the aggregate.
