# 🚀 GitHub Profile Setup Instructions

Follow these 4 simple steps to set up your newly generated GitHub profile & automated metrics dashboard!

---

### Step 1: Create Your Profile Repository
1. Log in to [GitHub](https://github.com).
2. Create a **New Repository**.
3. Name the repository **`mohammed123-code`** (it MUST match your exact username).
4. Set visibility to **Public**.
5. Check **Initialize this repository with a README** (if asked).

---

### Step 2: Generate a GitHub Personal Access Token (PAT)
To allow `lowlighter/metrics` to pull your stats automatically, you need a access token:

1. Go to **GitHub Settings** -> **Developer Settings** -> **Personal Access Tokens** -> **Tokens (classic)** (or click [here](https://github.com/settings/tokens)).
2. Click **Generate new token (classic)**.
3. Name/Note: `GitHub Metrics Profile Token`.
4. Expiration: Select `No expiration` or `90 days`.
5. Check the following scopes:
   - `repo` (Full control of private/public repositories)
   - `read:user`
   - `user:email`
6. Click **Generate token** and **copy the token immediately** (you won't be able to see it again).

---

### Step 3: Add Secret to Your Repository
1. Go to your new `mohammed123-code` repository page on GitHub.
2. Go to **Settings** -> **Secrets and variables** -> **Actions**.
3. Click **New repository secret**.
4. Set **Name**: `METRICS_TOKEN`
5. Set **Secret**: Paste the token you copied in Step 2.
6. Click **Add secret**.

---

### Step 4: Upload the ZIP Files to Your Repository
1. Extract this `.zip` file on your computer.
2. In your `mohammed123-code` repo, upload or push:
   - `README.md` to the root folder.
   - `.github/workflows/metrics.yml` into `.github/workflows/`.
3. Commit and push the changes to GitHub.
4. Go to the **Actions** tab in your repository, click on **Metrics**, and click **Run workflow** -> **Run workflow** to generate your first `github-metrics.svg` graphic manually!

Once the workflow finishes running, refresh your GitHub profile page—your custom profile dashboard and stats will be live! 🎉
