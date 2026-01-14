# Pokemon Search – Coveo Technical Assignment

## Overview
This project indexes pokemondb.net and provides a searchable Pokémon experience using Coveo Atomic.

## Features
- Full Pokémon indexing via sitemap source
- Facets:
  - Pokémon Type (multi-value)
  - Pokémon Generation (numeric)
- Sorting:
  - Name (A–Z), (Z-A)
  - Generation
- Rich results:
  - Pokémon images
  - Type metadata
  - Generation metadata
- Relevance Generative Answering (RGA)

## Technical Decisions
- Used a DEV source for fast iteration
- Used XPath scraping to extract clean metadata
- Numeric facets use half-open ranges
- Local Atomic setup to avoid Search Pages privilege requirements

## Running Locally
```bash
npm install
npm start

## Live Demo
https://marcbourbonnais.github.io/pokemon-search-coveo/