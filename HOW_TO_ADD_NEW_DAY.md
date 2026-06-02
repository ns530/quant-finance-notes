# How to Add a New Day Article

## Every day — 3 simple steps:

### Step 1: Create the new file
Copy day2.html → rename to day3.html (or whatever day)
Update:
- `<title>` tag
- nav-badge: "Day X / 90"
- hero series-tag: "Day X of 90"
- hero h1 title
- hero-sub description
- day-badge: "0X / 90"
- All article content
- article-nav links (prev/next days)
- footer-next (tomorrow's topic)

### Step 2: Update index.html
Find the "coming-soon" card for that day and:
1. Change `class="day-card coming-soon lX"` → `class="day-card published lX"`
2. Change `<div class="day-status">Coming soon</div>` → `<div class="day-status">✓ Published</div>`
3. Change `<div class="day-card-title">` to wrap in `<a href="dayX.html" ...>`
4. Add `<span class="day-card-arrow">→</span>` in footer
5. Update nav-badge: "Day X / 90"
6. Update progress-fill width: (X/90 * 100)%
7. Update progress-label number
8. Update hero-stat "Published" number

### Step 3: Push to GitHub
```bash
git add .
git commit -m "Add Day X: [Topic Name]"
git push
```
GitHub Pages auto-deploys in ~60 seconds!

## File naming convention:
- day1.html, day2.html, day3.html ... day90.html
- style.css (shared — never edit unless changing theme for ALL articles)
- index.html (homepage — update published count each day)

## Layer colors for day-num-badge:
- Layer 1 (Days 1-17):  class="l1"  → blue
- Layer 2 (Days 18-26): class="l2"  → purple  
- Layer 3 (Days 27-33): class="l3"  → red
- Layer 4 (Days 34-44): class="l4"  → amber
- Layer 5 (Days 45-50): class="l5"  → green
- Layer 6 (Days 51-65): class="l6"  → orange
