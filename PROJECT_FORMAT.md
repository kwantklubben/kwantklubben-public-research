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

The index may also contain curated flagship entries (e.g. the Kwant Atlas) that have their own repo/site and are not published research. They always sort first and are marked `"featured": true` with an external `source`.

On the site, each card links its `source` as a whole (the entire card is the link). A project's `status` drives its verdict sticker: `Flagship`, `Paper`/`Live`, or `Killed` each render as a stamp. `authors` is a list of GitHub usernames, shown as `@username` in the card footer.
