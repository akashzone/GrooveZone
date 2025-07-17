# GrooveZone AI Coding Agent Instructions

## Project Overview

GrooveZone is a static web application for a music player interface. The codebase consists of HTML, CSS, and JavaScript files, with assets for icons and images. There is no build system, backend, or test framework present.

## Key Files & Structure

- `index.html`: Main entry point. Defines the UI structure, including header, navigation, search bar, and placeholders for sidebar, main content, and footer.
- `style.css`: Contains all styling rules. Pay attention to selector specificity and order for overrides (e.g., button color issues).
- `script.js`: Reserved for interactive features (currently empty or minimal).
- `Assets/`: Contains all images and icons used in the UI.

## Patterns & Conventions

- **CSS Specificity**: Later rules override earlier ones. Use class selectors (e.g., `.nav-2 .btn-2`) for targeted styling. Inline styles in HTML may override CSS file rules.
- **Font Awesome**: Icons are used via CDN. Reference with `<i class="fa-...">` in HTML.
- **Responsive Design**: Uses rem units and flexbox for layout. Check `style.css` for flexbox usage in header and navigation.
- **No Frameworks**: Pure HTML/CSS/JS. No React, Vue, or build tools.
- **No Automated Workflows**: No build, test, or lint commands. All changes are manual and visible on page reload.

## Common Tasks

- **UI Changes**: Edit `index.html` for structure, `style.css` for appearance. Use browser dev tools to debug CSS issues.
- **Asset Management**: Add new images/icons to `Assets/` and reference with relative paths in HTML/CSS.
- **Interactivity**: Add JavaScript to `script.js` and link via `<script src="script.js"></script>` in `index.html`.

## Examples

- To make a button round: Use `border-radius: 50%` in CSS.
- To override button color: Place `.nav-2 .btn-2 { ... }` after `.nav-2 button { ... }` in `style.css`.
- To add an icon: `<i class="fa-solid fa-house"></i>` for a home icon.

## Integration Points

- **External**: Font Awesome CDN for icons, Google Fonts for typography.
- **No API/Backend**: All data and UI are static.

## Troubleshooting

- If a style does not apply, check selector specificity and order in `style.css`.
- For missing assets, verify the path and file existence in `Assets/`.

---

For questions about missing features, unclear patterns, or expanding functionality, ask the user for clarification or examples from similar projects.
