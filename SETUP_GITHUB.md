# How to Upload to GitHub

## Step 1: Open PowerShell in Project Folder

```powershell
cd "C:\Users\MansourYoum\Documents\ProjectCursor\BibliPrompt"
```

## Step 2: Initialize Git (if not already done)

```powershell
git init
```

## Step 3: Add All Files

```powershell
git add .
```

## Step 4: Create Initial Commit

```powershell
git commit -m "Initial commit: AI Prompt Studio v1"
```

## Step 5: Add Remote Repository

Go to GitHub.com and create a new repository named `v3promptlibrary` (or any name you prefer), then:

```powershell
git remote add origin https://github.com/YOUR_USERNAME/v3promptlibrary.git
```

## Step 6: Push to GitHub

```powershell
git branch -M main
git push -u origin main
```

## Step 7: Deploy on Streamlit Cloud

1. Go to https://share.streamlit.io
2. Sign in with GitHub
3. Click "New app"
4. Select repository: `v3promptlibrary`
5. Set main file path: `app.py`
6. Click "Deploy"

## Troubleshooting

### If you get "origin already exists":
```powershell
git remote remove origin
git remote add origin https://github.com/YOUR_USERNAME/v3promptlibrary.git
```

### If you need to force push:
```powershell
git push -u origin main --force
```

