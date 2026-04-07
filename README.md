# spec-id
# 🗂️ System Cards

**System Cards** is a beautiful, local-first product documentation and handoff tool built as a single-page Progressive Web App (PWA). It helps creators, developers, and product managers document the core essence of a project—problems, solutions, workflows, and handoff readiness—in a concise, highly readable format.

##  Features

* ** Glassmorphic UI:** A fluid, modern interface built with CSS grid, custom properties, and backdrop-filters.
* ** Local-First Storage:** Powered by **IndexedDB**, ensuring high storage capacity, non-blocking asynchronous data saves, and complete data privacy (nothing is sent to a server).
* ** PWA Ready:** Installable directly to your desktop or home screen. Includes a generated Service Worker for fully offline functionality.
* ** Markdown Export:** Instantly preview and export any system card (or all of them at once) as clean, formatted `.md` files.
* ** Smart Templates:** Jumpstart your documentation with pre-filled templates for AI Tools, Developer Tools, Media Pipelines, Internal Dashboards, and Browser Extensions.
* ** Undo/Redo History:** Made a mistake? Seamlessly step back and forth through your session's edit history.
* ** Instant Search:** Filter through your cards in real-time.

##  How to Use

Because System Cards is entirely client-side and requires no build step, getting started takes seconds:

1. **Download:** Save the provided code as `index.html`.
2. **Run:** Double-click `index.html` to open it in any modern web browser.
3. **Install (Optional):** Click the "Install App" button in the bottom right corner to install it as a standalone PWA on your device.

### The Workflow
1. **Cards Tab:** View your dashboard of existing projects. Use the search icon to filter by project name or description.
2. **+ New Tab:** Create a new card from scratch. Rate its "Handoff Readiness" on a scale of 1-10.
3. **Templates Tab:** Start a new card using tailored prompts and structures based on your project type.
4. **Detail View:** Click on any card in your dashboard to view its full details, edit it, or export it to Markdown.

## 🏗️ Architecture & Tech Stack

System Cards is built with zero external dependencies, emphasizing performance and longevity:

* **HTML5:** Semantic structure and built-in PWA manifest.
* **CSS3:** Scoped custom properties (variables), Flexbox, CSS Grid, and hardware-accelerated animations. No CSS frameworks required.
* **Vanilla JavaScript (ES6+):** * **IndexedDB API:** Used for robust, asynchronous client-side storage, replacing `localStorage` to avoid 5MB limits and main-thread blocking.
  * **Service Worker API:** Caches the application assets dynamically for offline use.
  * **Blob API:** Generates downloadable `.md` files entirely in the browser.

## 💾 Why IndexedDB?

While many single-page tools rely on `localStorage`, System Cards is built to hold extensive, text-heavy documentation. IndexedDB was chosen for this project because:
1. **Capacity:** It allows for hundreds of megabytes of storage, ensuring you never run out of space for your markdown content.
2. **Performance:** Database transactions run asynchronously, meaning auto-saves and large exports will never cause the UI or animations to stutter.

# AI Post Generator for System Cards

## Goal
Automatically generate polished posts for different platforms (Reddit, LinkedIn, Twitter, Indie Hackers) based on a project/product description.

## Why
- Reduce friction in handoff and publishing.
- Keep creators focused on building new ideas rather than rewriting posts for each platform.
- Validate ideas by sharing outputs early and consistently.

## How
1. Take project description from user.
2. Use deterministic AI templates to generate platform-specific posts.
3. Show auto-preview in modal.
4. Batch generate for all platforms at once.
5. Allow export of all generated posts as Markdown.
6. Fully client-side, integrates into existing IndexedDB PWA.

## Outcome
- System Cards now not only document projects but generate actionable, shareable posts.
- Helps creators move from internal validation to external signal.

## 📄 License

This project is open-source and free to use or modify for your personal and professional workflow needs.
