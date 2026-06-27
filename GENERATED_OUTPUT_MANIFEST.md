# Generated Output Manifest

This manifest documents the major files/pages the builder is expected to emit into a generated school-platform ZIP.

## Always-emitted core files
- `index.html`
- `login.html`
- `dashboard.html`
- `voting.html`
- `notifications.html`
- `about.html`
- `contact.html`
- `manifest.json`
- `sw.js`
- `robots.txt`
- `sitemap.xml`
- `offline.html`
- `README.md`
- `DEPLOYMENT-GUIDE.md`
- `TROUBLESHOOTING.md`
- `.nojekyll`
- `.gitignore`

## Always-emitted asset/runtime files
- `assets/css/style.css`
- `assets/js/config.js`
- `assets/js/app.js`
- `assets/js/notifications.js`
- `assets/js/voting.js`
- `assets/js/pwa-install.js`
- `assets/js/cbt-engine.js`
- `assets/js/analytics.js`
- `assets/js/super.js`
- `assets/js/enterprise.js`
- `assets/js/crud.js`
- `assets/js/site-help.js`
- `assets/img/logo.<ext>`

## Always-emitted database/support files
- `database/schema.sql`
- `database/voting-schema.sql`
- `database/cbt-schema.sql`
- `database/reportcard-schema.sql`
- `database/enterprise-schema.sql`
- `database/enhancements-schema.sql`
- `database/update-v1-schema.sql`
- `database/update-v2-schema.sql`
- `database/update-v4-schema.sql`
- `database/students_import_template.csv`
- `database/sample-questions.csv`
- `students_import_template.csv`

## Always-emitted dedicated feature pages
- `cbt.html`
- `cbt-exam.html`
- `report-cards.html`
- `analytics.html`
- `admin-data.html`
- `approvals.html`
- `admissions.html`
- `apply.html`
- `idcards.html`
- `certificates.html`
- `flyer.html`
- `cbt-prompts.html`
- `entrance.html`
- `storage.html`
- `developer.html`
- `student-profile.html`
- `academic_records.html`
- `academic-records.html`
- `academic_setup.html`
- `timetable-generator.html`
- `checkin.html`
- `diary.html`
- `surveys.html`
- `menu.html`
- `settings.html`

## Module-driven generated pages
These are emitted when selected in the module configuration or treated as core/demo modules in the generator loop.

Representative module ids include:
- `students`
- `staff`
- `classes`
- `subjects`
- `attendance`
- `results`
- `timetable`
- `sow`
- `assignments`
- `library`
- `conduct`
- `health`
- `promotion`
- `fees`
- `finance`
- `leave`
- `visitors`
- `transport`
- `announcements`
- `events`
- `messages`
- `inbox`
- `complaints`
- `broadcast`
- `gallery`
- `eresources`
- `birthdays`
- `reports`
- `directory`
- `departments`
- `parents`
- `hr`
- `payroll`
- `staff_loans`
- `staff_bonus`
- `appraisals`
- `rubrics`
- `transcripts`
- `transfer_cert`
- `counselling`
- `hostel`
- `alumni`
- `inventory`
- `lms`
- `gamification`
- `cafeteria`
- `financial_aid`
- `front_desk`
- `career_counseling`
- `document_builder`
- `fleet_tracking`
- `facility_booking`
- `compliance`
- `activity_log`
- `lesson_plans`
- `behaviour`
- `support_plans`
- `donations`
- `substitutions`
- `helpdesk`
- `payments_online`
- `school_calendar`
- `lost_found`
- `parent_meeting`
- `book_request`
- `digital_library`

## Modern build additions
When `buildType === 'modern'`, the generator also emits:
- `package.json`
- `server.js`
- public-app file moves/copies as defined by generator logic

## Maintainer note
Some files listed here are expected only in generated output and do not necessarily exist in the repository root. See `MAINTAINER_NOTES.md`.
