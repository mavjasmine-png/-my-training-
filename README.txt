PHASE 3 — PUBLICATION PACKAGE v3.2.0

START HERE
index.html is the app. programme.html is the complete readable programme.
review.html contains the critique, changes, test evidence and limitations.
All supplied files are at the ZIP root to simplify iPhone file uploads.

UPDATE YOUR EXISTING GITHUB PAGES WEBSITE
1. Open the old training app and export its backup before updating.
2. Save this ZIP in Files and tap it to extract it.
3. In Safari, open your existing GitHub training repository.
4. Add file > Upload files. Select the extracted FILES, not the ZIP or outer folder.
5. Upload/replace the supplied files, keeping index.html at repository root.
6. Commit changes. If Pages is already enabled, wait for deployment.
7. Otherwise Settings > Pages > Deploy from a branch > main > / (root) > Save.
8. Open the existing HTTPS website address. Close old app tabs/windows and reopen
   to let a newly installed service worker activate. Do not clear browser storage
   as a routine update step; doing so can erase your records.
9. Safari > Share > Add to Home Screen. Open once online and check More for
   the offline-cache status. Then test loading in airplane mode.

No build command, npm install, external font, API key, login or paid backend is
required. Any HTTPS static host that serves the files unchanged is suitable.
GitHub Pages settings/account availability are controlled by GitHub.
GitHub's native iPhone app does not offer the full website-file upload workflow;
use Safari for the upload and Pages settings.

DATA
New records use phase3-training-v2 local storage. The previous phase3-state-v1
key is not deleted. When present on the same browser/origin, earlier data is
retained as a separate exportable archive. Old backup JSON can also be imported
as an archive. Do not assume old raw strings can become accurate per-set logs.

A backup import replaces active data after an explicit confirmation step.
Export your current records first. Data does not sync between devices, domains,
browser profiles, Safari and an installed Home Screen app. Export/import when
moving environments. No personal training logs are included in this package.

ONE SESSION PER DAY SLOT PER WEEK
You can train the named session on another date and edit its date. The app keeps
one session per named slot per block/week; it does not create unlimited sessions
for the same slot. Reopen a session to correct it. Old blocks remain in history.

EIGHT-WEEK BEHAVIOUR
The week, effort targets and deload are automatic. After day 56 the app displays
a review prompt. It does not automatically generate or deploy new exercises.
Starting another block repeats the same programme and retains history.

OFFLINE / TIMER
A secure HTTPS host is needed for service workers (except local development).
The new service worker waits until old app windows close before activating.
Core assets are cached together. New releases must use a new cache version.
iOS may suspend timers when locked or backgrounded. The clock catches up on
return, but no background alarm is guaranteed.

FINAL ON-DEVICE ACCEPTANCE
Check iPhone Home Screen install; offline launch; keyboard/numeric entry;
export and import via Files; saved data after closing/reopening; timer in
foreground; safe-area spacing and VoiceOver labels. These cannot be certified
by the desktop Chromium viewport checks performed here.

DEVELOPER CHECK
node verify.cjs
No packages needed; uses Node's standard library (Node 18+).
Tests are optional for hosting. verify.cjs is not loaded by the website.
