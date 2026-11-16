# veliyat.com

Personal site of Ravi Veliyat. Plain HTML and CSS: no JavaScript, no build step, no third-party requests.

## Preview locally

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000. Run it from the repository root, because links are root-relative.

## Structure

```
index.html            Home
work/index.html       Work
teaching/index.html   Teaching
videos/index.html     Videos
about/index.html      About
resume/index.html     Resume
404.html              404 Not Found
assets/css/site.css   The one stylesheet
assets/img/           Images
```

Header, navigation and footer markup is identical on every page. If you change one, change all.

## Site address

`https://veliyat.com` is used in the canonical, Open Graph and JSON-LD tags. Each page keeps these in a block marked `SITE-ADDRESS`.

## Open items

Waiting on Ravi:

- [ ] Portrait file for Home and About (alt text: "Portrait of Ravi Veliyat"). A fixed 176 × 220 px space is reserved on both pages.
- [ ] Three selected videos for Home: titles and YouTube URLs. Thumbnails are downloaded once and stored in `assets/img/`.
- [ ] Social image `assets/img/social.jpg` (1200 × 630): review the generated one.

Needed for later rounds:

- [ ] Work: update the Optivo launch-status sentence when Optivo goes live.
- [ ] Work: confirm the AI Coding Tutor live demo is running and supply its URL.
- [ ] Videos: exact titles, URLs and group for each video.
- [ ] Resume: replace the PDF on Google Drive before the site goes live.
- [ ] Re-check the Fightrons wording against fightrons.com before launch.
