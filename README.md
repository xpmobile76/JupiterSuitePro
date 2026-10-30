# Jupiter Suite Pro

**Web Scraper · Media Downloader · NLP Data Preparation Suite**  
*Version 5.93 Family — Jupiter Innovation Group*

Jupiter Suite Pro is an enterprise desktop environment and Chrome extension bridge engineered for capturing social media content, downloading streaming video/audio through multi-engine fallbacks, and preparing rich NLP datasets from real browser sessions.

---

## 🚀 Key Highlights & Architectural Overview

1. **Live Chrome Session Bridge**
   - Direct DOM extraction from authenticated and anti-bot cleared browser sessions (Cloudflare, bot interstitials).
   - Session cookie sync between extension, native host (`JupiterMediaHost.exe`), and desktop worker threads.

2. **Platform-Aware Social Capture**
   - **Reddit (Integrated):** Recursive cycles for nested comment replies, subreddit thread metadata, author profiles, and native `v.redd.it` / `i.redd.it` media handling.
   - **Instagram:** Posts, reels, comments drawer parsing, and progressive CDN fallback.
   - **YouTube:** Video and Shorts comments, live player audio-language metadata tags, yt-dlp + sniffer integration.
   - **TikTok / Douyin / Bilibili / Facebook / LinkedIn / X (Twitter):** Individual expand and download paths.

3. **Multi-Engine Media Downloader**
   - `yt-dlp` primary downloader with browser cookie passing.
   - Direct API CDN progressive download fallbacks.
   - Live stream sniffer with automated `ffmpeg` remuxing.

4. **Companion NLP Pipeline Apps**
   - Classical Data Preparation (spaCy, tokenization, TF-IDF).
   - SEA-Lion regional NLP modules and PyTorch / Transformers model export.

---

## 📦 Repository Structure

```
├── index.html                                   # Web presentation & video demo page (GitHub Pages ready)
├── recording_20261030_105349.mp4                # Demo recording of review extraction & media download
├── screenshot_demo.jpg                          # Jupiter Suite Pro & Browser Extension UI screenshot
├── JupiterSuitePro_Features_and_Description.pdf # Full specification and documentation PDF
└── README.md                                    # Project documentation
```

---

## 🛠️ Quick Start & Usage

1. Open `index.html` in any modern browser or host directly via **GitHub Pages**.
2. Run the desktop application and copy your extension token into the Chrome extension popup.
3. Navigate to any target social media post (e.g., Reddit thread or Instagram Reel) and click **Capture This Page**.
4. Extracted reviews, metadata, and media items automatically populate the Scraper and Media Download queues.

---
*© 2026 Jupiter Suite Pro · Jupiter Innovation Group*
