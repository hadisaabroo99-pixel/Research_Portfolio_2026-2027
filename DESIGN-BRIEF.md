# Design brief: academic website for Hadisa Abroo

Use this brief when updating the site or asking a designer or AI tool for changes, so every version keeps the same direction.

## Objective

Create a personal academic website that persuades principal investigators and PhD admissions committees, within 30 seconds, that Hadisa Abroo is a serious, well-prepared candidate in theoretical quantum physics, and makes it effortless to read her work, download her CV, and contact her.

## Primary audience

Professors and senior researchers in quantum optics, quantum sensing and metrology, and non-Hermitian physics, in Germany, Canada, the United Kingdom, Australia, and Ireland. They are time-poor, skeptical of exaggeration, and typically scan a candidate page for four answers, in this order:

1. **Who is this?** Name, career stage, field, and current goal.
2. **Is she a fit for my group?** The research questions and methods.
3. **What is the evidence?** Manuscripts, venues, honest status, co-authors, and code.
4. **How do I act?** CV and email, reachable in one click from anywhere.

## Content principles

- One idea per section, and short sentences. Every claim must be verifiable from the CV.
- Report publication status exactly (submitted, under review, in preparation). Never inflate.
- Publish full abstracts only for work already in a journal's review system or timestamped on a preprint server. For unpublished manuscripts, show the research question alone and offer the full text on request.
- Show physics visually. Figures and a single equation earn more trust than adjectives.
- Lead every manuscript with the question it answers, then let the full abstract expand for readers who want depth. Professors decide on the question; reviewers read the abstract.
- Keep grades, certificates, phone number, and referee names off the public site.

## Page structure

1. **Hero:** status, name, one-sentence research identity, Download CV, Explore research, ORCID, GitHub, LinkedIn.
2. **Research statement:** one sentence that defines the central question, three facts (including first authorship on all manuscripts), and research-interest keywords for quick fit-scanning.
3. **Featured project:** exceptional-point sensing, told in three scroll-driven steps with a live eigenvalue plot.
4. **Other research:** three concise cards, each with a figure.
5. **Publications:** year, title, authors, venue, and status, each with the central research question in one line, a full abstract that expands on demand, a link to the supporting code repository, and a full-text request link.
6. **Open-source code:** public repositories only.
7. **Background:** education, research experience, and methods and tools as simple rows.
7b. **Research direction:** three concrete things the candidate wants to do next in a PhD, so the reader sees forward intent, not only past work.
8. **CV:** a dedicated card with page previews, format, length, size, and date, plus download and view buttons.
9. **Contact:** email with a copy button, a supervisor-facing panel (availability, funding position, location, languages, interests, and what the candidate adds to a group), and CV, LinkedIn, and ORCID links.

## Visual system

- **Style:** Apple and Google product-page restraint. Generous whitespace, large confident type, few elements, no decorative clutter.
- **Colour:** near-black background (#0A0B0E), primary text #F5F5F7, secondary #A1A1AA, a single teal accent (#4FC3C0) for links and data, and amber (#F2A65A) reserved for the PhD status and the exceptional point.
- **Typography:** Inter for all text (bold, tightly tracked headlines; relaxed body text); Source Serif 4 italic only for mathematics.
- **Portrait:** a studio headshot in a rounded 4:5 card with a slowly rotating light border (teal into amber), a floating glass caption, and a Bloch sphere turning behind it.

## Motion

Motion should feel physical and calm, and every animated element should relate to quantum physics.

- **Background:** a 3D field of points rippling with two-source interference, the pattern behind the double-slit experiment. Scrolling slowly turns and tilts the field; it dims behind reading sections and brightens again at the contact section.
- **Portrait:** the card enters with a 3D tilt-up, floats gently, and tilts toward the cursor with a moving light sheen. Behind it, a Bloch sphere rotates while a qubit state precesses around the z axis, leaving a fading trail.
- **Scroll:** the hero recedes in depth as the visitor scrolls away. Sections rise into place with a 3D tilt; research and code cards tilt under the cursor.
- **Research statement:** lights up word by word as it scrolls into view.
- **Featured project:** scrolling sweeps the coupling in the eigenvalue plot while the figure turns slightly in 3D, so the visitor watches the exceptional point form.
- Everything respects the visitor's "reduce motion" setting, and animations pause when the tab is hidden.

## Technical requirements

Single self-contained HTML file hosted on GitHub Pages; works on phones; fast to load; accessible (keyboard focus, alt text, sufficient contrast); every link and download verified before publishing.
