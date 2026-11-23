# Harsha Vardhan Moddu — Portfolio

A responsive personal portfolio for a Computer Science and Engineering undergraduate at IIIT Kottayam. The site presents selected software engineering, full-stack, AI/ML, cybersecurity and open-source work.

## Built with

- Semantic HTML
- CSS custom properties, responsive layouts and motion effects
- Vanilla JavaScript
- GitHub Pages-compatible static hosting

The current implementation intentionally stays framework-free. A React migration is not required for the present scope; the project can be split into modules or migrated later if the product's complexity justifies it.

## Run locally

From the repository root:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000`.

You can also use the Live Server extension in Visual Studio Code.

## Project structure

```text
.
├── index.html
├── resume.html
├── assets/
│   ├── campus-background.webp
│   ├── iiit-kottayam-logo.webp
│   └── profile.webp
└── README.md
```

## Included experiences

- Abstract ambient background with a lightweight particle canvas
- Responsive navigation and dark/light theme
- Interactive terminal-style introduction
- Filterable skills and project collections
- Project case-study dialog with repository and contribution links
- Experience timeline and contact section
- Printable resume page

## Accessibility and performance notes

The interface includes a skip link, visible keyboard focus, keyboard-operable project cards, dialog focus management, accessible mobile-navigation state, and live form validation messages.

Motion-sensitive preferences are respected. The particle animation pauses when the browser tab is hidden, uses a lower particle budget on small screens, and is disabled for reduced-motion users. Reveal animations use `IntersectionObserver` and remain progressively enhanced so content is not hidden when JavaScript or the observer is unavailable.

## Contact form behavior

The contact form validates the visitor's details and opens their configured email application with a prepared message addressed to the portfolio owner. It does **not** send or store messages on a server. The visitor must press Send in their email application.

## Content accuracy

Project descriptions distinguish personal projects from collaborative contributions. SatQuery AI is presented as a project concept under SIH 2026 Problem Statement 26167; it is not described as shortlisted. The InterviewAI entry links directly to the merged contribution.

## Manual release checklist

Before publishing a release, verify:

- [ ] Test the page at 360px, 390px, 768px, 1024px and a wide desktop viewport.
- [ ] Navigate all interactive elements using Tab, Shift+Tab, Enter, Space and Escape.
- [ ] Open and close every project dialog; confirm focus returns to its card.
- [ ] Test project and skill filters after scrolling.
- [ ] Test dark/light theme persistence and storage-disabled behavior.
- [ ] Test with reduced motion enabled and with the browser tab hidden/restored.
- [ ] Validate contact form errors and the generated email draft.
- [ ] Check external repository, LinkedIn and resume links.
- [ ] Run Lighthouse and an accessibility audit in the target browser.
- [ ] Confirm the deployed site and printable resume render correctly.

## Deployment

The site is static and can be hosted with GitHub Pages. Configure the repository's Pages source to the intended branch/folder and use the deployed URL as the canonical URL only if that remains the production address.
