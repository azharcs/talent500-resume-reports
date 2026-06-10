# Talent500 Resume Reports

Static HTML resume report delivery platform, hosted on GitHub Pages.

## How it works

Each candidate gets a unique URL:
```
https://YOUR_ORG.github.io/talent500-resume-reports/reports/firstname-lastname.html
```

The root URL (`/`) shows a neutral landing page — not a candidate report.

## Adding a new report

1. Generate the report HTML (AI-generated, recruiter-reviewed)
2. Save it to `/reports/firstname-lastname.html`
3. Commit and push — live within ~60 seconds

```bash
git add reports/firstname-lastname.html
git commit -m "Add resume report: Firstname Lastname"
git push
```

## Folder structure

```
/
├── index.html              ← neutral landing page
├── README.md
├── CHECKLIST.md
└── reports/
    └── aakash-gaurav.html  ← example report
```

## Edit mode

Each report has built-in Edit Mode. Open in browser → click "Edit Report" → make changes → click "Publish" → replace the file → push.

## Deployment

GitHub Pages: Settings → Pages → Source: Deploy from branch → main → / (root)
