# Upload this project to GitHub

1. Open https://github.com/new and sign in.
2. Use repository name `mikrotik-rb2011-home-network`, optionally add a description, and choose Public or Private.
3. **Do not** tick "Add a README", .gitignore or license (they are supplied in this project).
4. Click **Create repository**.
5. On the empty repository page choose **uploading an existing file** (or **Add file → Upload files** if shown).
6. On your computer, **extract the ZIP**. Open the extracted `mikrotik-rb2011-home-network` folder and upload `README.md`, `GITHUB_UPLOAD_GUIDE.md`, `.gitignore` and **the entire `images` folder**. Preserve the `images/` paths, or the README pictures will not render. GitHub's browser uploader may not include hidden `.gitignore` from drag-and-drop; add it later if necessary. If the browser flattens your images, use GitHub Desktop or the `git` commands below instead.
7. Enter a commit message such as `Document MikroTik router, PPPoE and Tenda AP setup` and click **Commit changes**.
8. Return to the repo landing page and verify the README and image links display.

## Reliable alternative: Git in Terminal

In Terminal, open the **extracted repository folder**, then run:

```bash
git init
git add README.md GITHUB_UPLOAD_GUIDE.md .gitignore images/
git commit -m "Document MikroTik RB2011 and Tenda Wi-Fi setup"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/mikrotik-rb2011-home-network.git
git push -u origin main
```

Create an **empty** repository on GitHub first, and replace `YOUR-USERNAME` with your actual username. You must authenticate with GitHub when prompted (for HTTPS, GitHub uses a credential manager or token rather than an account password).

## Security

The screenshots in `images/` have identifying values redacted where needed. Never upload the original unredacted PPPoE Dial Out screenshot, router configuration exports, admin passwords, or credential backups. Rotate the exposed PPPoE password through your ISP.
