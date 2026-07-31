# how-to-illustrate

An AI / agent skill: a mandatory router for **any** request to draw, illustrate, diagram, chart, graph, visualize, or map something.

It gives an agent an exhaustive diagram-type taxonomy — 30+ categories and 200+ named types spanning processes, hierarchies, networks, business strategy, science, engineering, finance, UX, sports, music, and more — each with what it depicts, its structural anatomy, and when to reach for it over a near-neighbor type, a tool-selection framework (e.g. Excalidraw / tldraw / penecho, or whatever diagramming tools you have available), and a non-negotiable **interactivity-and-animation mandate** — so agents stop defaulting to a wall of prose or a static box diagram when a real, live visualization is what the user actually wants.

## Why

Left to their own devices, coding agents tend to:

- Describe something spatial or relational in a markdown table instead of drawing it.
- Reach for the first diagram type that comes to mind (usually a flowchart) even when a different type (a Sankey diagram, a Gantt chart, a decision tree, a Wardley map...) is the standard, recognizable choice for the domain.
- Produce a static image when the tool at hand could have made it interactive or animated.

This skill fixes all three by giving the agent a checklist to run through before it starts drawing.

## What's inside

`SKILL.md` walks the agent through four steps:

1. **Pick the right diagram type** — matched against 30+ categories (Processes & Workflows, Structures & Hierarchies, Relationships & Logic, Cybersecurity & Networks, Biological & Life Sciences, Chemistry, Physics & Astronomy, Linguistics & Social Sciences, Business & Strategy, Comparison & Ranking, Trends Over Time, Part-to-Whole, Distribution & Range, Correlation, Flow & Spatial, Product/UX, Manufacturing & Engineering, Finance & Economics, Environmental Science, Music & Audio, Sports & Games, Legal & Governance, Data Science & ML, Genealogy, and more), each type described in depth rather than as a one-line label.
2. **Pick the right tool** — a router for whichever diagramming/canvas tools are available in your environment.
3. **Apply the interactivity/animation mandate** — if the chosen tool supports click-to-reveal, animated sequences, or bound/interactive elements, use them whenever even remotely useful.
4. **Execute** — actually build and open the result; never stop at "here's what I'd draw."

## Using it

This follows the standard [Agent Skills](https://www.anthropic.com/news/agent-skills) format — a `SKILL.md` with YAML frontmatter (`name`, `description`) that any compatible agent (Claude Code, Grok Build, Codex, Hermes, in general, or another skill-aware harness) can discover and load.

Drop `SKILL.md` into your skills directory (e.g. `~/.claude/skills/how-to-illustrate/` or your agent's equivalent) and it activates automatically whenever a request matches its description.

## License

MIT — use it, fork it, adapt the taxonomy and tool router to whatever diagramming tools you have.
