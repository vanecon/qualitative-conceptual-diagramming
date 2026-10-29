# Casting Call

A field guide for assessing, or deliberately designing, how an AI assistant is gendered.

**Use the live tool here: https://gendairesearch.com/casting-call/**

## What it does

Casting Call walks you through four parts of an AI assistant:

- its markers (name, pronouns, voice, imagery)
- its behavior (the job it does and the manner it does it in)
- whether it adapts under pushback
- the assumptions behind those choices

It then shows which pathway the design falls on: reinforcing a gender stereotype or disrupting one. There are two paths: assess an existing AI assistant (Path A), or design your own (Path B).

## How it runs

The tool is a single page (`index.html`). Its Claude features ("Have Claude look it up", the help judging how a marker reads, and the avatar proposal) go through the website's server, which holds the API key and sets the model (Claude Sonnet 4.6) and temperature (0). For security and cost reasons, the server only accepts requests from the website, so the copy in this repository shows the full code but its Claude features work only at the link above. Everything you fill in by hand works anywhere.

"Have Claude look it up" draws on Claude's general knowledge, which extends to roughly August 2025. It does not search the internet, so newer or less well-known assistants may be missing or out of date.

## Data

Information you enter may be saved. What you enter is processed by Anthropic's Claude.

## Limitations

The framework currently addresses gender. It does not yet address race, age, accent, or other important considerations.
