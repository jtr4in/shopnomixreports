# AI Rules for shopnomixreports

This document outlines the technical guidelines and conventions for developing the `shopnomixreports` application.

## Tech Stack Description

*   **HTML5:** Used for structuring the content and defining the user interface.
*   **CSS3:** Used for styling the application, currently implemented via an inline `<style>` block.
*   **Vanilla JavaScript:** Used for all interactive elements and dynamic behavior. No external JavaScript frameworks or libraries are currently in use.
*   **Browser-based Application:** The application runs entirely in the browser, with no server-side components.
*   **Direct API Calls:** Reports are downloaded by directly opening URLs to an external API in a new tab.

## Library Usage Rules

*   **Core Technologies:** Prioritize the use of native HTML, CSS, and Vanilla JavaScript for all new features and modifications.
*   **Styling:** Continue to use plain CSS for styling. If the application grows, consider external CSS files or a CSS preprocessor if explicitly requested by the user.
*   **JavaScript:** All interactivity should be implemented using Vanilla JavaScript. Avoid introducing new JavaScript frameworks (e.g., React, Vue, Angular) or large libraries unless there's a clear, explicit request from the user and a strong justification for their necessity.
*   **Minimal Dependencies:** Strive to keep the project dependency-free. If a specific utility or feature absolutely requires a third-party library, propose it to the user with a clear explanation of its benefits and impact.
*   **No Build Process:** Currently, there is no build process (e.g., Webpack, Vite). Maintain this simplicity unless a build tool is explicitly requested for more complex development needs.
*   **API Interaction:** Continue to use direct `window.open()` for downloading reports. If more complex asynchronous data fetching is required, use native `fetch` API.