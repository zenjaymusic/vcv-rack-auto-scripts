# VCV Rack Auto Scripts

Tampermonkey userscripts that automate tedious tasks in the VCV Rack library — subscribing to plugins and adding free modules across paginated results.

---

## Scripts

### 1. VCV Plugin Auto-Subscribe All

Automatically subscribes to every free VCV plugin on the library plugins page in fast batches.

**What it does:**
- Finds all visible Subscribe buttons on the page
- Clicks them in batches of 10
- Waits for each subscription to confirm before moving to the next batch
- Skips plugins you're already subscribed to
- Logs progress to the browser console

**Install:** [VCV Plugin Auto-Subscribe All](https://github.com/zenjaymusic/vcv-rack-auto-scripts/raw/refs/heads/main/VCV%20Plugin%20Auto-Subscribe%20All%20(Fast%20Batching))

**Usage:** Navigate to `https://library.vcvrack.com/plugins` and the script runs automatically on page load.

---

### 2. VCV Library Auto-Add Free Modules

Automatically clicks Add on every free module across all paginated pages of the VCV library.

**What it does:**
- Finds all Add buttons on the current page
- Clicks them in batches of 10
- Waits for each module to confirm before continuing
- Automatically clicks the next page arrow and repeats until all pages are done
- Handles VCV's SPA navigation correctly

**Install:** [VCV Library Auto-Add Free Modules](https://github.com/zenjaymusic/vcv-rack-auto-scripts/raw/refs/heads/main/VCV%20Library%20Auto-Add%20Free%20Modules)

**Usage:** Navigate to `https://library.vcvrack.com` and the script runs automatically, paging through the entire library until complete.

---

## Installation

1. Install [Tampermonkey](https://www.tampermonkey.net/) for your browser
2. Click an install link above
3. Click **Install** in the Tampermonkey prompt
4. Navigate to the relevant VCV library page — the script will run automatically

## Notes

- You must be logged in to your VCV Rack account for subscriptions and adds to save
- Progress is logged to the browser console (F12 → Console) if you want to monitor it
- Both scripts run in batches to avoid overwhelming the VCV library server

## License

MIT — free to use, modify, and share.
