# PULSE 249⁴⁹ website

A static website in English and German. All texts, people, events and news live in
`content.json`; the page reads that file and builds itself. No build step, no cookies,
no external fonts or trackers.

## Files

| Path | What it is |
|---|---|
| `index.html` | The website. Reads `content.json`. |
| `content.json` | All content. The admin panel edits this file. |
| `admin/index.html`, `admin/config.yml` | The admin panel (Sveltia CMS) at `yourdomain/admin/`. |
| `uploads/` | Photos, logos, videos and PDFs you upload. |
| `assets/fonts/` | Fonts, served from your own site. |

Keep this folder structure when you upload to GitHub. `admin/index.html` must stay inside
`admin/`; if it lands in the top folder it replaces the website with the panel.

## Preview on your computer

The site loads `content.json`, so open it through a small local server, not by double-click:

```bash
npx serve .        # then open the address it prints
```

## Publish (free hosting)

1. Upload the whole folder to your GitHub repository, replacing what is there.
2. Cloudflare dashboard → Workers & Pages → Create → Pages → connect the repository.
   Leave the build command empty and set the output directory to `/`.
3. Add your domain under Custom domains and follow the DNS step. HTTPS is automatic.

## Admin panel

1. In `admin/config.yml`, replace `YOUR_GITHUB_USERNAME/YOUR_REPO` with your repository.
2. Open `yourdomain/admin/` and sign in with GitHub. Sign-in options are described at
   github.com/sveltia/sveltia-cms; check them there, they can change.
3. Every save in the panel commits to the repository and the live site updates.

## Before going live

- Replace the sample content: team names, partners, address, phone, project and news texts.
- Social links set to `#` are hidden until you enter real addresses.
- Fill in the Impressum under Legal pages (required for sites run from Germany). Its footer
  link appears once the text is filled. Have the Impressum and privacy text checked.
- Logo: the header and footer are dark blue, so use a white or transparent version.

## How things behave

- Language follows the visitor's browser and can be switched in the menu.
- News, departments, people, projects, careers and highlights each open their own page.
- Events show upcoming dates first; past events drop off automatically.
- The contact form and "Apply now" open the visitor's email program with the text filled in.
  A static site cannot send email by itself.
- Front page animation: turn off "Animate the circuit lines" in the panel for a still picture.
