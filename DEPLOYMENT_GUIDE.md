# GitHub Pages Deployment Guide

## Quick Setup (5 minutes)

### 1. Create Repository
- Go to GitHub and create a new repository
- Name it: `your-username.github.io` (use your actual GitHub username)
- Set to **Public**
- Don't initialize with README

### 2. Upload Files
**Option A: Using GitHub Web Interface**
1. Click "uploading an existing file"
2. Drag and drop all files (`index.html`, `styles.css`, `script.js`, `README.md`)
3. Commit with message: "Initial portfolio website"

**Option B: Using Git Commands**
\`\`\`bash
git clone https://github.com/your-username/your-username.github.io.git
cd your-username.github.io
# Copy your files here
git add .
git commit -m "Add portfolio website"
git push origin main
\`\`\`

### 3. Enable GitHub Pages
1. Go to repository **Settings**
2. Scroll to **Pages** section
3. Source: **Deploy from a branch**
4. Branch: **main**
5. Folder: **/ (root)**
6. Click **Save**

### 4. Access Your Site
Visit: `https://your-username.github.io`

## Important Updates Needed

Before deploying, update these placeholders:

### In `index.html`:
- Replace `#` in social media links with actual URLs
- Update phone number format if needed
- Add your actual LinkedIn, GitHub, Kaggle URLs

### Example Social Links:
\`\`\`html
<a href="https://linkedin.com/in/your-profile" class="social-link">
<a href="https://github.com/your-username" class="social-link">
<a href="https://kaggle.com/your-username" class="social-link">
\`\`\`

## Custom Domain (Optional)

To use a custom domain like `yourname.com`:

1. Buy a domain from any registrar
2. Create a `CNAME` file in your repository with your domain:
   \`\`\`
   yourname.com
   \`\`\`
3. Configure DNS settings with your domain provider:
   - Add CNAME record pointing to `your-username.github.io`
4. Update GitHub Pages settings to use custom domain

## Troubleshooting

**Site not loading?**
- Wait 5-10 minutes after first deployment
- Check that repository is public
- Ensure `index.html` is in root directory

**Changes not showing?**
- Hard refresh browser (Ctrl+F5 or Cmd+Shift+R)
- Check GitHub Actions tab for deployment status
- Clear browser cache

**Mobile not responsive?**
- Ensure viewport meta tag is present
- Test on actual devices, not just browser dev tools

## Performance Tips

1. **Optimize Images**: Compress any images you add
2. **Minimize Files**: The current CSS/JS is already optimized
3. **Use CDN**: Font Awesome and Google Fonts are loaded from CDN
4. **Enable Caching**: GitHub Pages automatically handles this

## Security

- Never commit sensitive information (API keys, passwords)
- Keep repository public for free GitHub Pages
- Use environment variables for any dynamic content

Your portfolio will be live and professional-looking within minutes of deployment!
