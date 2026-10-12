# The Skill-Gap Analyzer

**Understand how your resume aligns with a target role—then identify what to improve next.**

The Skill-Gap Analyzer is a lightweight browser-based tool for comparing resume text with a job description. It surfaces matched skills, highlights gaps, and offers role-aligned suggestions to help make career preparation more focused.

## Features

- Compare resume content against a target job description
- Extract and match technical and professional skills
- Display an overall match score
- Separate matched, recommended, and critical skills
- Generate suggestions for strengthening resume bullets
- Perform analysis in the browser in the current implementation

## Tech stack

- HTML5 and JavaScript
- Vite
- Tailwind CSS

## Quick start

```bash
git clone https://github.com/saikishore2410/The-Skill-Gap-Analyzer.git
cd The-Skill-Gap-Analyzer
npm install
npm run dev
```

Open the local URL printed by Vite.

## Validate and build

```bash
npm test
npm run lint
npm run build
npm run preview
```

Check `package.json` for the authoritative scripts available in the current branch.

## Privacy and limitations

The current implementation runs in the browser and does not send resume/job text to a backend. Match scores are indicators to guide review—not a guarantee of ATS performance or hiring outcomes. Always verify suggested skills and resume statements for accuracy.

## Contributing

Report issues with reproduction steps, and submit focused pull requests with appropriate tests.

## License

No license is specified. Add a `LICENSE` file before granting reuse rights.