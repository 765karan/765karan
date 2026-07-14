# How to Set Up Your GitHub Profile README

This zip contains everything you need:
- `README.md` — your profile README
- `.github/workflows/snake.yml` — GitHub Action that auto-generates the snake contribution animation at the bottom of your README

## Step 1: Create the special profile repository

1. Go to https://github.com/new
2. Repository name: **765karan** (must match your GitHub username *exactly*, case-sensitive)
3. Set it to **Public**
4. Check **"Add a README file"**
5. Click **Create repository**

GitHub will detect the repo name matches your username and automatically show its README on your profile page.

## Step 2: Upload the files

**Option A — Using the GitHub website (no Git needed)**
1. Open your new `765karan` repo
2. Click **Add file → Upload files**
3. Drag in `README.md` (this replaces the default one — confirm overwrite)
4. For the snake animation, create the folder path manually: click **Add file → Create new file**, type `.github/workflows/snake.yml` as the filename (GitHub auto-creates the folders), then paste the contents of `snake.yml`
5. Commit both changes directly to the `main` branch

**Option B — Using Git on your computer**
```bash
# unzip the folder first, then:
cd 765karan-profile
git init
git remote add origin https://github.com/765karan/765karan.git
git add .
git commit -m "Set up profile README"
git branch -M main
git push -u origin main
```

## Step 3: Let the snake animation generate

1. In your repo, go to the **Actions** tab
2. You should see the "Generate Snake Animation" workflow — click it, then **Run workflow** to trigger it manually the first time
3. Once it finishes (takes ~1 min), it creates a new branch called `output` with the generated SVGs
4. Your `README.md` already points to this file, so it will render automatically once the branch exists

> If the Action fails with a permissions error: go to **Settings → Actions → General → Workflow permissions**, select **Read and write permissions**, and save. Then re-run the workflow.

## Step 4: Check your profile

Visit `https://github.com/765karan` — your new README should now be live on your profile page.

## Step 5 (optional): Personalize further

- Add a portfolio/website badge once you have a live site — just add another shields.io badge line next to LinkedIn/Email
- Swap the top banner GIF for your own if you want something more personal
- Pin your top 4-6 repos on your profile (Customize your pins on the main GitHub profile page) so the "Featured Projects" links match what's pinned
- Make sure the `safeher-app`, `Google-Search-Trend-Analysis`, `Zomato-Data-Analysis`, and `study-group-finder` repos are public — otherwise their stat cards won't render

That's it — your profile is live!
