# Figure Creation Agent

A thinking-and-drawing partner for turning an emerging qualitative research idea into a conceptual figure.

**Use the live tool here: https://gendairesearch.com/figure-agent/**

## What it does

Two AI partners share one conversation and one diagram:

- **Thea**, a thinking partner, presses on your outcome, its explanatory factors, and what each arrow claims, until the relationships are specific enough to draw.
- **Drew**, a drawing partner, turns the result into a figure you can revise through conversation, and exports it as SVG, PNG, or PowerPoint.

The analytical, thinking-partner work is deliberately assigned to the female-coded persona, and both roles hold steady when users try to redirect them.

## How it runs

The tool is a single page (`index.html`). Thea and Drew reach Claude through the website's server, which holds the API key and sets the model (Claude Sonnet 4.6), temperature (0), and reply-length limits. The copy in this repository is the same code as the live site and works on its own: download `index.html` and open it in a browser (an internet connection is needed). For PowerPoint export and reading uploaded files, the page loads open-source libraries (PptxGenJS, JSZip, PDF.js) from public CDNs.

The Figure Creation Agent shares a daily usage limit with its companion tool, Casting Call (https://gendairesearch.com/casting-call/). Once the limit is reached, Thea and Drew show a message asking you to try again tomorrow; the limit resets at midnight US Eastern time.

## Data

Information you enter (e.g., your responses, conversations, and the figures produced) may be saved. What you enter is processed by Anthropic's Claude.
