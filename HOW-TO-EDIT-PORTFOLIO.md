# 📋 How to Edit Your Portfolio Website

## A Complete Guide for Sanjay P

---

## 📁 File Structure

Your portfolio consists of just **2 files**:

| File | Purpose |
|------|---------|
| `index.html` | The entire website (HTML + CSS + JavaScript) |
| `profile.jpg` | Your profile photo |

---

## 🔧 How to Open and Edit

1. **Right-click** on `index.html`
2. Select **"Open with"** → **Notepad** or **VS Code** (recommended)
3. Make your changes
4. **Save** the file (Ctrl + S)
5. **Double-click** `index.html` to preview in your browser

> [!TIP]
> Download **VS Code** (free) for the best editing experience — it color-codes your HTML and catches errors.

---

## ✏️ What You Can Edit and Where to Find It

### 1. **Your Name & Title** (Hero Section)
Search for `SANJAY` in the file. The hero section starts around the `<section class="hero">` tag.

```html
<h1>
    Python Developer <br>
    DevOps Engineer <br>
    <span class="highlight" id="typed-title">Data Engineer</span>
</h1>
```

To change the rotating titles, find this JavaScript array:
```javascript
const titles = ["Data Engineer", "Python Developer", "AI Engineer"];
```
Change the text inside the quotes to whatever titles you want.

---

### 2. **Profile Photo**
Replace the `profile.jpg` file with your new photo. **Keep the same filename** (`profile.jpg`), or update this line:
```html
<img src="profile.jpg" alt="Sanjay P - AI and Data Science graduate">
```

---

### 3. **Contact Information**
Search for `sanjaypanneerselvam2004@gmail.com` to find all email references. Search for `9543647888` for phone. Update these throughout:

```html
<!-- Email -->
<a href="mailto:YOUR_NEW_EMAIL@gmail.com">YOUR_NEW_EMAIL@gmail.com</a>

<!-- Phone -->
<a href="tel:+91XXXXXXXXXX">+91 XXXXXXXXXX</a>

<!-- LinkedIn -->
<a href="https://linkedin.com/in/YOUR_LINKEDIN_ID">

<!-- GitHub -->
<a href="https://github.com/YOUR_GITHUB_USERNAME">
```

> [!IMPORTANT]
> Your email, phone, GitHub, and LinkedIn appear in **multiple places** (hero, about, contact, footer). Use **Ctrl + H** (Find & Replace) to update all at once.

---

### 4. **About Me / Summary**
Find `<section id="about">` and edit the paragraph inside the `about-box full-width` div:

```html
<div class="about-box full-width">
    <h3>Summary</h3>
    <p>
        <!-- Write your updated summary here -->
    </p>
</div>
```

---

### 5. **Experience**
Find `<section id="experience">`. Each job is inside an `experience-card`:

```html
<div class="experience-card">
    <h3>YOUR JOB TITLE</h3>
    <p class="company">COMPANY NAME</p>
    <p class="date-location">DATE | LOCATION</p>
    <ul>
        <li>Bullet point 1</li>
        <li>Bullet point 2</li>
    </ul>
</div>
```

**To add another experience**, copy the entire `<div class="experience-card">...</div>` block and paste it below.

---

### 6. **Skills**
Find `<section id="skills">`. Each skill is a `skill-card`:

```html
<div class="skill-card reveal-child">
    <div class="skill-icon"><i class="fab fa-python"></i></div>
    <h3>Skill Name</h3>
    <p>Description</p>
    <div class="skill-tags">
        <span class="skill-tag">Tag1</span>
        <span class="skill-tag">Tag2</span>
    </div>
</div>
```

**Icons**: Find icons at [Font Awesome](https://fontawesome.com/icons). Replace the `class="fab fa-python"` with any icon class.

---

### 7. **Projects**
Find `<section id="projects">`. Each project is a `project-card`:

```html
<article class="project-card reveal-child">
    <span class="project-label">Category</span>
    <h3>Project Name</h3>
    <p>Description of the project.</p>
    <div class="project-tech">
        <span>Tech1</span>
        <span>Tech2</span>
    </div>
    <div class="project-links">
        <a href="https://github.com/YOUR_REPO" target="_blank">
            <i class="fab fa-github"></i> GitHub →
        </a>
    </div>
</article>
```

**To add a new project**, copy this entire block and paste it inside the `projects-grid` div.

---

### 8. **Education**
Find `<section id="education">`. Update the grades:

```html
<div class="grade-badge">
    <div class="label">CGPA</div>
    <div class="value">7.4</div>  <!-- Change this number -->
</div>
```

---

### 9. **Colors & Theme**
The main colors are defined in the CSS at the top of the file. Search for these values:

| Color | Hex Code | Used For |
|-------|----------|----------|
| Dark background | `#0b1020` | Page background |
| Card background | `#11192c` | Cards & boxes |
| Accent / Highlight | `#72e6ff` | Links, titles, borders |
| Text | `#f4f6ff` | Main text |
| Muted text | `#bac4da` | Descriptions |
| Border | `#28344e` | Card borders |

**To change the accent color**, use **Ctrl + H** to replace `#72e6ff` with your preferred color (e.g., `#ff6b9d` for pink, `#4ade80` for green).

---

### 10. **Stats Numbers**
Find the `stats-row` section. Change the `data-target` values:

```html
<span class="stat-number" data-target="5">0</span>  <!-- Projects count -->
```

---

## 🚀 How to Deploy (Put Online)

### Option 1: GitHub Pages (Free & Recommended)
1. Create a GitHub repository named `your-username.github.io`
2. Upload `index.html` and `profile.jpg`
3. Go to **Settings → Pages → Source: main branch**
4. Your site will be live at `https://your-username.github.io`

### Option 2: Netlify (Free)
1. Go to [netlify.com](https://netlify.com)
2. Drag & drop your `my-portfolio` folder
3. Get a free URL instantly

### Option 3: Vercel (Free)
1. Go to [vercel.com](https://vercel.com)
2. Import your GitHub repository
3. Auto-deploys on every push

---

## 💡 Pro Tips for Freshers

1. **Keep it updated** — Add new projects as you build them
2. **Use real GitHub links** — Recruiters check your code
3. **Add a resume PDF** — Link a downloadable resume in the hero section
4. **Custom domain** — Buy a `.dev` or `.me` domain for ₹200-500/year for professionalism
5. **Add project screenshots** — Visual projects are more impressive
6. **Google Analytics** — Track who visits your portfolio

---

## 🔗 Useful Resources

- **Font Awesome Icons**: https://fontawesome.com/icons
- **Color Picker**: https://coolors.co
- **Google Fonts**: https://fonts.google.com
- **VS Code Download**: https://code.visualstudio.com
- **GitHub Pages Guide**: https://pages.github.com

---

*Last updated: November 2026*
