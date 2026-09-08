# Assignment Tracker V5

A simple web-based academic tracker for assignments, deadlines, exams, classes, grades, GPA estimates, recurring work, and project hierarchy.

## V5 changes
- Minimal black-and-white interface.
- Color accents are limited to status and urgency.
- Classes can be added directly from **Classes**.
- Fixed the Supabase error: `null value in column "semester_id" of relation "courses" violates not-null constraint`.
- If a user has no semester yet, adding the first class automatically creates the appropriate Spring, Summer, or Fall semester.
- Uses the supplied Supabase project URL and publishable key in `config.js`.

## Setup
1. Create/open your Supabase project.
2. In Supabase SQL Editor, run `supabase/schema.sql`. If you already ran the earlier schema, run the V4 hierarchy migration at the bottom of that file.
3. Open `config.js` and confirm the Supabase URL and publishable key.
4. Upload the files in this folder to your GitHub repository.
5. Enable GitHub Pages from Settings → Pages → Deploy from branch → `main` → `/ (root)`.

Never put a Supabase `service_role` or secret key in `config.js`.
