# Maintainer Notes

## Important: some files exist only in generated output

This repository is both:
1. the public marketing/builder site, and
2. the source blueprint for generated school-platform ZIPs.

Because of that, some files referenced in templates and generator logic are not expected to exist as root repository files.

### Example: `assets/js/app.js`
`assets/js/app.js` is generated at ZIP-build time by `Generator.appJS(cfg)` in:
- `assets/js/generator.js`

So if you do not see `assets/js/app.js` in the repository root, that is expected.
It exists in generated output, not as a source-controlled root file.

### Other generated pages
The builder also generates many pages dynamically, including examples such as:
- `login.html`
- `contact.html`
- `apply.html`
- `cbt-exam.html`
- `report-cards.html`
- `analytics.html`
- `admin-data.html`
- `approvals.html`
- `admissions.html`
- `idcards.html`
- `certificates.html`
- `developer.html`
- `student-profile.html`
- `academic_setup.html`
- `academic_records.html`
- `timetable-generator.html`
- `checkin.html`
- `diary.html`
- `surveys.html`
- `menu.html`
- `settings.html`

## Dedicated page safety
When a module has a dedicated page builder in `assets/js/generator.js`, ensure its module id is also protected in the `DEDICATED` list so the generic module generator does not overwrite it.

## Recommended workflow
- Edit templates and generator logic in source
- Run validation scripts before packaging
- Produce ZIPs from the builder/generator path, not by assuming repo-root parity for all generated files
