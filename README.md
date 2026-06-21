# Deploying the SnuggleKins site

This folder is a real, working copy of your site (not a Claude preview). Getting
it live takes two free accounts and about ten minutes, no coding or command
line needed — everything below happens in your browser.

## 1. Put this folder on GitHub

1. Go to github.com and create a free account if you don't have one.
2. Click the "+" in the top right → "New repository." Name it something like
   `snugglekins-site`, leave it Public, and click "Create repository."
3. On the new repo's page, click "uploading an existing file" (or drag files
   into the box). Upload every file in this folder, keeping the `src` folder
   structure intact (drag the whole `src` folder in, GitHub keeps the
   structure).
4. Click "Commit changes."

## 2. Deploy it with Vercel

1. Go to vercel.com and sign up — choose "Continue with GitHub" so the two
   are linked automatically.
2. Click "Add New" → "Project."
3. Find and select the `snugglekins-site` repository you just created, then
   click "Import."
4. Vercel will detect this is a Vite project automatically. You don't need to
   change any settings — just click "Deploy."
5. Wait about a minute. You'll get a live URL like
   `snugglekins-site.vercel.app` — that's your real, working site.

From here on, any time you want a change made, I'll update the file in this
chat, you re-upload it to GitHub (replacing the old version), and Vercel
automatically redeploys within a minute or two — no need to repeat the
Vercel setup steps again.

## 3. Test the admin dashboard

Once it's live, go to `your-url.vercel.app/?admin` and log in with the
email and password you created in Supabase → Authentication → Users.
This is the real test — it should work now that it's not running inside
Claude's sandboxed preview.

## Later: a real domain

Once you're happy with everything, Vercel lets you connect your own domain
name (like `snugglekins.co.za`) for free under Project → Settings →
Domains — you'd just need to buy the domain itself from a registrar first.
