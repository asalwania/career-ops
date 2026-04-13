# Career-Ops

AI-powered job search pipeline built on Claude Code. Evaluates job offers, generates tailored CVs, scans portals, and tracks applications.

## Setup

```bash
git clone https://github.com/asalwania/career-ops.git
cd career-ops && npm install
npx playwright install chromium

cp config/profile.example.yml config/profile.yml
cp templates/portals.example.yml portals.yml
# Create cv.md with your CV in markdown
```

## Usage

Open Claude Code in this directory, then use the `/career-ops` command:

```
/career-ops                → Show all commands
/career-ops {paste a JD}   → Full pipeline: evaluate + PDF + tracker
/career-ops scan           → Scan portals for new offers
/career-ops pdf            → Generate ATS-optimized CV
/career-ops batch          → Batch evaluate multiple offers
/career-ops tracker        → View application status
/career-ops pipeline       → Process pending URLs
/career-ops apply          → Fill application forms with AI
/career-ops contacto       → LinkedIn outreach message
/career-ops deep           → Deep company research
/career-ops patterns       → Analyze rejection patterns
/career-ops followup       → Follow-up cadence tracker
```

Or just paste a job URL or description directly — career-ops auto-detects it and runs the full pipeline.

## License

MIT
