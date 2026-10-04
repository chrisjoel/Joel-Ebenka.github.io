# Joel Ebenka | DevOps and Cloud Engineer Portfolio
# Joel-Ebenka.github.io

Personal portfolio site, live at [https://Joel-Ebenka.github.io](https://Joel-Ebenka.github.io).

It presents my experience, projects, tool stack, certifications, and contact details. It is a static site: it is built once into plain HTML, CSS, and JavaScript and hosted for free on GitHub Pages, and every push to `master` redeploys it automatically.

---

## What is on the Site

| Section | What it shows |
| :--- | :--- |
| **Home** | Name, animated role line, short pitch, terminal-style summary, CV download |
| **About** | Short bio and an interactive tools panel: filter the tool logos by Cloud, IaC, CI/CD, Containers, Monitoring, or Code |
| **Experience** | Roles, dates, and measurable results, laid out as a timeline |
| **Projects** | Filterable cards (Terraform, AWS, Kubernetes, CI/CD) with stack logos and a link to each GitHub repository |
| **Certifications and badges** | Clickable cards; each opens a popup with the issuer, issue date, credential ID, skills, and a verification link |
| **Contact** | Icon buttons for GitHub, email, and LinkedIn |

The site follows the visitor's light or dark system theme, works on phones, has visible keyboard focus, and respects the "reduce motion" setting.

---

## Tech Stack

* **Next.js (App Router)** with a static export, **React**, and **TypeScript**
* **Plain CSS** in `app/globals.css`, with no UI framework
* **GitHub Actions** to build and deploy
* **GitHub Pages** for hosting
* *Optional:* **Docker** and **nginx** for local testing

---

## Project Structure

```text
.
├── app/
│   ├── data.ts                  # All site content: edit this to update the site
│   ├── page.tsx                 # Page layout and sections
│   ├── layout.tsx               # HTML shell, metadata and fonts
│   ├── globals.css              # All styling
│   └── components/
│       ├── Typing.tsx           # Animated role line
│       ├── AboutStack.tsx       # Bio plus filterable tools
│       ├── Projects.tsx         # Filterable project cards
│       └── Certifications.tsx   # Certification cards and popup
├── public/
│   ├── logos/                   # Tool and issuer logos (SVG)
│   ├── badges/                  # Certification badge images (PNG)
│   └── Joel-Ebenka-CV.pdf       # Downloadable CV
├── .github/workflows/deploy.yml # Build and deploy to GitHub Pages
├── docker-test/                 # Optional local Docker setup
├── next.config.ts               # Static export settings
└── package.jsonl Docker setup
├── next.config.ts               # Static export settings
└── package.json
