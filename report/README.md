# SWE-420 Internship Report — FlowGenX AI

LaTeX source for **Md. Rakibul Kabir**'s internship report.
Reg. No. **2020831051** · Dept. of Software Engineering, IICT, SUST.

## Project layout

```
report/
├── main.tex                    ← entry point — compile this
├── preamble.tex                ← packages, fonts, headers, hyperlinks
├── chapters/
│   ├── titlepage.tex
│   ├── acknowledgement.tex
│   ├── executive_summary.tex
│   ├── introduction.tex            ← Chapter 1
│   ├── company_profile.tex         ← Chapter 2
│   ├── methodology.tex             ← Chapter 3
│   ├── internship_activities.tex   ← Chapter 4 (the biggest)
│   ├── skills.tex                  ← Chapter 5
│   ├── life.tex                    ← Chapter 6
│   ├── conclusion.tex              ← Chapter 7
│   └── references.tex
├── extra/
│   ├── transmittal.tex             ← Letter of Transmittal
│   └── endorsement.tex             ← Letter of Endorsement template
└── figures/
    ├── sust.png
    └── screenshots/
        ├── APP_gallery.jpg
        ├── Auth_config.jpg
        ├── Connected_apps.jpg
        ├── MCP_playground.jpg
        ├── landing_page_dashboard.jpg
        ├── paricular_connector_endpoint_test.jpg
        └── workflow_editor.jpg
```

## How to compile

Easiest path on Windows: install **MiKTeX** + **TeXworks** (or use
**Overleaf** as a hosted alternative).

```bash
cd report
pdflatex main.tex
pdflatex main.tex   # second pass for ToC & cross-references
pdflatex main.tex   # third pass to settle list of figures
```

Or with `latexmk` (preferred — handles passes automatically):

```bash
cd report
latexmk -pdf main.tex
```

## What's already filled in

- All seven chapters with substantial content drawn from:
  - The senior LaTeX template (Ashrafur, Orbitax 2025).
  - The senior PDF template (Mehrajul, Vivasoft 2025).
  - FlowGenX public website (about, /, /FAQ, /usecases).
  - Internal repos at `D:\FlowGenX.AI\` (READMEs + `CLAUDE.md`).
  - The git-history work report.
  - The internship offer letter.
- Front matter (title page, transmittal, endorsement, acknowledgement,
  exec summary).
- 7 platform UI screenshots referenced as figures (Chapters 2–4).
- References / bibliography list.

## Open `TODO`s in the source — search the `.tex` files for `TODO`

These are the items waiting on input from the FlowGenX CEO (Sumon Bhai)
or from your own confirmation:

1. **Title page** — replace the FlowGenX logo placeholder with a real
   logo file at `figures/flowgenx_logo.png`.
2. **Endorsement letter** (`extra/endorsement.tex`) — confirm the
   signer (CEO / supervisor / team lead) and update name and
   designation.
3. **Chapter 2** — fill in: founding year, employee count globally,
   number of engineers in Bangladesh, registered entity status in
   Bangladesh, funding stage.
4. **Chapter 2** — confirm the list of FlowGenX functional teams
   beyond Engineering (Product, GTM/Sales, Customer Success, etc.).
5. **Chapter 3** — confirm formal methodology name (Agile / Scrum /
   Kanban / hybrid), sprint cadence, release cadence, hotfix
   process, exact CI/CD platform, environment names (dev/staging/prod),
   and the code-review approval policy (number of reviewers required).

After each `TODO` resolution, search the file for the matching `TODO`
comment and replace the surrounding placeholder paragraph.

## Approximate length

Roughly **55–70 pages** once compiled, depending on figure sizing and
font settings. Within the 50–80 page band typical of SUST IICT
internship reports.

## Source materials this report was built from

- `resource/My_company_flowgenx.ai/flowgenx.ai.md`
- `resource/My_company_flowgenx.ai/my-work-from-git-history-report.md`
- `resource/My_company_flowgenx.ai/Rakibul_Intern_Offer_Letter.pdf`
- `resource/My_company_flowgenx.ai/Connectors_List_Native_Connector.csv`
- `resource/My_company_flowgenx.ai/Images/*.jpg`
- `resource/others_reports/2019831070_InternshipReportSWE420/` (LaTeX template by Ashrafur)
- `resource/others_reports/2019831074_Mehrajul_Islam.pdf` (Vivasoft report)
- `D:\FlowGenX.AI\runtime_connectivity\README.md` and `CLAUDE.md`
- `D:\FlowGenX.AI\runtime_apis\README.md`
- `D:\FlowGenX.AI\runtime_components\README.md`
- Cached pages from `https://www.flowgenx.ai/` (about, /, /FAQ, /usecases)
