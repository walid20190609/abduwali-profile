# Abduwali Moallim — Personal Profile Site

This repository is a simple static personal profile site for Abduwali Moallim. It contains a single-page resume-style site with contact details, skills, and a short bio.

Files
- `index.html` — the main profile page (updated with improved markup and accessibility)
- `style.css` — site styles (merged with improved layout and navigation)

Quick notes and suggested improvements
- Add real links for LinkedIn and other profiles (they're currently set to the LinkedIn profile and GitHub).
- Consider adding a small photo (use `img` with `alt` text and prefer a WebP or optimized JPEG).
- Improve SEO: add structured data (JSON-LD) for Person and add Open Graph/Twitter Card meta tags.
- Make the site responsive and test on small screens — current CSS includes basic responsiveness.
- Consider deploying to GitHub Pages or Netlify for a quick live site.

Small checklist of actionable improvements
- [ ] Replace placeholder certifications with actual credentials.
- [ ] Add a lightweight contact form (with a spam-protection method) or anonymized contact link.
- [ ] Add semantic HTML landmarks (role/aria) where helpful (already present in header/main/nav).

If you want, I can:
- add a hero image and optimize it;
- add Open Graph meta tags and JSON-LD for better sharing;
- scaffold a simple contact form that posts to Formspree or Netlify Forms;
- prepare a GitHub Pages workflow and brief README with deployment steps.

Deployment (GitHub Pages)
-------------------------
- A GitHub Actions workflow was added at `.github/workflows/deploy.yml` that publishes the repository to the `gh-pages` branch on push to `main`.
- After pushing to `main`, GitHub Actions will run and publish the repository root as a static site. By default the site will be available at:

	https://<your-github-username>.github.io/abduwali-profile/

Notes & required edits before going live
- Replace the Formspree action URL in `index.html` (`https://formspree.io/f/your-id`) with your Formspree form ID or connect a different form backend.
- Confirm the `og:url` and JSON-LD `url` values in `index.html` match your final publishing URL.
- Optionally enable GitHub Pages in the repository settings and point it at the `gh-pages` branch (Actions also creates this branch).

If you'd like, I can handle the last mile: replace the Formspree ID, test the form submission, and verify the GitHub Pages deployment once you confirm the Formspree ID and that you're OK with using `gh-pages` for publishing.

