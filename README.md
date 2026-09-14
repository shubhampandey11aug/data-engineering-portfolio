# Shubham Pandey - Data Engineer Portfolio Website

A modern, high-performance, single self-contained portfolio website designed for **GitHub Pages**. 

Built with an **HTML5 UP Editorial** inspired fixed left sidebar, responsive project grid, dynamic interactive case study modal with architecture diagrams and raw writeups, live skills broadcast ticker, light/dark theme switcher, interactive screenshot gallery with click-to-zoom lightbox, and instant copy-to-clipboard contact actions.

---

## 📁 Exact File & Asset Placement Guide

To customize the website with your personal photo, resume, and screenshots from `assest.rar`:

### 1. Profile Picture
- **File Name:** `profile.jpg` (or `profile.png`)
- **Path:** Place inside the `images/` directory (`images/profile.jpg`).
- If not provided, it automatically falls back gracefully to `images/profile-placeholder.svg`.

### 2. Resume Download
- **File Name:** `resume.pdf`
- **Path:** Place in the **root directory** alongside `index.html` (`./resume.pdf`).
- All "Download Resume" buttons automatically target `resume.pdf`.

### 3. Screenshots & Main Card Images (Extracted from `assest.rar`)
Extract the images from `assest.rar`, rename them according to the reference mapping below, and copy them into the `images/` folder. The **"Title Image"** of each project automatically acts as the card thumbnail on the homepage (`cardImage`):

| Case Study | Title Image (Main Card Thumbnail) | Gallery Screenshots |
|---|---|---|
| **CS 01: Global Listing Intelligence** | `images/cs01-title.png` | `cs01-pipeline.png`, `cs01-copy-source.png`, `cs01-copy-dest.png`, `cs01-schema-mapping.png`, `cs01-system-constraints.png`, `cs01-archive-source.png`, `cs01-archive-dest.png`, `cs01-landing.png` |
| **CS 02: Logistics Watermark State** | `images/cs02-title.png` | `cs02-pipeline.png`, `cs02-notebook-table.png`, `cs02-set-watermark.png`, `cs02-copy-source.png`, `cs02-update-watermark.png`, `cs02-pipeline-run.png` |
| **CS 03: Workforce Intelligence Lakehouse** | `images/cs03-title.png` | `cs03-target-tables.png`, `cs03-copy-source.png`, `cs03-pipeline-design.png`, `cs03-copy-dest.png`, `cs03-bronze-table.png`, `cs03-notebook-read.png`, `cs03-quarantine-logic.png`, `cs03-filter-invalid.png`, `cs03-drop-duplicates.png`, `cs03-write-silver.png`, `cs03-view-quarantine.png`, `cs03-view-silver.png` |
| **CS 04: Financial PySpark Optimization** | `images/cs04-title.png` | `cs04-schema.png`, `cs04-tx-view.png`, `cs04-physical-plan.png`, `cs04-broadcast-join.png`, `cs04-bad-data.png`, `cs04-time-travel-update.png`, `cs04-describe-history.png`, `cs04-restore-version.png` |
| **CS 05: Commerce Medallion & Direct Lake** | `images/cs05-title.png` | `cs05-architecture.png`, `cs05-lookup.png`, `cs05-foreach.png`, `cs05-foreach-copy.png`, `cs05-bronze-to-silver.png`, `cs05-silver-view.png`, `cs05-silver-to-gold.png`, `cs05-gold-tables.png` |
| **CS 06: Market Risk T-SQL JSON Shredding** | `images/cs06-title.png` | `cs06-create-schema.png`, `cs06-json-parsing.png`, `cs06-create-sp.png`, `cs06-pipeline.png`, `cs06-pipeline-sp.png`, `cs06-pipeline-run.png`, `cs06-idempotent-sp.png` |
| **CS 07: Regulatory SCD Type 2 Hierarchy** | `images/cs07-title.png` | `cs07-schema-copy.png`, `cs07-gold-view.png`, `cs07-rm-leaderboard.png`, `cs07-hierarchy-cte.png`, `cs07-hierarchy-output.png`, `cs07-scd2-structure.png`, `cs07-scd2-merge.png` |
| **CS 08: On-Premise Gateway Lakehouse** | `images/cs08-title.png` | `cs08-gateway-config.png`, `cs08-postgres-table.png`, `cs08-pipeline-design.png`, `cs08-copy-settings.png`, `cs08-lakehouse-load.png`, `cs08-audit-logging.png` |
| **CS 09: Customer Dataflow Gen2 Cleansing** | `images/cs09-title.png` | `cs09-bronze-customer.png`, `cs09-merge-state.png`, `cs09-split-address.png`, `cs09-merge-address.png`, `cs09-phone-clean.png`, `cs09-clean-silver.png` |
| **CS 10: Real-Time Intelligence Eventhouse** | `images/cs10-title.png` | `cs10-eventhouse.png`, `cs10-kql-schema.png`, `cs10-eventstream.png`, `cs10-kql-queries.png`, `cs10-activator-alert.png`, `cs10-audit-log.png`, `cs10-rt-dashboard.png` |

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
2. Upload the following files:
   - `index.html` (the main single-file portfolio)
   - `resume.pdf` (your personal resume PDF)
   - `images/` folder (with all SVGs and PNG screenshots)
   - `README.md`
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

## 🎨 Features Included

- **Single Self-Contained File:** All styling and JavaScript logic are fully embedded in `index.html`.
- **Editorial Layout:** Fixed desktop sidebar with mobile drawer navigation.
- **Redesigned Engineering Profile Card:** Modern rectangular profile card displaying core engineering metadata, certifications, and live status.
- **Continuous Live Tools Broadcaster:** Smooth CSS-animated ticker showcasing Microsoft Fabric, Databricks, Azure, Power BI, Delta Lake, and PySpark.
- **Interactive 5-Tab Case Study Modal:** Deep technical views covering:
  1. *Overview & Challenge*
  2. *Architecture & Pipeline*
  3. *Implementation & Code*
  4. *Results & Impact*
  5. *Gallery & Screenshots* (with interactive thumbnail grid)
- **Click-to-Zoom Screenshot Lightbox:** Full-screen inspection modal with image captions and keyboard/backdrop dismissal.
- **Light & Dark Theme:** Switcher stored in `localStorage`.
- **Defensive Image Fallbacks:** Embedded `onerror` handlers prevent broken image boxes if files are renamed or missing.
