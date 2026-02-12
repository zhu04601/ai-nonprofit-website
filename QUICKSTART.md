# 🚀 Quick Start - Fixed Version

## Step 1: Extract Files

Unzip the `ai-nonprofit-website-fixed.zip` file.

## Step 2: Install MkDocs

```bash
pip install mkdocs-material
```

## Step 3: Test Locally

```bash
cd ai-nonprofit-website-fixed
mkdocs serve
```

Open: http://127.0.0.1:8000

## Step 4: Deploy to GitHub

### Option A: Replace Everything

```bash
# In your GitHub repo folder:
rm -rf * (keep .git folder!)
cp -r /path/to/ai-nonprofit-website-fixed/* .
git add .
git commit -m "Complete fix with all content"
git push
mkdocs gh-deploy
```

### Option B: Fresh Start

```bash
# Create new repo on GitHub
# Then:
cd ai-nonprofit-website-fixed
git init
git add .
git commit -m "Initial commit - fixed version"
git remote add origin https://github.com/zhu04601/ai-nonprofit-website.git
git push -u origin main
mkdocs gh-deploy
```

## Done! ✅

Site live at: https://zhu04601.github.io/ai-nonprofit-website/

## What You'll See

✅ Working logo  
✅ Beautiful hero image  
✅ All pages with content  
✅ Working navigation  
✅ Complete glossary  
✅ Full FAQ  
✅ Resource links  

Perfect!
