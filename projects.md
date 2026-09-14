---
title: "Technical Projects"
---

## Featured Project: Pokémon Showdown Meta Dashboard
**Tools:** Python, Polars, Streamlit, Requests, GitHub Releases API

A high-performance analytics platform and web application designed to explore competitive Pokémon Showdown metagame trends, player statistics, and match replays. 

- **Data Engineering Pipeline:** Implements an incremental, stateful ingestion module (`ingest.py`) leveraging O(1) hash-map lookups against JSON manifests and sharding raw data into compressed Apache Parquet batch files.
- **Optimized Compute:** Uses **Polars** `LazyFrame` evaluation (`scan_parquet`) to execute deferred query plans with predicate and projection pushdown, minimizing memory overhead.
- **Serverless Hydration:** Decouples storage from runtime compute by dynamically fetching versioned `.zip` release assets and ledgers on-demand from GitHub.

[View Live Dashboard](https://showdown-projectgit-mbetkr9fi9vhup2xqbggbq.streamlit.app) | [GitHub Repository](https://github.com/jonnboi13/Showdown-project)

---

## Featured Project: Board Game Complexity Analysis
**Tools:** R (tidyverse, ggplot2), Kaggle

In this project, I used R to explore the relationship between board game "weight" (complexity) and user ratings from BoardGameGeek. I performed data wrangling to filter and categorize thousands of games to identify trends in the gaming community.

[Read the Full Analysis](board_games.qmd)

---