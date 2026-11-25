# Tyrone Darby | Developer Portfolio

A personal portfolio website showcasing Tyrone Darby's Java backend development projects, software quality assurance experience, and computer science background. It gives recruiters, engineering teams, and collaborators a place to explore his work, download his resume, and get in touch.

The design pairs an illustrated profile portrait with an ink-blue, white, and lavender palette, clear typography, and responsive layouts for desktop and mobile.

## Features

- Introduction highlighting Java, Spring Boot, and secure backend development.
- Featured projects with technology tags and expandable implementation details.
- Professional experience at Youbloom and grouped technical skills.
- Education and Spring Boot, Spring Framework, and Hibernate certification details.
- Downloadable PDF resume and direct email, GitHub, and LinkedIn links.
- Copy-email button with confirmation feedback and a fallback message.
- Mobile navigation with keyboard support, a skip-to-content link, visible focus styles, and reduced-motion support.
- Page metadata, social sharing metadata, and a custom SVG favicon.

## Featured projects

### Customer Relationship Management Application

A full-stack CRM application featuring authenticated customer management, RESTful CRUD endpoints, role-based authorization, and MySQL persistence. The portfolio explains its Spring Boot, Spring Security, Spring Data JPA, and Hibernate architecture through a labeled system illustration.

### ToDoList - JavaFX Task Manager

A lightweight desktop task manager built with Java, JavaFX, and CSS. The project uses custom VBox and ScrollPane layouts, dynamically updating task cards, and custom styling without third-party UI libraries.

[View the ToDoList source code](https://github.com/tyronedarby/ToDoList).

The project visuals on the portfolio are labeled illustrations. The applications themselves are separate projects and are not included in this repository.

## Technology

| Technology | Purpose |
| --- | --- |
| HTML5 | Page content, semantic sections, and native expandable project details |
| CSS3 | Layout, responsive breakpoints, colors, typography, and illustrations |
| Vanilla JavaScript | Mobile navigation and copy-email interaction |
| Node.js built-in modules | Optional local HTTP preview server |

The website has no third-party runtime dependencies, package installation, or build step. Its images, stylesheet, script, favicon, and resume are stored locally. Contact links open an email client or external profile; the site does not include a contact-form backend.

## Project structure

```text
tyrone-portfolio/
|-- dist/
|   |-- assets/
|   |   |-- favicon.svg
|   |   |-- tyrone-darby.jpg
|   |   `-- Tyrone-Darby-Resume.pdf
|   |-- index.html
|   |-- styles.css
|   `-- script.js
|-- serve.mjs
|-- DESIGN.md
|-- README.md
`-- .gitignore
```

`dist/` contains the editable website source and is also the directory to deploy. `DESIGN.md` documents the visual direction and layout decisions.

## Run locally

For a quick look, open `dist/index.html` directly in a browser.

For an HTTP preview, install Node.js if needed, open a terminal in the `tyrone-portfolio` directory, and run:

```sh
node serve.mjs
```

Visit [http://127.0.0.1:4173](http://127.0.0.1:4173). Stop the server with `Ctrl+C`. Refresh the browser after editing files; the preview server does not provide live reload.

The copy-email feature uses the browser Clipboard API, which requires a supported secure context such as HTTPS or localhost. If clipboard access is unavailable, the page displays alternative instructions.

## Customize

| File | What to change |
| --- | --- |
| `dist/index.html` | Introduction, projects, experience, skills, education, contact links, and metadata |
| `dist/styles.css` | Color variables, fonts, spacing, responsive layouts, and project illustrations |
| `dist/script.js` | Navigation behavior, copied email address, and feedback messages |
| `dist/assets/tyrone-darby.jpg` | Profile picture |
| `dist/assets/Tyrone-Darby-Resume.pdf` | Downloadable resume |
| `dist/assets/favicon.svg` | Browser tab icon |

When changing the email address, update both the links in `index.html` and the clipboard value in `script.js`. Keep asset references and download links in sync if filenames change.

## Deployment

Deploy the contents of `dist/` to a static web host, preserving the asset paths. No application server or database is required for the portfolio.

Before publishing, update the absolute `og:image` URL in `dist/index.html` to match the deployed domain. The existing metadata URL is not confirmation of a live deployment.

## Contact

- **Email:** [tyronedarby18@gmail.com](mailto:tyronedarby18@gmail.com)
- **GitHub:** [tyronedarby](https://github.com/tyronedarby)
- **LinkedIn:** [Tyrone Darby](https://www.linkedin.com/in/tyrone-darby-50a230367)
