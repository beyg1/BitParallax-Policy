# BitParallax Policy Pages

Static policy pages for BitParallax Studio apps, hosted on GitHub Pages.

## Live URLs

| App | Page | URL |
|-----|------|-----|
| CoLedger | Account Deletion | `https://bitparallax.github.io/coledger/account_deletion/` |

## Adding a New App Page

1. Create a directory under the project root named after your app (lowercase, no spaces):

   ```
   mkdir -p <app-name>/<page-name>
   ```

   Example for a privacy policy:
   ```
   mkdir -p myapp/privacy_policy
   ```

2. Add an `index.html` file inside that directory with your page content.

3. Add any assets (icons, images) inside the same directory.

4. Update this README's table with the new URL.

The page will be live at:
```
https://bitparallax.github.io/<app-name>/<page-name>/
```

No build step required — just push the files.

## GitHub Pages Setup Instructions

### Prerequisites
- A GitHub account with a repository named `bitparallax` (or any name you prefer)

### Steps

1. **Initialize git and push to GitHub:**

   ```bash
   cd /home/darth/Playground/BitParallax\ Policy
   git init
   git add .
   git commit -m "Initial commit: CoLedger account deletion page"
   git branch -M main
   git remote add origin https://github.com/bitparallax/bitparallax.github.io.git
   git push -u origin main
   ```

   > If you want the URL `bitparallax.github.io`, the repo **must** be named `bitparallax.github.io`.

2. **Enable GitHub Pages:**
   - Go to your repo on GitHub → **Settings** → **Pages**
   - Under "Source", select **Deploy from a branch**
   - Branch: `main` | Folder: `/ (root)`
   - Click **Save**

3. **Wait a minute** for the first deployment. Your page will be available at:
   ```
   https://bitparallax.github.io/coledger/account_deletion/
   ```

### Custom Domain (Optional)
If you want to use a custom domain like `policies.bitparallax.com`:
1. Add a `CNAME` file to the repo root with your domain
2. Configure DNS at your domain provider
3. Update the domain in GitHub Pages settings