# Marta O'Toole — portfolio

Static portfolio site. Plain HTML/CSS/JS, no build step, no dependencies.
Intended for deployment to GitHub Pages (not yet deployed).

Visual system: white ground, deep navy (`--navy-ink #0f2942`), teal accent
(`--teal #17877b`), occasional blue. Tokens + components live at the top of
`assets/css/style.css` (buttons, tags, status pills, cards, metric blocks,
check-lists, screenshot frames, section labels). Icons are inline SVGs.

## Structure

```
index.html                              Homepage (hero, AI builds, transformation, about, contact)
case-studies/
  discovery-os.html                     Discovery OS case study (written)
  enterprise-cpd-ai-assistant.html      Enterprise CPD AI Assistant case study (written)
assets/
  css/style.css                         All styles
  js/main.js                            Mobile nav toggle + footer year
  img/
    portrait.jpg                          Hero portrait, 900x900 (downscaled for web from a user-supplied image)
    (Discovery OS screenshots, copied from OS Discovery/screenshots/):
    process-map.png                       <- Process Map.png       (case-study hero + homepage feature)
    discovery-os-as-is.png                <- As Is.png
    discovery-os-pain-point.png           <- Pain Points.png
    discovery-os-gap.png                  <- Gaps.png
    discovery-os-requirement.png          <- Requirements.png
    cpd-ai-assistant-synthetic.png        Synthetic representative chatbot visual for the CPD case study
                                          (downscaled from a user-supplied ChatGPT mockup; not a real interface)
```

## Run locally

```bash
python -m http.server 8000
```

Then open http://localhost:8000

## Still to do

- All LinkedIn/email links are live across the homepage and both case studies.
- Both case studies are written. `cpd-ai-assistant-synthetic.png` is a stand-in synthetic visual — swap if a more polished one is produced (keep it clearly synthetic; no real EY screens).
- To swap the hero portrait, replace `assets/img/portrait.jpg` (square, ~900px+, subject centred works well).
