# Portfolio Repo - Final Setup Guide

## ✅ What's Done
- Repo renamed to: `portfolio`
- Website live at: `https://vkiefner.github.io/portfolio`
- CV compiles successfully

---

## 📁 Files to Update in Your Repo

### 1. Replace `.github/workflows/compile-cv.yml`
**Location:** `.github/workflows/compile-cv.yml`

Use the file: `compile-cv-portfolio.yml` from outputs

**Changes made:**
- Updated git push to use correct repo reference
- Optimized for fast compilation (2-3 mins instead of 30)

---

### 2. Replace `index.html`
**Location:** `index.html` (root of repo)

Use the file: `index-portfolio.html` from outputs

**Changes made:**
- All paths now relative and correct for `/portfolio` subdirectory
- Links to `files/CV_Kiefner.pdf` work correctly
- Links to `images/profile.jpg` work correctly

---

### 3. Ensure These Files Exist in Your Repo

```
portfolio/
├── index.html                    ← Updated
├── .github/
│   └── workflows/
│       └── compile-cv.yml        ← Updated
├── files/
│   ├── CV_Kiefner.tex           ← Use CV_Kiefner_FIXED.tex
│   └── CV_Kiefner.pdf           ← Auto-generated
├── images/
│   └── profile.jpg              ← Your profile photo (180x180px)
└── README.md                     ← Optional
```

---

## 🚀 Next Steps

1. **Update `.github/workflows/compile-cv.yml`**
   - Copy content from `compile-cv-portfolio.yml`
   - Commit and push

2. **Update `index.html`**
   - Copy content from `index-portfolio.html`
   - Commit and push

3. **Update `files/CV_Kiefner.tex`**
   - Copy content from `CV_Kiefner_FIXED.tex`
   - Commit and push

4. **Add profile photo**
   - Upload or drag `profile.jpg` to `images/` folder
   - Should be 180x180px for best results
   - Commit and push

5. **Test everything**
   - Visit: `https://vkiefner.github.io/portfolio`
   - Download CV button should work
   - All links should work

---

## ✅ Verify Everything Works

After pushing all files:
1. Check `https://vkiefner.github.io/portfolio` loads correctly
2. Click "Download CV (PDF)" — should download CV_Kiefner.pdf
3. All contact links work (email, Google Scholar, etc.)
4. Profile photo displays

---

## 🔧 If Git Push Fails

Error message: `Permission denied to github-actions[bot]`

**Solution:**
1. Go to repo Settings
2. **Actions** → **General**
3. Under "Workflow permissions":
   - Select: "Read and write permissions"
   - Check: "Allow GitHub Actions to create and approve pull requests"
4. Save and re-run workflow

---

## 📝 Future CV Updates

Now whenever you edit `files/CV_Kiefner.tex`:
1. Commit and push
2. GitHub Actions auto-compiles (2-3 mins)
3. New PDF auto-uploads to repo
4. Your website shows latest CV ✅

No more manual compilation needed!

---

**All done! Your academic portfolio is live at:**
# 🎉 https://vkiefner.github.io/portfolio
