# Wasati: email confirmed

The page Supabase shows after someone opens the link in a Wasati confirmation
email. It is static and sends nothing anywhere: no analytics, no referrer, and
any sign-in tokens in the address are removed as soon as it loads. Its source
is kept in the Wasati repository at `tool/auth_confirmed_page/index.html`.
