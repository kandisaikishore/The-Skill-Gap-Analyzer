# Development and Evaluation Guide

The Skill-Gap Analyzer compares a current skill profile with target-role requirements. Verify the actual scoring and recommendation implementation before describing a feature as available.

## Setup

```bash
git clone https://github.com/kandisaikishore/The-Skill-Gap-Analyzer.git
cd The-Skill-Gap-Analyzer
```

Use the runtime, dependency manager, and commands declared by the repository manifests. Keep API keys and personal career profiles out of version control.

## Input normalization

For implemented assessment flows, test missing, empty, duplicated, differently cased, and whitespace-padded skill names. Define whether synonyms are normalized and document that behavior. Reject malformed input with actionable feedback rather than silently treating it as a valid profile.

## Scoring and explainability

- Document the actual inputs and weights used by the scoring algorithm.
- Ensure identical normalized inputs produce deterministic results.
- Explain which target-role requirements contribute to each reported gap.
- Do not invent role requirements or imply that a recommendation guarantees employment.
- Test ties, empty profiles, and targets with no requirements.

## Privacy

Career profiles may include personal and employment information. Minimize collection, avoid logging full profiles by default, and explain persistence and deletion behavior based on the implementation.

## Pull-request checklist

- [ ] Add deterministic tests for normalization and score boundaries.
- [ ] Run the declared test/build commands.
- [ ] Verify explanations are traceable to input evidence.
- [ ] State any checks that could not be run.
- [ ] Keep planned functionality separate from implemented functionality.
