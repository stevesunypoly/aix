# Contributing to the AIX Center Site

**Artificial Intelligence Exploration Center — SUNY Polytechnic Institute**
Site: [stevesunypoly.github.io/aix](https://stevesunypoly.github.io/aix)
Repo: [github.com/stevesunypoly/aix](https://github.com/stevesunypoly/aix)

---

## Getting Started

1. **GitHub account** — create one at github.com if you don't have one, then ask Steve to add you as a collaborator (Settings → Collaborators)
2. **Clone the repo** to your local machine:
   ```bash
   git clone https://github.com/stevesunypoly/aix.git
   ```

---

## Adding a Project

### 1. Create your project page

Add a new file to the `projects/` directory:

```
projects/your-project-name.html
```

Use any existing project page as a template, or generate one with your favorite AI model. Link `../style.css` for consistent styling.

### 2. Update the projects index

Open `projects/index.html` and add a row to the table following this pattern:

```html
<tr>
  <td><strong><a href="your-project-name.html">Your Project Title</a></strong></td>
  <td>One or two sentence description of what the project is about.</td>
  <td>
    <span class="tag">Tag1</span>
    <span class="tag">Tag2</span>
  </td>
  <td><span class="status-badge status-active">Active</span></td>
  <td>Your Name</td>
</tr>
```

Status options: `status-active`, `status-planning`, `status-complete`

### 3. Add images (optional)

Drop any images into the `images/` directory and reference them as `../images/yourfile.png`.

### 4. Commit and push

```bash
git add .
git commit -m "Add [your project name]"
git push
```

The site updates automatically via GitHub Pages within a minute or two.

---

## Guidelines

- Keep HTML and CSS in the existing style — navy/gold, DM Sans font, `style.css` for everything
- One project per page, one row per project in the index
- No frameworks or build tools — plain HTML/CSS only
- If you're unsure, open a GitHub Issue and ask

---

*Questions? Contact [stevesuny@gmail.com](mailto:stevesuny@gmail.com)*
