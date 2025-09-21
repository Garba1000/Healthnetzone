
Health Netzome - Netlify-ready static site with Netlify CMS admin scaffold
-----------------------------------------------------------------------

Contents:
- index.html (home)
- articles/ (pre-generated HTML articles)
- articles_markdown/ (markdown source compatible with Netlify CMS)
- about.html, privacy.html, terms.html
- about.md, privacy.md, terms.md (for Netlify CMS editing)
- admin/ (Netlify CMS admin index and config.yml)
- styles.css

Important setup notes:
1) Upload this project to a GitHub repository (create a new repo and push the files).
2) In admin/config.yml, change 'repo' to YOUR_GITHUB_USERNAME/YOUR_REPO_NAME and the branch if different.
3) In Netlify, add your site (connect to GitHub) and enable Netlify Identity and Git Gateway (for CMS auth),
   or configure GitHub OAuth per Netlify CMS docs.
4) Point your domain (healthnetzome.tzy) to Netlify using DNS instructions.
5) When Netlify builds the site, the markdown files in 'articles_markdown' will be available to edit in /admin.
6) For AdSense approval, ensure you keep the site content original, add a Privacy Policy, About page, and contact info.
7) If you want dynamic HTML pages generated from markdown automatically, add a build step (eleventy/hugo) in the future.
