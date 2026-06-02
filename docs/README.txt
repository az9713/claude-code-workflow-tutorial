https://www.youtube.com/watch?v=9_ExDZFlaNc&t=12s

create you own tutorial
ask CC to go over all sessopm json files

have agent mine 

[
I added a step 0 to use a deterministic script (non llm) to extract just the chat and skill/tool calls from the jsonl logs and it removed 94% of the size and token count to read them, that solved it.
]

look for patterns you use CC
tailor advice

[
Here is the text extracted verbatim from the screen:

I would like you to build a workflow that analyzes all JSONL files in [PASTE YOUR FOLDER PATH HERE - e.g. ./logs or /path/to/your/jsonl/*.jsonl] and produces a single self-contained HTML upgrade guide for moving from Opus 4.7 to Opus 4.8.

The goal is to help me extract maximum value from Opus 4.8 plus dynamic workflows and ultracode, grounded in my actual usage patterns rather than generic advice.

STEP 1 - DATA ANALYSIS

Recursively find and read every .jsonl file in the specified folder. Parse the content thoroughly, then extract and categorize:

Prompting patterns and phrasing I use most often.

Skill invocations: which skills, how they are called, and any success or failure patterns.

Tool uses, with emphasis on computer use, terminal, file operations, browser, and long-running tasks.

Agentic behaviors: multi-step reasoning, subagent usage, verification steps, and error recovery.

Pain points visible in the traces - hallucinations or limitations, especially around honesty, long-horizon tasks, code review, and complex migrations or refactors.

Token usage patterns and session length characteristics.


Repeated workflows or high-value tasks I run frequently.

Be honest and specific. Cite concrete examples from the traces rather than generalizing.

STEP 2 - MODEL COMPARISON (MACRO AND MICRO)

Use the claude-code-guide agent (or its knowledge) as a primary expert source on Claude Code internals. Cross-reference the official Opus 4.8 release notes, system card, and any available documentation on differences between 4.8 and 4.7.

Macro differences to assess: overall judgment, honesty about code flaws, long-horizon agentic performance, native support for dynamic workflows, reliability on complex multi-file tasks, and computer use / browser agent improvements.

Micro differences to assess: changes in tool-calling behavior, prompting patterns that now work better or worse, improvements in self-verification, parallel thinking, error flagging, and handling of large-scale work.

...

STEP 3 - SYNTHESIS AND OUTPUT

Produce one beautiful, self-contained HTML file (no external dependencies except Tailwind via CDN) with these sections:

1. Executive Summary - key takeaways tailored to my usage patterns from the JSONL analysis. Lead with the highest-ROI changes.
2. Usage Profile Analysis - what my data reveals about how I actually use Claude Code: top prompting styles, most-used skills and tools, common workflows, and where 4.7 showed friction.
3. Opus 4.8 vs 4.7 - macro and micro differences, using clear comparison tables plus explanation. Include both general improvements and those most relevant to my traces.
4. Prompting Pattern Upgrades - specific before/after examples based on patterns found in my files, showing improved ways to prompt for the same goals on 4.8.
5. Skill and Tool Recommendations - which skills and tools to use differently, enhance, or combine with dynamic workflows, with concrete examples.
6. Dynamic Workflows / Ultracode Opportunities - specific high-value
cases from my data where I should now use workflow: or /effort
ultracode. Include copy-ready example prompts.
7. Migration Checklist - an actionable, prioritized list of changes to
make across my prompting, skills, projects, and workflows.
8. Advanced Opportunities - creative new ways to use Opus 4.8 plus
dynamic workflows that were impractical on 4.7, especially leveraging
parallel subagents and built-in verification.

HTML REQUIREMENTS

lean, modern, professional design using Tailwind via CDN.

Strong typography and generous spacing.

Collapsible sections or tabs where they aid navigation.

Copy-to-clipboard buttons on every example prompt and code block.

Comparison tables where useful.

Visually highlighted "High Impact" recommendations.

Mobile-friendly, but optimized for desktop reading.

Delivered as a single self-contained file.

TO BEGIN

First confirm the folder path and report the number of JSONL files found. Then proceed with the deep analysis.


]


he said connect to hyperframe
"take this html page and convert it to a short 2-min video on 2x speed"



then distill a skill from this process
/model-migration  skill
for future model migration

get my explainer html and video


=>
but claude-code-guide says
 1. Type: "Run a workflow to [your task]"
  2. Review the script (Ctrl+G to open in editor)
  3. Approve
  4. Monitor with /workflows
  5. Save: in /workflows → select run → press s → save to .claude/workflows/
  6. Reuse: /your-workflow-name via autocomplete


so you can save as workflow - dont need to save as a skill dummy

###


use case 02
deep research Engine

in general no devil advocate

but /deep-research comes with CC
he classify x post as unconfirmed, cut, survives

peer review research

[
Here is the text extracted verbatim from the screen:

I want you to research all the findings on the dynamic workflows feature associated with Opus 4.8. Pull together everything people are actually reporting about it, the real results, the claims, what holds up and what is just hype, things like the 750,000 lines ported in 11 days and the swarms doing audits in hours. As part of the research, use the Apify X scraper to pull the actual X threads people are posting about dynamic workflows and ultracode, so this is grounded in what is really being said and not just web articles. Pitch me the angles you will research first, then fan your agents out across the web and those threads, fact-check every claim so only what genuinely holds up survives, and hand it back as a clean self-contained HTML report with the source on every line, a count of how many claims survived versus got cut, and a short section on anything you could not confirm.


] <-- Apify X scraper

<-- but no workflow keyword

dynamic workflows <-- will this trigger workflow



212 agents !!
###

use 03
ecosystem audit

where your .claude setup is leaking
audit global and project Claude config




agent tell what to fix
overlapping skills
dup skills

design-designer 
use only once


do this once a month

dwf sporadically
deserve token burn


large meaty problems
* research
* validation
