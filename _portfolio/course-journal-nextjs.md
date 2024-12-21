---
layout: project-item
title: "Next.js Course Journal"
thumbnail: /assets/images/projects/project-course-journal-nextjs.png
repository: https://github.com/TheAttentionSeeker5050/nextjs-teachers-course-journal
---
<p id="heading-p">This full-stack application is a fork of one of my own GitHub organization’s projects, developed in collaboration with my colleague Oladoyin.</p>

## Overview:
The Course Grid Project is a comprehensive journaling web app designed specifically for faculty teachers. It enables teachers to perform CRUD operations on courses, lessons, and units, manage course notes, and upload file attachments. This functionality empowers teachers to track their practices, evaluate student reception and outcomes, and continuously improve their teaching methods.

## Technologies Used:
- **Frontend:** Next.js, Tailwind CSS, Font Awesome icons
- **Text Editor API:** TinyMCE
- **Authentication:** JSON Web Tokens (JWT)
- **Backend:** Prisma database ORM, PostgreSQL database system, Docker Compose
- **Testing Suite:** Jest for CRUD transactions, validation, and token authentication methods
- **Data Validation:** Zod
- **File Storage:** Multer

## Build Instructions:
1. Install dependencies: `npm install`
2. Run Docker Compose: `docker compose up -d`
3. Push database changes: `npx prisma db push`
4. Update .env file:
    1. Copy the key entry from `TEST_DATABASE_URL`
    2. Replace the database URL in `.prisma/schema.prisma` with this key name:
  ```javascript
// in prisma/schema.prisma
datasource db {
  provider = "postgresql"
  url = env("TEST_DATABASE_URL")
}
```
5. Push database changes again: `npx prisma db push`
    1. Revert the database URL change in `.prisma/schema.prisma` back to `DATABASE_URL`
```javascript
// in prisma/schema.prisma
datasource db {
  provider = "postgresql"
  url = env("DATABASE_URL")
}
```
6. Run tests: `npm run test`
7. Run local development build: `npm run dev`

For cloud deployment, use `npm run build` and `npm run start`. Ensure that your cloud infrastructure provider supports these commands. Note that this project requires Node.js version 20 for development and deployment.

**Note:** Please keep in mind that in the live version of the Course Grid Project, some images and files may not load properly, displaying default placeholder images or indicating “image not found.” Additionally, users are required to create an account to access the app’s features. There is no email confirmation required, allowing the creation of a burner account for testing purposes.

Forked from [NSCC-IT-Web-Capstone-Project-Ola-Nick/capstone-course-grid-development-repo](https://github.com/NSCC-IT-Web-Capstone-Project-Ola-Nick/capstone-course-grid-development-repo){:target="_blank"}
