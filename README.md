# KubeDesk Pro App Store Pages

This directory contains the GitHub Pages site for KubeDesk Pro's privacy policy and copyright information, required for App Store submission.

## 📁 Files

- **index.html** - Landing page with app overview
- **privacy.html** - Privacy Policy (required by App Store Connect)
- **copyright.html** - Copyright & Legal Information

## 🚀 Publishing to GitHub Pages

### 1. Create a New Public Repository

```bash
# Create a new repo on GitHub (e.g., kubedesk-legal or kubedesk-pages)
# Then:
cd appstore
git init
git add .
git commit -m "Initial commit: Privacy policy and copyright pages"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
git push -u origin main
```

### 2. Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** → **Pages**
3. Under **Source**, select:
   - Branch: `main`
   - Folder: `/ (root)`
4. Click **Save**
5. Wait a few minutes for deployment

### 3. Your URLs

After GitHub Pages is enabled, your pages will be available at:

```
https://YOUR_USERNAME.github.io/YOUR_REPO/
https://YOUR_USERNAME.github.io/YOUR_REPO/privacy.html
https://YOUR_USERNAME.github.io/YOUR_REPO/copyright.html
```

### 4. Add URLs to App Store Connect

In App Store Connect, add these URLs:

- **Privacy Policy URL**: `https://YOUR_USERNAME.github.io/YOUR_REPO/privacy.html`
- **Copyright**: Add the copyright page URL in the app description or legal section

## 🎨 Customization

### Update Contact Email

The pages currently use placeholder emails:
- `admin@kubedesk.app`

**Find and replace** these with your actual contact email in:
- `privacy.html` (line ~210)
- `copyright.html` (line ~245)

### Update Company/Developer Name

If you want to use a different company name instead of "KubeDesk Pro", update:
- Copyright notices: `© 2024 KubeDesk Pro`
- Company references throughout the pages

### Update Helper Repository Link

The copyright page references:
```
https://github.com/kubedeskpro/kubedesk-helper
```

Make sure this matches your actual helper repository URL.

## 📝 Maintenance

### Update Last Modified Date

When you make changes, update the "Last Updated" date in:
- `privacy.html` (line ~99)
- `copyright.html` (line ~117)

### Keep Privacy Policy Current

Review and update the privacy policy if you:
- Add new features that access user data
- Integrate third-party services
- Change data handling practices

## ✅ Checklist for App Store Submission

- [ ] Create public GitHub repository
- [ ] Push these files to the repository
- [ ] Enable GitHub Pages
- [ ] Verify pages are accessible via HTTPS
- [ ] Update contact emails in both pages
- [ ] Add Privacy Policy URL to App Store Connect
- [ ] Test all links work correctly

## 🔗 Recommended Repository Names

- `kubedesk-legal`
- `kubedesk-pages`
- `kubedesk-privacy`
- `kubedesk-appstore`

Choose a short, memorable name for cleaner URLs.

## 📧 Support

If you need to update these pages after App Store submission, just commit changes to the repository and GitHub Pages will automatically redeploy within a few minutes.

