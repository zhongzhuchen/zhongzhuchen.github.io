# How to Preview Your Website

## Quick Start (Recommended)

The easiest way to preview your website is to deploy it to GitHub Pages:

### Step 1: Commit your changes
```bash
git commit -m "Initial commit: Single-page personal website"
```

### Step 2: Push to GitHub
```bash
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages
1. Go to https://github.com/zhongzhuchen/zhongzhuchen/settings/pages
2. Under "Source", select "Deploy from a branch"
3. Select branch: `main` and folder: `/ (root)`
4. Click "Save"

### Step 4: View Your Site
After 1-2 minutes, your site will be live at:
**https://zhongzhuchen.github.io/**

## Making Changes

After the initial deployment, any changes you push will automatically rebuild and update the site:

```bash
# Edit files...
git add .
git commit -m "Update content"
git push
```

Wait 1-2 minutes and refresh your browser to see the changes.

## Local Preview (Advanced)

If you want to preview locally before pushing, you have two options:

### Option A: Using Docker
```bash
docker-compose up
# Visit http://localhost:4000
```

### Option B: Using rbenv (Ruby version manager)
```bash
# Install rbenv first
brew install rbenv

# Install Ruby
rbenv install 3.1.0
rbenv local 3.1.0

# Install dependencies
bundle install

# Run Jekyll
bundle exec jekyll serve

# Visit http://localhost:4000
```

## Current Status

Your website is ready to deploy! All content is configured:
- ✅ Personal information
- ✅ Research focus
- ✅ Education and experience
- ✅ 10 publications
- ✅ Honors and awards
- ✅ Service activities

Just commit and push to see it live!
