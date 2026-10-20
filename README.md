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

In **Settings**, pick an AI service. You can switch at any time.

### Free: Groq (recommended to start)

1. Go to https://console.groq.com/keys and sign up.
2. Click **Create API Key**, give it a name like `kladde`, and copy the key. It starts with `gsk_`.
3. Open your Kladde site, click **Settings**, choose **Groq**, paste the key and click **Save**.

Groq's free plan allows roughly 1,000 requests a day. Long notes and files are shortened before they're sent. Groq can't read photos with the default model, so upload PDF, Word or PowerPoint files instead.

### Free: OpenRouter

1. Go to https://openrouter.ai/settings/keys, sign up and create a key. It starts with `sk-or-`.
2. In Kladde **Settings**, choose **OpenRouter**, paste the key, click **Check key and list models**, pick a model, and click **Save**.

Free models allow about 50 requests a day (more if you've ever bought $10 of credit).

### Paid: Claude (best quality)

1. Go to https://console.anthropic.com and sign in or sign up. This is separate from your normal Claude subscription.
2. Click **Billing** and add some credit (for example $5). Each AI action usually costs well under one cent with Sonnet, less with Haiku.
3. Click **API keys**, then **Create key**. Give it a name like `kladde` and copy the key. It starts with `sk-ant-`.
4. Open your Kladde site, click **Settings**, choose **Claude**, paste the key into **API key** and click **Save**.

Claude reads PDFs (including scans) and photos directly and handles long files.

If your key ever leaks, delete it in the Anthropic Console and make a new one.

## Sync between devices

Kladde can keep the same notes, exercises and words on your laptop and phone. They're saved in a **private** GitHub repository that only you can see, one file per profile.

### 1. Make a private repository (once)

1. On GitHub, click **+** in the top right corner, then **New repository**.
2. Name it `kladde-data`, choose **Private**, and click **Create repository**.

### 2. Make a GitHub key (once)

1. Go to https://github.com/settings/personal-access-tokens/new
2. **Token name:** `kladde`. **Expiration:** pick the longest option. When it runs out, make a new key the same way and paste it into Kladde again.
3. **Repository access:** choose **Only select repositories**, then pick **kladde-data**.
4. **Permissions:** under repository permissions, give **Contents** the access **Read and write**.
5. Click **Generate token** and copy the key. It starts with `github_pat_`. You only see it once.

The key can only read and change `kladde-data`, nothing else in your GitHub account.

### 3. Connect each device

1. Open your Kladde site and click **Settings**.
2. Under **Sync between devices**, paste the key into **GitHub key**. Leave **Private repository** empty, Kladde fills it in.
3. Click **Connect**.

Do the same on your phone with the same key. After that, changes sync by themselves a few seconds after you make them, and when you come back to the page. The header shows "Synced" with the time.

### Profiles

Click the profile name in the header (it starts as **Main**) to add a profile or switch between them. Each profile has its own notes, exercises and Vocab bank. With sync on, every profile is synced, and a profile you add on one device shows up on the others.

## Changing the app later

To update the app, open `index.html` in your repository on GitHub, click the pencil icon to edit (or upload a new version the same way as step 4 and 5), and click **Commit changes**. The site updates within a couple of minutes.
