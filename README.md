# Hadisa Abroo, personal academic website

Live at **https://hadisaabroo99-pixel.github.io/Hadisa-Portfolio/**

The site is one self-contained file, `index.html`. Styling, animations, fonts (Inter and Source Serif 4, SIL Open Font License), the portrait, and the CV previews are all built in.

| File | Purpose |
| --- | --- |
| `index.html` | The website |
| `404.html` | Page shown for broken links |
| `Hadisa_Abroo_CV.pdf` | CV behind every download and view button |
| `og-image.jpg` | Preview card when the link is shared on LinkedIn, WhatsApp, or email |
| `apple-touch-icon.png` | Icon when the site is saved to a phone home screen |
| `sitemap.xml` | Lets Google Search Console index the site |

## Adding the DOI to the published paper

The Physica B article is live. Once you have its DOI from the ScienceDirect page (under the title, in the form `10.1016/j.physb.2026.xxxxxx`), search `index.html` for `sciencedirect.com/science/article/abs/pii/S0921452626011154` and replace that address with `https://doi.org/10.1016/j.physb.2026.xxxxxx`. A DOI link never breaks, whereas publisher URLs sometimes change. Add the volume and article number to the `<p class="ve">` line in the same block when the issue is assigned.

## Publishing

1. In the **Hadisa-Portfolio** repository, click **Add file → Upload files → choose your files**, select all files, and click **Commit changes**. Files with the same name are replaced.
2. Delete `robots.txt` from the repository if it is still there. It only works at a domain root, so it has no effect on this site.
3. Check **Settings → Pages**: Deploy from a branch, `main`, `/ (root)`.
4. After one to three minutes, open the address above in a private window.

If you ever rename the repository, replace `https://hadisaabroo99-pixel.github.io/Hadisa-Portfolio/` in `index.html`, `404.html`, and `sitemap.xml` with the new address.

## Updating

- **New CV:** upload a PDF named exactly `Hadisa_Abroo_CV.pdf`. The page previews in the CV section are images, so ask for them to be regenerated after major CV changes.
- **Paper links:** each paper is one `<li class="pub">` block in `index.html`. Each already links to its GitHub repository and a full-text request. Add an arXiv or DOI link inside `<div class="side">`:

  ```html
  <a class="link act" href="https://arxiv.org/abs/XXXX.XXXXX" target="_blank" rel="noopener">arXiv<svg class="i"><use href="#i-arrow"/></svg></a>
  ```

  When a paper is accepted, change the badge text (for example to `Published`) and replace "Submitted to" with the journal reference and DOI. Check with co-authors and the journal's preprint policy before posting a co-authored manuscript that is still under review.
- **Abstracts:** only the published Physica B paper shows an abstract, in `<div class="abs" id="abs-qdm">`. The other papers deliberately show no abstract and no summary of results, only the title, authors, venue, and a "Request manuscript" button, so unpublished findings stay private until each paper is timestamped on arXiv or published. To publish an abstract later, copy the `abs-t` button and `abs` panel from the Physica B entry.
- **Removing a paper:** delete its whole `<li class="pub">…</li>` block, then update the count in the facts row (search for `First author on five`).
- **Status line:** search for `Seeking PhD positions` in `index.html`.
- **Request buttons:** each paper's `.reqbtn` link opens an email pre-filled with that paper's title. If you change a title, update the `subject=` and `body=` text in its link too.
- **Supervisor panel:** the availability, funding, languages and interests block sits in `<dl class="supgrid">` in the contact section. Update the funding line as soon as a scholarship application is in progress.
- **Research direction:** the three "Where I want to take this" items are in `<ol class="next-list">`. Rewrite these in your own words before applying to a specific group, and tailor them to that group's work.
- **Research figures:** replace a `<svg id="fig-...">...</svg>` block with `<img src="your-figure.png" alt="Description">` after uploading the image.
