# GitHub Pages Deployment Guide

Follow these steps to deploy your food brand website to GitHub Pages.

## Prerequisites

- A GitHub account ([Sign up here](https://github.com/join))
- Git installed on your computer ([Download here](https://git-scm.com/downloads))

## Step-by-Step Deployment

### 1. Customize Your Website

Before deploying, make sure to:

- [ ] Replace "Your Food Brand" with your actual brand name in all HTML files
- [ ] Add your product images to the `images/` folder
- [ ] Update product names and descriptions in `index.html` and `products.html`
- [ ] Replace Amazon links with your actual product URLs
- [ ] Update contact information in the footer
- [ ] Customize the About Us page with your brand story

### 2. Create a GitHub Repository

1. Go to [GitHub](https://github.com) and log in
2. Click the **+** icon in the top right corner
3. Select **New repository**
4. Enter a repository name (e.g., `food-brand-website`)
5. Choose **Public** (required for free GitHub Pages)
6. Do NOT initialize with README (we already have files)
7. Click **Create repository**

### 3. Push Your Code to GitHub

Open Terminal (Mac/Linux) or Command Prompt (Windows) and navigate to your project folder:

```bash
cd /Users/abhishsharma/Documents/Abhishek/manas
```

Then run these commands:

```bash
# Initialize git repository
git init

# Add all files
git add .

# Commit files
git commit -m "Initial commit: Food brand website"

# Add your GitHub repository as remote (replace with your actual URL)
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git

# Push to GitHub
git branch -M main
git push -u origin main
```

**Note**: Replace `YOUR-USERNAME` and `YOUR-REPO-NAME` with your actual GitHub username and repository name.

### 4. Enable GitHub Pages

1. Go to your repository on GitHub
2. Click on **Settings** (top menu)
3. In the left sidebar, click **Pages**
4. Under **Source**:
   - Select branch: **main**
   - Select folder: **/ (root)**
5. Click **Save**

### 5. Wait for Deployment

- GitHub will build and deploy your site
- This usually takes 1-5 minutes
- You'll see a green checkmark when it's ready

### 6. Access Your Website

Your website will be available at:

```
https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/
```

For example: `https://johnsmith.github.io/food-brand-website/`

## Custom Domain (Optional)

If you want to use your own domain (e.g., `www.yourfoodbrand.com`):

1. Buy a domain from a registrar (GoDaddy, Namecheap, Google Domains, etc.)
2. In your GitHub repository settings → Pages → Custom domain
3. Enter your domain name
4. In your domain registrar's DNS settings, add these records:
   ```
   Type: A
   Name: @
   Value: 185.199.108.153
   
   Type: A
   Name: @
   Value: 185.199.109.153
   
   Type: A
   Name: @
   Value: 185.199.110.153
   
   Type: A
   Name: @
   Value: 185.199.111.153
   
   Type: CNAME
   Name: www
   Value: YOUR-USERNAME.github.io
   ```

## Updating Your Website

Whenever you make changes:

```bash
# Add changed files
git add .

# Commit changes
git commit -m "Description of changes"

# Push to GitHub
git push
```

GitHub Pages will automatically rebuild and deploy your updated site.

## Troubleshooting

### Site not loading?
- Wait a few more minutes (can take up to 10 minutes)
- Check that GitHub Pages is enabled in Settings → Pages
- Ensure your repository is Public

### Images not showing?
- Check that image files are in the `images/` folder
- Verify image filenames match exactly (case-sensitive)
- Make sure images were committed and pushed to GitHub

### Links not working?
- Ensure all internal links use relative paths (e.g., `about.html` not `/about.html`)
- Check that all HTML files are in the root directory

### CSS not loading?
- Verify `styles.css` is in the root directory
- Check the link tag in HTML files: `<link rel="stylesheet" href="styles.css">`

## Alternative Hosting Options

If you prefer not to use GitHub Pages:

- **Netlify**: Drag and drop deployment, free tier available
- **Vercel**: Similar to Netlify, great for static sites
- **Cloudflare Pages**: Fast CDN, free tier available
- **AWS S3 + CloudFront**: More technical, but very scalable

## Need Help?

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [GitHub Community Forum](https://github.community/)
- [Git Tutorial](https://www.atlassian.com/git/tutorials)

---

Good luck with your food brand website! 🎉

