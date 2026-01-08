# Dr. Ran Dai - Academic Website

A professional academic website for Dr. Ran Dai, Assistant Professor of Biostatistics at the University of Nebraska Medical Center.

## 📁 Files Included

- `index.html` - Home page with education and research highlights
- `research.html` - Research grants, publications, and software
- `teaching.html` - Teaching activities and student mentoring
- `styles.css` - Comprehensive stylesheet for all pages

## 🚀 Quick Setup for GitHub Pages

### Step 1: Create Your GitHub Repository

1. Go to [github.com](https://github.com) and sign in
2. Click the **+** icon in the top-right corner
3. Select **New repository**
4. Name it: `yourusername.github.io` (replace `yourusername` with your actual GitHub username)
   - Example: if your username is "randai", name it `randai.github.io`
5. Make it **Public**
6. Click **Create repository**

### Step 2: Upload Your Files

**Option A: Drag and Drop (Easiest)**
1. After creating the repository, click **uploading an existing file**
2. Drag all 4 files into the upload area:
   - `index.html`
   - `research.html`
   - `teaching.html`
   - `styles.css`
3. Scroll down and click **Commit changes**

**Option B: Using Git Command Line**
```bash
# Navigate to where you saved the files
cd /path/to/your/files

# Initialize git repository
git init

# Add all files
git add index.html research.html teaching.html styles.css

# Commit files
git commit -m "Initial commit: Add academic website"

# Add remote repository (replace 'yourusername' with your GitHub username)
git remote add origin https://github.com/yourusername/yourusername.github.io.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** (in the top menu)
3. Click **Pages** in the left sidebar
4. Under **Source**:
   - Select **Deploy from a branch**
   - Choose **main** branch
   - Select **/ (root)** folder
5. Click **Save**
6. Wait 2-5 minutes for your site to build

Your website will be live at: `https://yourusername.github.io`

## 📸 Adding Your Photo

### Method 1: Simple Photo Upload (Recommended)

1. Prepare your photo:
   - Use a professional headshot
   - Recommended size: 500x500 pixels or larger (square format)
   - Save as `photo.jpg`
   - File size should be under 1MB for fast loading

2. Upload to GitHub:
   - Go to your repository on GitHub
   - Click **Add file** → **Upload files**
   - Drag your `photo.jpg` file
   - Commit the upload

3. Update `index.html`:
   - In your repository, click on `index.html`
   - Click the pencil icon (Edit)
   - Find these lines (around line 55-60):
   ```html
   <div class="profile-photo-placeholder">
       <p>Your Photo Here</p>
       <span class="photo-instructions">Add your photo as "photo.jpg"</span>
   </div>
   <!-- UNCOMMENT THIS WHEN YOU ADD YOUR PHOTO:
   <img src="photo.jpg" alt="Dr. Ran Dai" class="profile-photo">
   -->
   ```
   
   - Replace with:
   ```html
   <img src="photo.jpg" alt="Dr. Ran Dai" class="profile-photo">
   ```
   
   - Click **Commit changes**

### Method 2: Using an Image Folder

If you want to organize images in a folder:

1. Create an `images` folder in your repository
2. Upload your photo as `images/photo.jpg`
3. In `index.html`, change the image src to:
   ```html
   <img src="images/photo.jpg" alt="Dr. Ran Dai" class="profile-photo">
   ```

### Method 3: Using an External URL

If your photo is hosted elsewhere (like a university website):

1. Copy the direct link to your photo
2. Update `index.html` with the external URL:
   ```html
   <img src="https://example.com/path/to/your/photo.jpg" alt="Dr. Ran Dai" class="profile-photo">
   ```

## 🎨 Customization Guide

### Update Contact Information

All contact info is in `index.html` (lines 37-49). Update:
- Email address
- Phone number
- Office address

### Modify Content

**Home Page (`index.html`):**
- Research highlights (lines 90-105)
- Research interests (lines 115-142)

**Research Page (`research.html`):**
- Grants section (lines 27-173)
- Publications (lines 178-288)
- Software projects (lines 295-320)

**Teaching Page (`teaching.html`):**
- Courses taught (lines 27-87)
- Course development (lines 93-108)
- Student mentoring (lines 113-280)

### Change Colors

Edit `styles.css` (lines 5-15) to change the color scheme:

```css
:root {
    --color-primary: #1a365d;      /* Main dark blue */
    --color-secondary: #2c5282;     /* Secondary blue */
    --color-accent: #c05621;        /* Orange accent */
    /* ... other colors */
}
```

### Customize Fonts

The site uses:
- **Crimson Pro** (serif) for headings
- **IBM Plex Sans** (sans-serif) for body text

To change fonts:
1. Visit [Google Fonts](https://fonts.google.com)
2. Choose your fonts
3. Replace the Google Fonts link in all HTML files (around line 8)
4. Update CSS variables in `styles.css`:
   ```css
   --font-serif: 'Your Heading Font', serif;
   --font-sans: 'Your Body Font', sans-serif;
   ```

## 📱 Features

- ✅ Fully responsive design (works on all devices)
- ✅ Professional academic styling
- ✅ Easy navigation between pages
- ✅ Clean, readable typography
- ✅ Organized sections for research, teaching, and mentoring
- ✅ Optimized for accessibility
- ✅ Fast loading times

## 🔧 Troubleshooting

**Site not loading?**
- Wait 5-10 minutes after enabling GitHub Pages
- Check that your repository is public
- Verify the repository name is exactly `yourusername.github.io`

**Photo not showing?**
- Check the filename is exactly `photo.jpg` (case-sensitive)
- Verify the photo is in the same folder as `index.html`
- Clear your browser cache and refresh

**Styling looks broken?**
- Ensure `styles.css` is in the same folder as the HTML files
- Check that all files were uploaded successfully

**Links not working?**
- Make sure all 4 files are in the root directory (not in subfolders)

## 🌟 Tips for Success

1. **Keep it updated**: Regularly add new publications and grants
2. **Professional photo**: Use a high-quality, professional headshot
3. **Link to publications**: Add DOI or journal links to your papers
4. **Google Scholar**: Link to your Google Scholar profile
5. **Social media**: Consider adding links to professional profiles (Twitter, LinkedIn, ResearchGate)
6. **Custom domain** (optional): You can use a custom domain like `randai.com` instead of `yourusername.github.io`

## 📝 Adding More Content

### To add a new publication:

Copy this template into the publications list in `research.html`:

```html
<div class="publication-item">
    <div class="pub-year">2025</div>
    <div class="pub-content">
        <p class="pub-authors">Author1, Author2, <strong>Dai, R.</strong></p>
        <p class="pub-title">Your Paper Title</p>
        <p class="pub-journal"><em>Journal Name</em>, Volume(Issue), Pages.</p>
    </div>
</div>
```

### To add a new grant:

Copy this template into the grants list in `research.html`:

```html
<div class="grant-item">
    <h3>Grant Title</h3>
    <div class="grant-details">
        <span class="grant-role">Your Role</span>
        <span class="grant-agency">Funding Agency</span>
        <span class="grant-period">Start-End Dates</span>
        <span class="grant-amount">$Amount</span>
    </div>
    <p class="grant-description">Brief description of the grant.</p>
</div>
```

### To add a new course:

Copy this template into the courses list in `teaching.html`:

```html
<div class="course-item">
    <div class="course-header">
        <h3>Course Code: Course Name</h3>
        <span class="course-credits">X credit hours</span>
    </div>
    <p class="course-level">Graduate Course</p>
    <p class="course-terms">Semester Year</p>
    <p class="course-description">Course description here.</p>
</div>
```

## 💡 Next Steps

1. Upload your files to GitHub
2. Add your professional photo
3. Update the Google Scholar link (when you add it)
4. Share your new website URL with colleagues!

## 📞 Need Help?

If you encounter issues:
1. Check the [GitHub Pages documentation](https://docs.github.com/en/pages)
2. Verify all files are uploaded correctly
3. Clear your browser cache
4. Wait a few minutes for changes to appear

---

**Built with modern web standards** | **Optimized for academic professionals** | **Easy to maintain and update**
