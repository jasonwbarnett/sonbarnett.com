# Jason Barnett Consulting Website

Professional consulting services website for software architecture, infrastructure, and CI/CD expertise.

## Deployment to GitHub Pages

### Initial Setup

1. Create a new GitHub repository (e.g., `sonbarnett.com`)

2. Initialize git and push your code:
   ```bash
   git init
   git add .
   git commit -m "Initial commit: consulting website"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/sonbarnett.com.git
   git push -u origin main
   ```

3. Configure GitHub Pages:
   - Go to your repository settings
   - Navigate to "Pages" section
   - Under "Source", select "Deploy from a branch"
   - Select "main" branch and "/ (root)" folder
   - Click "Save"

4. Configure custom domain (optional):
   - In the same Pages settings, enter your custom domain: `ja.sonbarnett.com`
   - Create a `CNAME` file in your repository root with the domain
   - Configure your DNS with a CNAME record pointing to `YOUR_USERNAME.github.io`

### DNS Configuration for Custom Domain

Add the following DNS records to your domain provider:

```
Type: CNAME
Name: ja
Value: YOUR_USERNAME.github.io
```

### Local Development

Simply open `index.html` in your browser to preview the site locally.

## Features

- Clean, professional design using Tailwind CSS
- Responsive layout (mobile-friendly)
- Email spam protection (click to reveal)
- Smooth scrolling navigation
- Fast loading (no build process required)

## Technologies

- HTML5
- Tailwind CSS (via CDN)
- Vanilla JavaScript

## Updates

To update the website, simply edit `index.html` and push your changes:

```bash
git add .
git commit -m "Update content"
git push
```

GitHub Pages will automatically deploy your changes within a few minutes.
