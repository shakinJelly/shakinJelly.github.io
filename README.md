# Zhicong Hong

English-language academic homepage: [shakinjelly.github.io](https://shakinjelly.github.io/).

## Template

The page follows [Dani El-Ayyass's README template](https://github.com/dayyass/dayyass/blob/main/README.md), listed in [Awesome GitHub Profile README](https://github.com/abhisheknaiidu/awesome-github-profile-readme#descriptive-):

1. A short greeting.
2. **Education**: one list item per university, placed before work experience.
3. **Work experience**: the original four-column structure, `Job Position | Company | Field | Work Period`.
4. **Achievements**: a plain list.

The previously requested fixed personal sidebar is retained. The content uses an unmodified copy of [github-markdown-css](https://github.com/sindresorhus/github-markdown-css) for standard GitHub Markdown rendering. There are no custom document frames, badges, research tags, or animations.

Sections from the example that have no corresponding personal information are omitted.

## Content organization

- School information belongs in **Education**. Each university's degree, dates, department, supervisor, and research are kept together in its own entry.
- Internship information belongs in **Work experience**. Each employer's role, location, dates, and tasks appear in a single table row.
- Awards appear only in **Achievements**.
- The personal sidebar contains the portrait, name, GitHub handle, contact links, and section navigation.
- Avoid repeating institution-specific research in the greeting or a separate research summary.
- The contact email is `zhicong.hong@connect.polyu.hk`.
- Preserve confirmed dates; do not infer an end month for the completed Shanghai AI Lab internship.
- Keep the entire page in English.

## Local preview

From the repository directory:

```sh
python -m http.server 8000 --bind 127.0.0.1
```

Open <http://127.0.0.1:8000/>. Press Ctrl+C to stop the server.

The page also works when opening `index.html` directly. There is no build step or runtime JavaScript.

## Files and maintenance

- `index.html`: personal content, HTML template, and the minimal sidebar/layout CSS.
- `photo.jpg`: portrait, with its natural width and height declared in the HTML.
- `assets/github-markdown-light.css`: unchanged upstream stylesheet, pinned to commit `7f38dcb9054bc5d860fac65291f5c98fef47932c`.
- `assets/github-markdown-css.LICENSE`: the upstream MIT license.

Update the visible email and `mailto:` link together. Keep the page title and social descriptions consistent with the content.

At widths of 900px or less, the sidebar becomes a normal page header. Tables retain the template's standard Markdown layout and can scroll horizontally within their bounds on narrow screens.

The `#internships`, `#education`, and `#awards` links remain unchanged. The earlier `#about` and `#research` links resolve to the greeting.

Continue using the existing GitHub Pages configuration. Local edits do not automatically commit or push the site.
