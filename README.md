[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa] ![GitHub Issues or Pull Requests][issues] ![GitHub last commit][commit] ![GitHub contributors][contributors]

# Escape from Tarkov SVG Maps Project

This repository provides high-quality SVG map data for the "Escape from Tarkov" community. These assets are designed to be "source-shared," giving developers a clean foundation to create community tools such as quest trackers, spawn overlays, and interactive web maps. You may have seen them used on [Tarkov.dev](https://tarkov.dev/) and [TarkovTracker](https://tarkovtracker.org/).

## 🗺️ SVG Maps Overview
Our maps are built as modular SVGs to ensure they are web-friendly and easy to manipulate. 
*   **Layered Design:** Maps use SVG group elements (`<g>`) for different floors (e.g., layers in Adobe Illustrator). You can selectively hide or change the opacity of these layers to toggle floor views.
*   **Feature Groups:** Each floor contains sub-groups for specific landmarks like 'roads', 'rocks', or 'ramps', allowing for easy filtering based on your application's needs.
*   **Styling:** Coordinated colour schemes can be updated via post-processing (refer to `replace_style_common.py` and `style_common.css`).

## 🛠️ How to Utilise
Because these are standard SVGs, they can be imported into most modern web or desktop applications.
1.  **Select Floors:** Toggle the parent group elements to display specific levels.
2.  **Filter Details:** Omit sub-layers if your application requires a "lo-fi" or simplified view.
3.  **Custom Styling:** Use the provided CSS/Python scripts to match the map aesthetic to your project.

## ✍️ Map Creation Guidelines
Contributions are welcome! Please open a **Discussion** before starting a major new map to coordinate efforts.
*   **Format:** Entirely SVG-drawn; do not include imported raster images.
*   **Accuracy:** Match in-game maps as closely as possible.
*   **Labels:** Do not include text labels (these should be handled by your application's UI).
*   **Detail Level:** Focus on landmarks, quests, and extracts. Avoid excessive clutter.
*   **Organisation:** Multi-floor maps must use parent-level groups for each floor.
*   **Source Files:** Please include the original source file (e.g., `.ai`) along with the final `.svg`.

## ⚖️ License & Use Restrictions

This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

### 🚫 Specific Use Prohibition & Revocation Clause
**Use of these assets in software designed to facilitate cheating or gaining an unfair advantage in the game *Escape from Tarkov* is EXPLICITLY DISALLOWED.** 

This includes, but is not limited to:
*   In-game radars or ESP overlays.
*   Modified maps intended for use with cheat clients.
*   Automation scripts or "pixel-bots."

**Automatic Revocation:** Any use of these assets in such software constitutes an immediate and automatic revocation of the license granted herein. Software found using these assets in violation of this clause will be considered as having no legal right to use the works and will be subject to DMCA takedown requests and further legal action.

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg
[issues]: https://img.shields.io/github/issues/the-hideout/tarkov-dev-svg-maps
[commit]: https://img.shields.io/github/last-commit/the-hideout/tarkov-dev-svg-maps
[contributors]: https://img.shields.io/github/contributors/the-hideout/tarkov-dev-svg-maps
