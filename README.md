# 🐄 Tyrol Almabtriebe & Cattle Drives 2026 — Fancy Cow Map

An interactive web application showcasing traditional cattle, sheep, and stallion drives (*Almabtriebe*) across Tyrol, Austria for the 2026 autumn season.

---

## ✨ Features

- **Interactive Leaflet Map**: Responsive alpine map with custom teardrop pins, date badges, and color coding by time of season.
- **Innsbruck Distance Engine**: Automatic straight-line (Haversine) distance calculations from Innsbruck Altstadt to every event location.
- **Bi-Directional Card & Pin Sync**:
  - Clicking any timeline card smoothly flies the map to the location and opens its details popup.
  - Clicking any map marker highlights the event card and scrolls it into view.
- **Search & Filters**:
  - **Live Search**: Instant lookup by event name, village, or valley.
  - **Animal Type Filters**: Cattle (*Almabtrieb*), Sheep (*Schafschoad*), and Stallions (*Hengstalmabtrieb*).
  - **Region Dropdown**: Filter across 14+ distinct Tyrolean regions (Zillertal, Tannheimer Tal, Achensee, Kitzbühel Alps, etc.).
  - **Sorting**: Chronological date order, closest to Innsbruck, furthest, or alphabetical.
- **Zero-Dependency Static Architecture**: Pure HTML, CSS, and vanilla JS using OpenStreetMap and Leaflet CDN. Works instantly locally and on GitHub Pages with zero build step.

---

## 🚀 Running Locally

You can open `index.html` directly in any web browser, or run a lightweight local HTTP server:

```bash
# In the project directory:
python3 -m http.server 8080
```

Then visit:
👉 **[http://localhost:8080](http://localhost:8080)**

---

## 🌐 Deploying to GitHub Pages (Step-by-Step)

Follow these simple steps to host this map publicly on your GitHub profile:

### Step 1: Create a New Repository on GitHub
1. Go to [github.com/new](https://github.com/new).
2. Name your repository (e.g., `Fancy_Cow_Map` or `tyrol-cow-map`).
3. Choose **Public** (required for free GitHub Pages).
4. Do **not** check "Add a README file" (we already have one).
5. Click **Create repository**.

### Step 2: Push Your Local Code to GitHub
In your terminal, inside this project directory (`/Applications/Fancy_Cow_Map`):

```bash
# Add your GitHub repository as the remote origin (replace YOUR-USERNAME and YOUR-REPO-NAME):
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git

# Push the main branch:
git push -u origin main
```

*(If you are using SSH instead of HTTPS, use `git@github.com:YOUR-USERNAME/YOUR-REPO-NAME.git`)*

### Step 3: Turn on GitHub Pages
1. Go to your repository on GitHub.
2. Click **Settings** (top tab with gear icon).
3. In the left sidebar, click **Pages** (under the "Code and automation" section).
4. Under **Build and deployment**:
   - **Source**: Select `Deploy from a branch`.
   - **Branch**: Select `main` branch and `/ (root)` folder.
   - Click **Save**.
5. Within 1–2 minutes, GitHub will generate your live URL:
   `https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/`

---

## 📁 Project Structure

```
Fancy_Cow_Map/
├── index.html                  # Main interactive web application
├── tyrol_cattle_drives_2026.html # Original standalone version
├── events.json                 # Raw JSON event dataset (36 drives)
├── .gitignore                  # Git ignore rules
└── README.md                   # Documentation and deployment guide
```

---

## 📜 Data Source
Event dates and locations are compiled from published tourist board schedules and regional media ([Allgäuer Zeitung](https://www.allgaeuer-zeitung.de)). Dates and celebrations are subject to local alpine weather conditions and pasture timing.
