# ahmedlotfi.dev · Control Plane Portfolio

**Live:** https://ahmedlotfi.dev

Personal portfolio of **Ahmed Lotfy Mahfouz**, Technical Team Lead (.NET × Production AI), Dubai.
Designed as a live *control plane*: a message bus runs the length of the page, each section is a
service node, and every project runs as a working simulation of the real system behind it.

## Highlights
- 🚌 **Signature layout**: animated message bus with scroll-synced service nodes
- 📡 **9 live simulations**: POS transaction stream, grounded RAG chat with on-prem/hosted
  routing toggle, RFID fuel-lane API trace, CI code-review scanner, and more
- 📄 **Case study** ([`dgx-llm.html`](dgx-llm.html)): four AI workloads in production on
  self-hosted LLMs (Ollama × NVIDIA DGX) behind one .NET abstraction
- 🌗 **Light default / dark toggle**, persisted across visits
- 🖨️ **Print = CV**: a print stylesheet collapses the site into a clean one-page resume
- ⚡ **Zero build step**: plain HTML/CSS/JS, self-hosted variable fonts (188 KB),
  respects `prefers-reduced-motion`, keyboard-accessible

## Stack
Vanilla HTML/CSS/JS · Archivo + IBM Plex (self-hosted, Fontsource) · Cloudflare Pages

## Structure
```
index.html                the site
dgx-llm.html              case study: production AI on-premises
resume.html               resume source (A4 print layout)
Ahmed-lotfy-resume.pdf    resume PDF, rendered from resume.html
certificates/             credential images (original plus web thumbnail)
fonts/                    woff2 (latin subsets)
_headers                  Cloudflare cache rules for fonts
```

## Resume
`resume.html` is the source of the PDF. After editing it, regenerate the PDF with headless Chrome from the repo root:
```sh
"/Applications/Google Chrome.app/Contents/MacOS/Google Chrome" --headless=new --no-pdf-header-footer \
  --print-to-pdf="$PWD/Ahmed-lotfy-resume.pdf" "file://$PWD/resume.html"
```

## Contact
📧 ahmedlotfiali@gmail.com · [LinkedIn](https://www.linkedin.com/in/ahmed-lotfi-ba2206111)
