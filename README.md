# CX Presentation System

The governed system for building customer-experience presentations with Claude. It includes story structures, slide templates, components, device frames, story rules and the **CX Presentation Design System** (Abbott palette).

**Documentation site:** https://YOUR-USERNAME.github.io/cx-presentation-system/ *(replace with your GitHub Pages link once it's live)*

## Download

| File | What it is |
|---|---|
| [CX_Presentation_System_Starter_v0.1.zip](downloads/CX_Presentation_System_Starter_v0.1.zip) | Everything needed to build a deck with Claude: `START_HERE.md`, the `.md` spec, the registry `.json`, 7 template decks, 111 icons, device frames, tokens and the sample deck |
| [CX_Presentation_Design_System.zip](downloads/CX_Presentation_Design_System.zip) | Design system source: tokens, components, guidelines |
| [Cologuard_Rescreen_Concept_v2.pptx](downloads/Cologuard_Rescreen_Concept_v2.pptx) | Sample deck built with the system (dummy data) |
| [downloads/templates/](downloads/templates/) | The 7 template decks as separate .pptx files |

You can also read the spec files directly:

- [files/START_HERE.md](files/START_HERE.md): how to use the system with Claude, with copy-paste prompts
- [files/cx-presentation-system.md](files/cx-presentation-system.md): the governing spec
- [files/cx-presentation-registry.json](files/cx-presentation-registry.json): every ID and status, machine-readable

## Build a deck with Claude in 3 steps

1. Download the starter zip and unzip it.
2. In Claude, create a Project and add the three files in `ai-upload-pack/` to its knowledge. For a one-off deck, upload them to a chat instead.
3. Paste the deck prompt from `START_HERE.md`. Claude proposes the story first and builds the `.pptx` only after you reply "approved".

## What's in this repository

```text
index.html     the documentation site (static, no build step)
tokens.css     CX Presentation Design System tokens
bundle.css     component styles
js/            in-browser deck generator (pptxgenjs, JSZip)
img/ files/ ds/  previews, icons, device frames, spec files, component previews
downloads/     zips, sample deck and template decks
.nojekyll      tells GitHub Pages to serve the files as they are
```

## Updating

Replace the changed files and push. GitHub Pages redeploys within a minute or two. When the spec, templates or decks change, rebuild the zips in `downloads/` too.

## Credits

- Icons: [Lucide](https://lucide.dev) (ISC License)
- Fonts: Bricolage Grotesque, Hanken Grotesk and IBM Plex Mono via Google Fonts (SIL Open Font License)
- Libraries: [PptxGenJS](https://github.com/gitbrent/PptxGenJS) (MIT), [JSZip](https://stuk.github.io/jszip/) (MIT)

Owner: Rajesh · v0.1
