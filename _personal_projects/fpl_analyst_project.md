---
title: "FPL Manager Assistant"
subtitle: "A Snowflake-native ontology platform Snowflake from a warehouse into a platform capable of using decision intelligence to support FPL managers in selecting their FPL teams, backed by data."
slug: fpl-analyst-project
model_name: "fpl_analyst"
summary: "A Snowflake Cortex Analyst solution leveraging ontologies to deliver decision intelligence."
order: 2
thumbnail: /assets/images/projects/fpl/fpl_analyst_thumbnail.png
stack: ["Snowflake", "Cortex", "Ontology", "Decision Intelligence"]
demo_url: ""
code_url: "https://github.com/SYellops01/fpl_analyst"
---
<img width="1068" height="561" alt="image" src="https://github.com/user-attachments/assets/00a9328f-bcf0-4330-b8c4-e47b01241341" />

## The Problem

Winning your FPL mini-league isn’t just about picking good players, but about consistently making better decisions than your competitors. With increasingly complex scoring rules, form metrics, and fixture difficulty, it’s hard to quickly identify which players offer the best value within budget.

The FPL Analyst solves this by providing a natural language interface powered by Snowflake, allowing managers to directly query player performance, fixtures, and squad optimisation in real time.

## The Build

I designed and built a five layer architecture that transforms Snowflake from a warehouse into a decision intelligence platform
<img width="1099" height="627" alt="image" src="https://github.com/user-attachments/assets/d6c1b0e0-0f5d-4de5-8294-06935b848e4e" />


- **Layer 5 - Cortex Agent:** Orchestrates semantic models and graph-based reasoning to interpret and answer user queries
- **Layer 4 - Semantic Models:** Knowledge graph and metadata layer enabling contextual understanding of players, teams, and relationships
- **Layer 3 - Generated Views:** Auto-generated ontology-driven views to standardise and simplify querying
- **Layer 2 - Ontology Metadata:** Defines entities, relationships, and properties across the FPL domain
- **Layer 1 - Physical Storage:** Graph structure using KG_NODE (entities) and KG_EDGE (relationships)

## Impact

- Enables natural language querying of both metadata (what data exists) and performance data (how players are performing)
- Reduces the effort required to analyse form, fixtures, and value—turning complex analysis into simple questions
- Provides a flexible, reusable Cortex Agent that can be extended to other analytical domains beyond FPL


***Q: "Which 3 teams have the easiest fixtures in gameweeks 10-14? Give me three recommendations for players to buy from each of these and their positions - I have a budget of 7.5m. When making this suggestion, consider the performance of these players in the previous 3 weeks"***
<img width="1800" height="466" alt="image" src="https://github.com/user-attachments/assets/d24d3d12-59c1-4873-b9bf-cfc1fe36d636" />

***Q: "In gameweeks 30-34, which defenders most frequently hit 10 DEFCONs?"***
<img width="1793" height="345" alt="image" src="https://github.com/user-attachments/assets/330e6090-066e-47c1-bcfb-4b16ff3132a4" />

***Q: "What performance attributes are available in the FPL data to compare?"***
<img width="1379" height="475" alt="image" src="https://github.com/user-attachments/assets/f9df1e32-e83a-44fa-b6f5-100006c8439b" />

