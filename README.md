
# GHX

A Chrome extension designed to perform Google Dorking, automatically load search results, and save them to a TXT file. Created by frostynxth, this extension features a dark mode interface with red-stroke buttons for a sleek user experience.

## Features

- Google Dorking: Enter custom dork queries (e.g., inurl:login) to search for specific web pages.
- Automatic Result Loading: Fetches and displays up to 100 URLs per query, with pagination support.
- Load More: A "Load More" button to retrieve additional results (10 URLs per page).
- Save to TXT: Export all loaded URLs to a dorking_results.txt file.
- Dark Mode UI: A modern dark theme with red-stroke buttons for improved aesthetics and readability.

# Google Dorking Extension – Setup Guide

## Setting Up Google Custom Search API

To use this extension, you need to set up the **Google Custom Search API** and obtain an **API Key** and **Custom Search Engine ID (CSE ID)**.

---

## 🔧 Step-by-Step Instructions

### 1. Create a Google Cloud Project

1. Visit the [Google Cloud Console](https://console.cloud.google.com/).
2. Click **"New Project"**, give it a name (e.g., `Google Dorking Extension`), and create the project.

---

### 2. Enable Custom Search API

1. In the Cloud Console, navigate to: `APIs & Services > Library`.
2. Search for **"Custom Search API"** and click **Enable**.

---

### 3. Generate an API Key

1. Go to: `APIs & Services > Credentials`.
2. Click **"Create Credentials" > "API Key"**.
3. Copy and save the generated **API Key**.

---

### 4. Create a Custom Search Engine (CSE)

1. Visit [Google Programmable Search Engine](https://programmablesearchengine.google.com/).
2. Click **"New Search Engine"**, set it to search the **Entire Web**, and create it.
3. Go to `Edit search engine > Setup`, and copy the **Search engine ID (CSE ID)**.

---

## 🛠 Configure the Extension

1. Open `popup.js` in your project folder.
2. Replace:
   - `YOUR_API_KEY` with your actual API Key.
   - `YOUR_CSE_ID` with your actual CSE ID.

---

## 📌 Notes

- The API has a **free quota of 100 queries per day**. If exceeded, billing needs to be enabled.
- Keep your **API Key** and **CSE ID** secure – **do not share them publicly**.

---

## 📸 Screenshots

> **Popup in dark mode** with red-stroke buttons and sample results:
>
> *(Add a screenshot of the popup here for visual reference.)*

---

## ⚠️ Limitations

- Maximum of **100 results per query** due to API limitations.
- Results may differ slightly from standard Google search results.
- Requires an **active internet connection** to fetch results.

---

## ✅ You're all set!

Your Google Dorking Extension should now be fully functional with the Google Custom Search API.

## Authors

- [@frostyxsec](https://www.github.com/frostyxsec)

