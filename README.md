<<<<<<< HEAD
﻿# Cush Jabez P. Nuñeza — Internship Portfolio

A responsive, matte black portfolio built with React, Vite, JavaScript, and Tailwind CSS v4 (available in the project setup). Content lives in small data files so you can update it without hunting through page markup. The contact form currently validates locally and does not send messages until you configure a service.

## Technology

- React and JavaScript
- Vite
- Tailwind CSS v4 / CSS custom properties
- ESLint
- Inline SVG icons (no icon dependency required)

## Run locally

```bash
npm install
npm run dev
```

Open the local URL printed by Vite. To create a production build or run ESLint:

```bash
npm run build
npm run lint
```

## Where to edit

- `src/data/personalInfo.js`: name, title, introduction, About Me text, email, location, social profile URLs, photo path, and resume path.
- `src/data/skills.js`: skill category names, descriptions, and tags.
- `src/data/projects.js`: project information, screenshot paths, technologies, contribution, and actual project/repository URLs. Empty URLs hide the respective links.
- `src/data/certificates.js`: add certificate objects only for credentials you have earned. Include `title`, `issuer`, `date`, `description`, and `image`.
- `src/data/experience.js`: experience and leadership entries, duration, responsibilities, and related skills.
- `src/data/education.js`: university, degree, college, status, location, and logo path.
- `src/App.jsx`: page sections, navigation list, contact-form integration point, and interactive behavior.
- `src/App.css`: layout, component styles, breakpoints, and animations.
- `src/index.css`: the palette variables and global styles.

## Add your assets

- Profile photo: replace/add `public/images/profile.jpg`.
- University logo: replace/add `public/images/buksu-logo.png`.
- Project screenshots: put files in `public/images/projects/` and update the matching path in `src/data/projects.js` (for example `oncocare.png`).
- Certificates: put image files in `public/certificates/`, then add their details and `/certificates/your-file.png` paths in `src/data/certificates.js`.
- Resume: put your real PDF at `public/documents/Cush-Jabez-Nuneza-Resume.pdf`, or update `resumePath` in `src/data/personalInfo.js`.

Public files are referenced by paths beginning with `/`, such as `/images/profile.jpg`. Missing photos, logo, project images, or certificates have a visible fallback state.

## Contact form setup

The form currently uses browser required-field and email validation only. In `src/App.jsx`, replace `submitForm` with an integration to your chosen email service or API. Add the service's loading and error handling there; do not publish secret API keys in client-side code. No message is sent by the current form.

## Palette and navigation

Edit the CSS custom properties at the top of `src/index.css` to adjust the colors. Edit `navItems` in `src/App.jsx` to change section links; section IDs must match their navigation targets.

## Deploy

Run `npm run build`, then deploy the generated `dist/` folder to a static host such as GitHub Pages, Netlify, or Vercel. For GitHub Pages, set the Vite `base` option in `vite.config.js` to your repository subpath if required by your deployment URL. A future API can be integrated behind the contact form without changing this frontend's content structure.

## Project structure

```text
public/
  images/                 profile, university logo, and project screenshots
  certificates/           certificate scans
  documents/              resume PDF
src/
  data/                    editable personal and portfolio content
  App.jsx                  reusable UI and page sections
  App.css                  responsive component and layout styles
  index.css                global styles and color palette
  main.jsx                 React application entry point
index.html                 SEO metadata and app mount point
```
=======
# Portfolio
>>>>>>> f7441bb7081621e82efe2395642ad9dfe35e575a
