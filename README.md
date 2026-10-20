# Kladde

A Danish study notebook with a Claude AI tutor. Write lesson notes, check your grammar, translate, collect vocabulary and get quizzed.

Everything is in one file, `index.html`. There is nothing to install.

## Where things are saved

- **Your notes and vocabulary** are saved in the browser you use (Chrome, Edge, Safari...). They don't sync between devices. Use **Settings > Download backup** now and then, and **Restore from backup** to move them to another computer.
- **Your Claude API key** is also saved only in your browser. It is never put on GitHub, and it is only sent to Anthropic.

## Put it online with GitHub Pages

You only do this once. It takes about 10 minutes.

1. Go to https://github.com and sign in (or click **Sign up** to make a free account).
2. In the top right corner, click the **+** button, then **New repository**.
3. In **Repository name**, type `kladde`. Leave it set to **Public**. Don't tick anything else. Click **Create repository**.
4. On the next page, find the line that says "...or **uploading an existing file**" and click that link.
5. Drag `index.html` and `README.md` from your computer into the browser window. Wait until both show in the list, then click the green **Commit changes** button.
6. Click the **Settings** tab at the top of your repository (the one with the gear icon).
7. In the menu on the left, click **Pages**.
8. Under **Build and deployment**, set **Source** to **Deploy from a branch**. Under **Branch**, choose **main** and **/ (root)**, then click **Save**.
9. Wait 1 to 2 minutes, then refresh the page. A box at the top will show your web address. It looks like `https://YOUR-USERNAME.github.io/kladde/`. Click **Visit site**.

Bookmark that address. That's your app.

## Turn on the AI tutor

1. Go to https://console.anthropic.com and sign in or sign up. This is separate from your normal Claude subscription.
2. Click **Billing** and add some credit (for example $5). Each AI action usually costs well under one cent with Sonnet, less with Haiku.
3. Click **API keys**, then **Create key**. Give it a name like `kladde` and copy the key. It starts with `sk-ant-`.
4. Open your Kladde site, click **Settings**, paste the key into **API key** and click **Save**.

If your key ever leaks, delete it in the Anthropic Console and make a new one.

## Changing the app later

To update the app, open `index.html` in your repository on GitHub, click the pencil icon to edit (or upload a new version the same way as step 4 and 5), and click **Commit changes**. The site updates within a couple of minutes.
