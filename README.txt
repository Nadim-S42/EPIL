EPIL GitHub Pages image fix package

Files:
- index.html
- images/epil-logo.png
- images/hero-bacteria.jpg

Why the images were not showing:
1. The current repository's index.html uses a text/symbol mark instead of an <img> tag for the logo, so the logo file is not displayed.
2. The current repository's hero CSS references images/pathogen-antibiotics-hero.jpg, but the repository listing shows pathogen-antibiotics-hero.jpg at the repository root. The folder/path does not match.

This package has a matching logo <img> reference and hero CSS path to images/hero-bacteria.jpg, with both assets included at those exact paths.

How to publish:
1. Download and extract this ZIP.
2. In GitHub, open https://github.com/Nadim-S42/EPIL
3. Upload index.html and the entire images folder (including both image files) to the repository root.
4. If prompted, replace the existing index.html. Do not upload the images into a nested images/images folder.
5. Commit the changes to the branch used by GitHub Pages (currently main, if that is still the configured branch).
6. Wait for GitHub Pages to rebuild, then hard-refresh https://nadim-s42.github.io/EPIL/ (Ctrl+F5 on Windows).

Important:
This package includes a complete EPIL index.html from the earlier prepared version, not a one-line patch to the currently published HTML. Review the page after replacing index.html to ensure the site content matches the version you want. If you need to preserve the exact current live content, make the two path/markup corrections in the current index.html instead of replacing it wholesale:
- Replace the text-only .brand-mark span with: <img class="brand-logo" src="images/epil-logo.png" alt="Enteric Pathogen Intelligence Lab logo">
- Change both hero CSS references to url("images/hero-bacteria.jpg") OR put the intended pathogen-antibiotics-hero.jpg inside images/ and keep the current CSS reference.
