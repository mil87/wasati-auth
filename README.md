# Wasati: email confirmed

The page Supabase shows after someone opens the link in a Wasati
confirmation email, in the look of the app's welcome screen. It is static
and sends nothing anywhere: no analytics, no referrer, and the address is
cleared as soon as it loads.

- `index.html` and `auth-callback/index.html`: the page. Sign-ups since
  27 November 2026 return to `/auth-callback`.
- `.well-known/assetlinks.json`: makes `/auth-callback` a verified link for
  the Wasati app on Android, so on the phone that made the account the link
  opens Wasati and signs the person in.
- `email/header.png`: the header picture of Wasati's account emails.

Its source is kept in the Wasati repository at `tool/auth_confirmed_page`
(built by `src/build.py`).
