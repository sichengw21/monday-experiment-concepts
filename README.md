# Monday experiment concepts

A reusable Claude skill for turning Monday.com experiment ideas into interactive HTML concepts aligned with an existing prototype.

## Workflow

Ready for concepts → Concepting → Ready for review → Approved for integration → Integrated.

Claude reads the Monday brief, references the local HTML prototype, and generates a separate versioned concept. Review links, feedback, and approval are recorded in Monday. Only the approved version is integrated into the prototype's experimentation tabs.

## Get the skill

- [Read SKILL.md](SKILL.md)
- [Download the skill package](monday-experiment-concepts.zip)

The package contains `monday-experiment-concepts/SKILL.md`. Use it in your Claude skill setup, or give Claude the skill file as workflow instructions.

## First-run settings

Provide your Monday board and status mapping, local HTML prototype location, authorized reviewers, and preview location. Claude should reuse the prototype's existing styles, assets, components, and interaction patterns.

Start by asking Claude: “Use this skill to analyze the items marked Ready for concepts on my Monday board and create concepts using my existing HTML prototype. Save review details in Monday and stop before integration until I approve a specific version.”

## Automation

The skill defines the workflow; it does not install a watcher or start jobs automatically. Automatic processing requires a separately configured runner with access to Monday and the local prototype. Webex and Figma are not required.
