# OAuth consent page for the Heron firm Mind

Static login + consent page for Supabase's OAuth 2.1 server, for the Heron firm Mind (Supabase project `heron-core`). Claude (or any MCP client) is sent here during the OAuth flow; the user signs in, approves, and is redirected back with an authorization code.

**Served at:** `https://heron-lab10.github.io/ht-consent/consent` (GitHub Pages, branch `main`, folder `/ (root)`; Pages serves `consent.html` without the extension).

**Supabase (Authentication → OAuth Server):** Site URL = `https://heron-lab10.github.io/ht-consent`, Authorization Path = `/consent`.

**Reuse for another Mind:** change `SUPABASE_URL` and `SUPABASE_ANON_KEY` at the top of the script in `consent.html`.

Test: open `…/consent?authorization_id=test` → login form renders; after sign-in it shows an error for the fake id (expected).
