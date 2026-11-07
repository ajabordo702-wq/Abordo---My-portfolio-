ANTHONY JAMES ABORDO - PORTFOLIO WITH ADMIN UPLOAD
===================================================

FILES
- index.html: public portfolio
- admin.html: private login + upload/delete dashboard
- style.css: responsive design
- script.js: public activity gallery
- supabase-config.js: add your Supabase Project URL + anon/publishable key
- supabase-setup.sql: database + Storage + access policies

SUPABASE SETUP (PHONE OR COMPUTER)
1. Open your Supabase project dashboard.
2. Open SQL Editor > New query.
3. Open supabase-setup.sql from this package, copy all SQL, paste into SQL Editor, and Run.
4. In Supabase Project Settings > API (or API Keys), copy the Project URL and anon/public or publishable key.
5. Open supabase-config.js in your GitHub repository and replace the two placeholder values. Use ONLY the anon/public/publishable key. NEVER use service_role or secret keys in website code.
6. In Supabase Authentication > Users, create your admin user (your email and a strong password). Disable public sign-ups in Authentication settings so strangers cannot create accounts.
7. In Authentication > URL Configuration, add your GitHub Pages website URL to Site URL and Redirect URLs if required.
8. In GitHub Pages, ensure your site is deployed from main / (root).

HOW TO USE
1. Open your website and tap Admin in the navigation, or visit /admin.html.
2. Sign in using the admin email/password you created in Supabase.
3. Add title, category, description, choose an image or PDF (up to 10 MB), then tap Upload and publish.
4. The item appears on your public portfolio. You can delete published activities from the admin page.

SECURITY NOTES
- The website uses the public anon/publishable key, protected by Row Level Security policies in the SQL.
- Never expose a Supabase service_role or secret key in GitHub or browser code.
- This setup grants upload/delete to authenticated users. Disable public signups and create only your own admin account.
- Files are public so visitors can open published portfolio activities. Do not upload private or sensitive documents.
- If you later need multiple admins or stricter role-based permissions, add a dedicated admin allow-list policy.
