# Adam Venham-Carter — Engineering Portfolio

A lightweight static engineering portfolio designed for GitHub Pages. No frameworks, package managers, or build tools are required.

## Publish for free with GitHub Pages

### Best URL: `YOUR_USERNAME.github.io`
1. Create a **public** GitHub repository named exactly `YOUR_USERNAME.github.io`.
2. Upload the contents of this folder to the repository root. `index.html` must be at the top level.
3. Commit to the `main` branch.
4. Open **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select **main** and **/(root)**, then Save.
7. Your portfolio will be available at `https://YOUR_USERNAME.github.io/` after GitHub finishes the deployment.

You can also use a normal repository name such as `engineering-portfolio`; the default URL will then include the repository name.

## Customize before publishing

### 1. Contact links
Open `index.html` and replace the placeholder Email, LinkedIn, and GitHub buttons near the bottom of the page.

Example:
```html
<a class="btn primary" href="mailto:you@example.com">Email me</a>
<a class="btn secondary" href="https://www.linkedin.com/in/YOURNAME/">LinkedIn</a>
<a class="btn secondary" href="https://github.com/YOUR_USERNAME">GitHub</a>
```
Remove the `placeholder`, `data-placeholder`, and `href="#"` attributes from the existing buttons.

### 2. Add real project images
Create folders such as:
```
assets/
  freeze-desalination/
  daq/
  vtgt/
  brake-temp/
  cad/
```
Then replace each `.figure-placeholder` block with an `<img>` and caption. Example:
```html
<figure>
  <img src="../assets/freeze-desalination/test-rig.jpg" alt="Freeze desalination experimental test rig">
  <figcaption>Experimental freeze-desalination test rig.</figcaption>
</figure>
```

### 3. Add résumé
Copy your PDF into `assets/` and add a button to the hero or contact section:
```html
<a class="btn secondary" href="assets/Adam-Venham-Carter-Resume.pdf">Résumé</a>
```

### 4. Replace draft language with final quantified results
The current copy is intentionally conservative. Add numbers wherever you can defend them: test ranges, accuracy, weight, temperature, flow, lap time, reliability, number of channels, iteration count, etc.

## File structure
```
.
├── index.html
├── styles.css
├── script.js
├── .nojekyll
├── README.md
├── assets/
└── projects/
    ├── freeze-desalination.html
    ├── daq-system.html
    ├── vtgt.html
    ├── brake-temperature.html
    └── mechanical-design.html
```

## Editing
You can edit the HTML in GitHub's browser editor, VS Code, or any text editor. Most visual changes are controlled by the CSS variables at the top of `styles.css`.

## Privacy check before publishing
Engineering portfolios are public. Remove proprietary/confidential material, private contact information you do not want indexed, unpublished research details that should remain private, and identifying information from drawings/title blocks.
