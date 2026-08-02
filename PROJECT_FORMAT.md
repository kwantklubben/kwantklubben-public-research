# Approved public project format

Projects in this repository are copied from the private research repository only after explicit publication approval.

Each published folder contains:

```text
projects/<slug>/
  README.md
  project.json
  ...approved supporting files...
```

`project.json` fields:

```json
{
  "title": "Project title",
  "question": "One-line question",
  "tags": ["research"],
  "status": "PASS",
  "summary": "Short result or limitation",
  "author": "GitHub username",
  "date": "2026-01-01",
  "source": "https://github.com/alfredbirkelund/kwantklubben-research/tree/main/projects/example"
}
```

The website consumes the root `projects.json` index. The repository remains the public source of truth for published project files.
