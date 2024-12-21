---
layout: project-item
title: "HTMX File Download and Playlist Site"
thumbnail: /assets/images/projects/project-playlist-app-nodejs-web-workers.gif
repository: https://github.com/TheAttentionSeeker5050/nodejs-htmx-web-worker-example
---

<p id="heading-p">
    This project demonstrates the use of Node.js, Express, HTMX, and Web Workers to create a file download and playlist web application with a visually engaging progress indicator. The app features a progress wheel animation that fills up as the download progresses, alongside a textual display of the percentage and file size.
</p>

## Features
- Dynamic Progress Animation: A visually engaging download progress wheel fills up based on the download progress.
- File Size Display: Shows the percentage of the file downloaded and the size in MB/KB/GB.
- Web Workers: Background file downloading and progress tracking without blocking the main thread.
- Dynamic Video List: Automatically generates download buttons for video files in the /public/files directory.
- Responsive Design: Styled with a modern green and grayish accent palette using SASS.
- HTMX Integration: Enables dynamic UI updates without full page reloads.

## Technologies Used
- Node.js: Backend server
- Express: Web framework
- HTMX: For dynamic UI updates
- Web Workers: For background processing
- SASS: For styling
- EJS: Template engine