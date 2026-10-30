# Platform Compatibility and Installation

The method is portable; the packaging is not universal. This file separates what was verified against current documentation from what is general guidance.

## 1. What travels

- **Method:** SKILL.md, references, checklists, examples and tests are plain Markdown. Any AI with file access or a long system prompt can use them.
- **Trigger:** the YAML description in SKILL.md frontmatter is what makes an agent load the skill automatically. Preserve it when adapting.
- **Progressive disclosure:** the main file is under 500 lines; detail lives in references and checklists. Keep that split in any adaptation.

## 2. Claude Agent Skills (verified)

Verified against platform.claude.com documentation (Agent Skills overview, Best practices, Skills API guide; retrieved October 2026). Re-check before publishing; the format has changed before and will change again.

### Required structure

A skill bundle is a directory with SKILL.md at the top level:

    writing-novels/
      SKILL.md
      README.md
      references/...
      checklists/...
      examples/...
      tests/...

### Frontmatter rules

- name: required, maximum 64 characters, lowercase letters, numbers and hyphens only, no XML tags, must not contain the reserved words "anthropic" or "claude".
- description: required, maximum 1,024 characters, non-empty, no XML tags, and must state both what the skill does and when to use it. This is the text the model matches against a request.
- license and allowed-tools are optional in current documentation.

This package uses name: writing-novels and a description that names the tasks and the trigger conditions.

### Size guidance

Documentation recommends keeping the SKILL.md body under 500 lines for best performance and splitting detail into separate files. This package's SKILL.md is about 250 lines.

### Installation by product

**claude.ai.** Upload the skill as a ZIP through Settings > Features. Custom skills require a plan with code execution enabled (Pro, Max, Team or Enterprise at the time of writing). Custom skills are individual to each user, not shared organization-wide. Upload the folder, not the loose files: the ZIP must contain a top-level directory holding SKILL.md.

**Claude Code.** Place the directory in ~/.claude/skills/ for personal use or .claude/skills/ inside a project. No upload step; Claude Code discovers and loads it automatically. Unzip the archive so that the path is .../skills/writing-novels/SKILL.md.

**Claude API.** Upload with POST /v1/skills (multipart, files[] entries named with their path inside the bundle, or a single ZIP) or with the SDK's files_from_dir helper, then reference the returned skill_id in the container parameter alongside the code execution tool: type "custom", version "latest" or a specific version ID. Custom skills are shared workspace-wide. The container has no network access.

**Claude Platform on AWS / Microsoft Foundry.** Documentation states custom skills are uploaded through the Skills API for these deployments; on Foundry, hosted-on-Anthropic deployments are required.

### Activation

Skills load when the description matches the request. If a user's request is oblique ("my draft feels flat"), the skill may not trigger; in that case the user can name it explicitly.

## 3. Adapting to other AI environments (general guidance, not vendor-verified)

No other platform is guaranteed to implement this format. The reliable adaptation is: keep the method, change the packaging.

| Environment type | Practical adaptation |
| --- | --- |
| Systems with a persistent instruction file (AGENTS.md, project rules, custom instructions, system prompt) | Paste SKILL.md as the standing instruction block, then attach the references that the current task needs. Keep the frontmatter as a comment or a header so the trigger text survives. |
| Chat with a long system prompt or a custom GPT/Gem/Gemini-style assistant | Put SKILL.md in the instructions, and add one line naming the file paths you will paste on demand ("when the user asks for a diagnosis, request references/failure_taxonomy.md"). |
| IDE agents with rule files | Use SKILL.md as the rule body; keep references/ next to it and reference them by relative path. |
| API or agent frameworks with tools | Expose the skill directory as readable files and add the description to the tool's or agent's routing prompt. |
| No file access at all | Use the condensed single-document mode (section 4). |

### Portability rules

- Do not depend on scripts, network access, or platform-specific tools. This package has none.
- Use relative links between files so the bundle works wherever it is unzipped.
- Keep the trigger description free of vendor names; it should describe the task, not the platform.
- If a platform truncates long instructions, load SKILL.md only, and pull checklists on demand.

## 4. Condensed single-document mode

For environments with a tight context budget, concatenate:

1. SKILL.md (all of it).
2. checklists/scene_audit.md and checklists/revision_audit.md (the two most-used tools).
3. The mechanism list from references/craft_principles.md, section 4.

Leave the comparative analysis and failure taxonomy out unless the user asks for evidence or diagnosis. This preserves roughly 80% of the operational value at about 40% of the length.

## 5. Known limitations

- Automatic triggering is probabilistic. A skill is a strong prior, not a guarantee.
- Reference files cost context only when read; a model that never reads them will behave like SKILL.md alone.
- The skill cannot verify facts about a user's manuscript that are not in the files it is given; it must ask for or read the text.
- Nothing here is a substitute for a human editor's taste on questions the method treats as conventions (register, genre expectations, content boundaries).
