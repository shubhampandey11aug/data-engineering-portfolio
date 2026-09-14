# Shubham Pandey - Data Engineer Portfolio Website

A modern, high-performance, single self-contained portfolio website designed for **GitHub Pages**. 

Built with an **HTML5 UP Editorial** inspired fixed left sidebar, responsive 3-column project grid, dynamic interactive case study modal with architecture diagrams and raw writeups, live skills broadcast, light/dark theme switcher, and instant copy-to-clipboard contact actions.

---

## 🚀 Quick Setup: Host on GitHub Pages (Step-by-Step)

Follow these simple steps to deploy your portfolio for free on GitHub in under 3 minutes:

### Step 1: Create a GitHub Repository
1. Log in to your GitHub account ([github.com](https://github.com)).
2. Click the **+** (plus icon) in the top-right corner and select **New repository**.
3. Name your repository:
   - For a user site: `shubham-pandey.github.io` (or your GitHub username: `<username>.github.io`)
   - Or as a project site: `portfolio` or `data-engineer-portfolio`
4. Make sure it is set to **Public**.
5. Do not check "Add a README file" if you are uploading this folder directly. Click **Create repository**.

### Step 2: Upload Files to the Repository
1. On the repository page, click **uploading an existing file** (or push via Git command line).
2. Drag and drop:
   - `index.html` (the main website file)
   - `images/` folder (containing `.gitkeep` and all SVG/PNG diagrams)
   - `README.md`
   - Your `resume.pdf` (optional: place your PDF in the root directory named `resume.pdf`)
3. Write a commit message (e.g., `"Initial portfolio commit"`) and click **Commit changes**.

### Step 3: Enable GitHub Pages
1. In your GitHub repository, click on **Settings** (top tab bar).
2. In the left navigation menu, scroll down and click **Pages** (under the "Code and automation" section).
3. Under **Build and deployment** -> **Source**:
   - Select **Deploy from a branch**.
   - Under **Branch**, select `main` (or `master`) from the dropdown and leave the folder as `/ (root)`.
4. Click **Save**.

### Step 4: Access Your Live Portfolio!
- GitHub Pages will take about 30 to 60 seconds to build.
- Refresh the **Settings -> Pages** page, and you will see your live URL:
  👉 `https://<your-username>.github.io/<repo-name>/` (or `https://<your-username>.github.io`)

---

## 🛠️ How to Customize and Add New Projects

The `index.html` file is designed to be **self-contained and self-guiding** with clear plain-English comments.

### 1. Replace Profile Photo
1. Place your photo (e.g. `profile.jpg`) into the `images/` folder.
2. In `index.html`, search for `images/profile-placeholder.svg` and replace with `images/profile.jpg`.

### 2. Add Your Resume (PDF)
1. Place your resume PDF in the repository root directory named `resume.pdf`.
2. The download buttons in the sidebar, banner, and resume section will automatically download it.

### 3. Add a New Project / Case Study
You can add a new project in two simple steps:

#### Step A: Add a Card to the Projects Grid in HTML
Find `<div class="projects-grid" id="projectsGrid">` and duplicate one of the card blocks:
```html
<div class="project-card" data-category="fabric" data-id="your-project-id">
  <div class="card-thumbnail-container">
    <img src="images/your-diagram.png" alt="Project Title" class="card-thumbnail" />
    <span class="card-category-badge">Microsoft Fabric</span>
  </div>
  <div class="card-body">
    <div class="card-tech-stack">
      <span class="card-tech-pill">Fabric</span>
      <span class="card-tech-pill">PySpark</span>
    </div>
    <h3 class="card-title">Your Project Title</h3>
    <p class="card-excerpt">Summary of your project...</p>
    <div class="card-footer">
      <button class="card-case-study-btn" onclick="openCaseStudyModal('your-project-id')">
        <i class="fa-solid fa-book-open"></i> View Case Study
      </button>
    </div>
  </div>
</div>
```

#### Step B: Add the Detailed Writeup & Screenshots to `CASE_STUDIES` in JavaScript
At the bottom of `index.html` inside `<script>`, add your project object to `CASE_STUDIES`:
```javascript
'your-project-id': {
  title: 'Your Detailed Case Study Title',
  category: 'Microsoft Fabric',
  bannerImg: 'images/your-screenshot.png',
  techStack: ['Microsoft Fabric', 'PySpark', 'Delta Lake', 'Power BI'],
  overview: `
    <h4 class="writeup-section-heading">Business Problem</h4>
    <p>Describe the challenge here...</p>
  `,
  architecture: `
    <h4 class="writeup-section-heading">Architecture</h4>
    <p>Describe your pipeline and medallion architecture...</p>
  `,
  implementation: `
    <h4 class="writeup-section-heading">Code Sample</h4>
    <div class="code-block-container">
      <pre><code># Your PySpark / SQL code here</code></pre>
    </div>
  `,
  results: `
    <h4 class="writeup-section-heading">Impact</h4>
    <p>Describe the business results and metrics...</p>
  `,
  rawWriteup: `
    <div class="code-block-container">
      <pre><code># Paste your raw case study writeup here</code></pre>
    </div>
  `
}
```

---

## 🎨 Features Included

- **Single Self-Contained File:** All styling and JavaScript logic are fully embedded in `index.html`.
- **Editorial Layout:** Fixed desktop sidebar with mobile drawer navigation.
- **Light & Dark Theme:** Switcher stored in `localStorage`.
- **Live Tech Stack Ticker:** Broadcaster highlighting Fabric, Databricks, Azure, Power BI, and GenAI.
- **Interactive Case Study Modal:** Tabbed technical deep dive (Overview, Architecture, Code, Results, Raw Writeup).
- **Search & Filter:** Instant search across tools and category filters (Fabric, Databricks, Power BI, GenAI).
- **One-Click Actions:** Direct email launcher, LinkedIn link, and copy-email toast notifications.
