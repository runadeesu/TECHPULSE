# Supabase setup

The connected Supabase project already has the anonymous forum schema applied.

For a fresh Supabase project:
1. Apply `migrations/0001_anonymous_forum.sql`.
2. Keep Row Level Security enabled.
3. Set the project URL and publishable key in `assets/config.js`.
4. Supabase Auth is not required for the forum.
5. Public visitors can read and create posts/replies; public update/delete is intentionally disabled.
6. Use trusted admin tooling to moderate rows with `is_hidden`.
