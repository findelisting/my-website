# GitHub Pages Setup Guide

## Step 1: Create GitHub Repository
1. Go to github.com and log in
2. Click the "+" icon in the top right → "New repository"
3. Name your repository (e.g., `my-website`)
4. Choose "Public" (required for free GitHub Pages)
5. Check "Add a README file"
6. Click "Create repository"

## Step 2: Push Your Code
```bash
# Initialize git (if not already done)
git init

# Add all files
git add .

# Commit changes
git commit -m "Initial commit"

# Add remote repository (replace with your repo URL)
git remote add origin https://github.com/yourusername/your-repo-name.git

# Push to GitHub
git push -u origin main
```

## Step 3: Configure GitHub Pages
1. Go to your repository on GitHub
2. Click "Settings" tab
3. Click "Pages" in the left sidebar
4. Under "Build and deployment":
   - Source: Select "Deploy from a branch"
   - Branch: Select "main" and folder "/ (root)"
5. Click "Save"

Your site will be live at: `https://yourusername.github.io/your-repo-name/`

## Step 4: Add Custom Domain (GoDaddy)
1. In GitHub Pages settings, under "Custom domain":
   - Enter your domain (e.g., `yourbusiness.com`)
   - Check "Enforce HTTPS"
   - Click "Save"

2. Go to GoDaddy DNS management:
   - Add A record pointing to GitHub's IPs:
     - `185.199.108.153`
     - `185.199.109.153`
     - `185.199.110.153`
     - `185.199.111.153`
   - Add CNAME record for `www` → `yourusername.github.io`

3. Wait for DNS propagation (up to 24 hours)

## Step 5: Verify Deployment
- Check GitHub Pages status in repository settings
- Visit your domain to confirm the site loads
- Test all links and responsiveness

Need help with any specific step?