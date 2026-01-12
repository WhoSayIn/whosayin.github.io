# Project Overview

This directory contains the source code for Huseyin Keles's personal website, hosted on GitHub Pages. It serves as a central hub for his online presence and occasionally hosts specific event pages. The site is a collection of static HTML files designed to be simple and lightweight.

# Key Files

-   **`index.html`**: The main entry point for the website. It is a minimal HTML page that lists links to Huseyin's various social media profiles and online accounts (LinkedIn, Twitter, GitHub, etc.).
-   **`CNAME`**: A configuration file used by GitHub Pages to map the repository to the custom domain `huseyinkel.es`.
-   **`bd/index.html`**: A standalone page for a specific event ("Huseyin's Birthday Party"). It includes details about the event, location (with an embedded map), and links to add the event to a calendar or join a WhatsApp group.
-   **`404.html`**: A custom error page displayed when a user navigates to a non-existent URL on the domain.

# Usage

This project is a static site. The content is served directly by GitHub Pages.

1.  **Deployment**: Any changes committed and pushed to the `main` (or `master`) branch of this repository are automatically deployed to `https://huseyinkel.es`.
2.  **Local Development**: To preview changes locally, you can simply open the `.html` files in a web browser. For a more accurate simulation, you can use a simple HTTP server (e.g., `python3 -m http.server` or `npx serve`).
