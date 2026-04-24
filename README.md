# almunam.github.io

Personal academic portfolio — Al Muktadir Munam  
M.Sc. Epidemiology & Applied Health Research, Dalhousie University

## Structure

```
index.html      # Main portfolio (single page, React via CDN + Babel)
style.css       # All styles
munam.jpg       # Portrait photo
favicon.svg     # Browser tab icon
```

## GitHub Pages setup

1. Push this repo to `<yourusername>.github.io`
2. Go to **Settings → Pages → Source → Deploy from branch → main / root**
3. Live at `https://<yourusername>.github.io`

## To update content

All content is inline in `index.html` — search for the section function you want to edit:
- `function Hero` — name, subtitle, links
- `function Research` — research interests
- `function Education` — degrees
- `function Experience` — positions
- `function Publications` — papers (update doi, journal, year)
- `function Awards` — awards and scholarships
- `function Writing` — blog/essay entries
- `function Expertise` — methods and tools
- `function Contact` — contact info
- `function Footer` — copyright year

Update Scholar/LinkedIn/ORCID URLs in `Hero` and `Contact` (currently placeholder `#`).

## CV download

Add your CV PDF to the repo root as `CV_AlMuktadirMunam.pdf`.  
The Download CV button will need an `href` update in the `Hero` function:

```jsx
<a className="btn btn-primary" href="CV_AlMuktadirMunam.pdf" download>
  Download CV <span className="arrow">↓</span>
</a>
```

## No build step required

Plain HTML/CSS + React loaded from CDN. No npm, no bundler.
