# Meta-Analysis Consultation

An interactive, browser-based toolkit for planning, evaluating, and presenting systematic reviews and meta-analyses using an eight-step PRISMA-informed workflow.

## Live Demo

Once GitHub Pages is enabled, the application will be available at:

<https://hanyassalem.github.io/meta-analysis-consultation/>

## Features

- Eight-step meta-analysis workflow covering:
  1. Research question and eligibility criteria
  2. Comprehensive literature search
  3. Dual screening and risk-of-bias appraisal
  4. Standardized data extraction
  5. Effect measures and statistical model selection
  6. Quantitative synthesis and heterogeneity assessment
  7. Subgroup, sensitivity, and publication-bias analyses
  8. Manuscript presentation and GRADE certainty assessment
- Interactive audit checklist
- Risk-of-bias matrix
- Forest plot sandbox with pooled-effect calculations
- AI Protocol Lab for generating a draft PICO framework and PubMed search strategy
- Export and copy tools for protocol content
- Responsive interface for desktop and mobile browsers

## Running the Application

This is a single static HTML application. No build process or package installation is required.

### Open locally

Clone the repository and open `index.html` in a browser:

```bash
git clone https://github.com/HanyasSalem/meta-analysis-consultation.git
cd meta-analysis-consultation
```

You can then double-click `index.html` or open it from your browser.

### Run with a local server

A local server is recommended for browser features such as clipboard access:

```bash
python3 -m http.server 8000
```

Open <http://localhost:8000> in your browser.

On Windows, use:

```bash
py -m http.server 8000
```

## GitHub Pages Deployment

To publish the application on GitHub Pages:

1. Open the repository's **Settings** page.
2. Select **Pages** in the sidebar.
3. Set the source to **Deploy from a branch**.
4. Select the `main` branch and the `/ (root)` folder.
5. Click **Save**.

The site will be served from the repository's `index.html` file after deployment finishes.

## Technology

The application is implemented in a single `index.html` file and uses browser-loaded dependencies from public CDNs:

- HTML5
- React 18
- React DOM 18
- Babel Standalone
- Tailwind CSS Play CDN

## Gemini API Features

The AI Protocol Lab and AI forest-plot interpretation require a Google Gemini API key.

1. Obtain a key from [Google AI Studio](https://aistudio.google.com/app/apikey).
2. Open the application.
3. Select **Set Free API Key** in the header.
4. Enter and test the key.

The key is entered client-side and is not stored in this repository. Do not commit a private API key to source control. For production use, consider routing AI requests through a secure backend instead of exposing an API key in the browser.

The standard workflow, checklist, risk-of-bias matrix, and forest plot functionality can be viewed without an API key.

## Disclaimer

This tool is intended for educational, planning, and consultation purposes. It does not replace formal statistical review, clinical judgment, methodological guidance, peer review, or the requirements of a target journal or registry. Verify all generated content and statistical decisions before using them in a protocol, manuscript, or clinical decision.

## License

No license has been specified for this repository. Contact the repository owner before redistributing or reusing the code.
