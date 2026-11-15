PULSE 249-49 website – how to publish and edit

FILES
  index.html      the website (do not edit)
  content.json    ALL texts, people, events, news (the admin panel edits this)
  admin/          the control panel  ->  yourdomain.com/admin
  uploads/        photos, logos, videos you upload

PUBLISH (about 15 minutes, free)
 1. Create a GitHub account and a new repository. Upload everything in this folder to it.
 2. Create a Netlify, Cloudflare Pages or GitHub Pages site connected to that repository.
    Every change you save in the panel will update the live site automatically.
 3. Buy your domain and connect it in the hosting settings.
 4. Open admin/config.yml and replace YOUR_GITHUB_USERNAME/YOUR_REPO with your repository.
 5. Go to yourdomain.com/admin and sign in with GitHub.
    (Steps for the panel (Sveltia CMS) are on its GitHub page: github.com/sveltia/sveltia-cms. Check them there, they can change.)

USE THE PANEL
  Add a news item, event, person, department, picture, video or PDF with forms – no code.
  Every text has an English and a German field.
  Logo: Website > Logo.

LOGO
  Panel: Website > Logo. Or put the file in uploads/ and write "logo":"/uploads/logo.png" in content.json.
  The header and footer are dark blue, so use a WHITE or transparent-background version of the logo.
TOP BANNER
  Website > Top banner. Leave both fields empty = no banner.
ANIMATION
  Website > Front page picture/video > turn off "Animate the circuit lines" for a still picture without the pause button.

NEW SECTIONS (all editable in the panel)
  Highlights   picture tiles; each opens its own page with full text
  News         categories (meetings, research, seminars, press...) with filter buttons, full article pages, video/PDF
  Projects     research projects with status, partners, department, own page
  Training & Careers   jobs / training / internships / volunteering; each has a page and an "Apply now" button
               (application form link, or email - the email is pre-filled with subject and template)
  FAQ          unlimited questions, searchable
  Contact      several contact persons + a message form
  Section titles   rename any section and its menu name
