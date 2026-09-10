# tm-catalog

**Generated. Do not edit by hand.** This public repo is the machine-readable course catalog that
[techmonster.dev](https://techmonster.dev) renders: every specialization track, its phases and projects,
and the published video lessons that belong to each project.

- `catalog.json` — every track (summary) + explainer video series + totals
- `tracks/<id>.json` — one track in full: phases → projects (title, description, tech, `video` when a lesson is published)

It is written by `Export-PublicCatalog.ps1` in the private `techmonster-dev/setup-automation` engine:
after a track is authored/updated (`Import-AuthoredProjects.ps1 -Push`), after the video pipeline's
morning run publishes new lessons, and daily by `tm-cohort-control/.github/workflows/export-catalog.yml`.
A leak guard refuses to publish rubrics, viva questions, grader signals or email addresses.

Raw URLs: `https://raw.githubusercontent.com/techmonster-dev-org/tm-catalog/main/catalog.json`
