# Evidence First Research

An agent skill for answering questions from documents with citations people can check. It helps an agent resolve conflicting policies, compare reported results, and say which conclusions the sources support.

## Install in Codex

```sh
git clone https://github.com/SergeiMisoian/evidence-first-research.git "$HOME/.agents/skills/evidence-first-research"
```

In Codex, invoke it with `$evidence-first-research`. The skill uses the files and search tools available to your agent. [Codex skill installation](https://developers.openai.com/codex/skills#where-codex-loads-local-skills)

## Try it on sample documents

Open a Codex session in the checkout and paste this request.

```text
$evidence-first-research Using only examples/sources, what was the approved
response target for EU email tickets on May 15, 2026? Explain why two
documents give a different number and cite the relevant passages.
```

The answer should identify the **eight business hour** target, cite the approved
policy, and explain the status of the older policy and the draft target. [Sample checks](examples/evaluation.md)

For your own work, give the agent a question and the documents or source
collection it should use. Include an as-of date if the answer depends on one.

Licensed under the [MIT License](LICENSE).
