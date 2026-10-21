# Site TODO

Live site: https://kdmalc.github.io (Jekyll, Academic Pages template, deploys from `master`).
Last updated: 2026-10-21

## Priority: missing content

- [ ] **Headshot.** Replace `images/profile.png` (still the template image) with a real photo. Keep the filename, or change `author.avatar` in `_config.yml`.
- [ ] **Public email.** Do not use the Gmail you log in with everywhere. Use the Rice address or a dedicated alias. Set `author.email` in `_config.yml` (currently blank, marked `TODO`).
- [ ] **Project descriptions.** Write 2-4 PhD project summaries (a sentence or two each, plus links), then:
  - add them as files in `_portfolio/` (front matter: `title`, `excerpt`, `collection: portfolio`);
  - uncomment the `Projects` entry in `_data/navigation.yml`.
- [ ] **Check the CV page** (`_pages/cv.md`). It was built from LinkedIn and Google Scholar, so verify:
  - Rice M.S. and Ph.D. wording and dates;
  - Vanderbilt dates (left out on purpose);
  - honors list.
- [ ] **Resume PDF.** Put it in `files/` (for example `files/Kai_Malcolm_CV.pdf`) and link it from `_pages/cv.md` as a download.

## Decisions pending

- [ ] **Other papers.** Not listed yet because details were unclear:
  - "EncoderMoE: Classifying User-Defined Gestures Using MoE Encoders and Meta-Learning" (under review as of May 2026);
  - the 2020 IAC Mars constellation paper (co-author list is long).
  - To add one, create a file in `_publications/` (copy `2026-03-01-federated-emg-decoding.md` as a template).
- [ ] **Unique design.** Send links or screenshots of personal sites you like. Mockups will be made on a separate branch or as preview pages, and nothing replaces the clean site until you approve one.

## Easy extensions

- [ ] **News items** in `_pages/about.md`: new papers, talks, defense dates, job news.
- [ ] **Talks / posters.** Add files to `_talks/` and uncomment `Talks` in `_data/navigation.yml`. (`_talks/` was deleted with the template content; recreate it.)
- [ ] **Teaching** page: same idea with `_teaching/`.
- [ ] **ORCID** link: fill `author.orcid` in `_config.yml`.
- [ ] **Social preview image:** set `og_image` in `_config.yml` so links look good when shared.
- [ ] **Add the Rice lab page or a "Contact" line** to `_pages/about.md`.
- [ ] **Blog / posts:** `_posts/` was removed; add posts and uncomment `Blog Posts` in `_data/navigation.yml` if wanted.
- [ ] **Theme:** try other `site_theme` values in `_config.yml` ("air", "sunrise", "mint", "dirt", "contrast") as a quick restyle.

## Cleanup (low priority)

- [ ] Remove leftover template files: `talkmap.py`, `talkmap.ipynb`, `talkmap_out.ipynb`, `talkmap/`, `markdown_generator/`, `CONTRIBUTING.md`, template text in `README.md`, `_pages/` archive demos you do not use.
- [ ] Verify the site locally (needs `bundler`; not installed on this machine yet): `bundle exec jekyll serve`, then open http://localhost:4000.

## Done

- [x] Site config, name, bio, Rice affiliation, GitHub / LinkedIn / Scholar links
- [x] Removed template publications, talks, teaching, portfolio, posts
- [x] Real publications: TNSRE 2026, spiking neural network review (arXiv 2023)
- [x] Real CV page; fixed the TNSRE link and typo on the About page
- [x] Pushed to `master` (2026-10-20)
