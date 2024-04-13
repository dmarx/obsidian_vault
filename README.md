---
tags:
  - prune/admin
---
![[2024-03-26_graph.png]]
# DigCyclopedia

- [[The Shape Of Data]]
	- [[Differential Geometry]]
	- [[Information Theory]]
	- [[Information Geometry]]
	- [[Renormalization Group Theory]]
	- [[Symmetry]]
	- [[Phase Transitions]]
	- [[Chaos Theory]]
	- [[Dissipative Structures]]
	- [[Information Flow in Interaction Networks]]
	- [[Collective Behavior]]
	- [[Free Energy]]
	- [[Topology]]
	- [[Measure Theory]]
	- [[Scale Invariance]]
	- [[Critical Exponents]]
	- [[Fisher Information]]
	- [[Statistical Mechanics]]
	- [[Group Theory]]
	- [[Learning Dynamics]]
	- [[Noether's Theorem]]
	- [[Invariants]]
	- [[Geodesics]]
	- [[Parallel Transport]]
	- [[Optimal Transport]]
	- [[Analysis]]
	- [[Concentration of Measure]]
	- [[Self-Organization]]
- [[The Anatomy Of Change]]
	- [[Criticality]]
	- [[Phase Transitions]]
	- [[Renormalization Group Theory]]
	- [[Conservation Laws]]
	- [[Phase Transitions]]
	- [[Chaos Theory]]
	- [[Dissipative Structures]]
	- [[Collective Behavior]]
	- [[Emergence]]
	- [[Gibbs free energy of activation]]
	- [[Scale Invariance]]
	- [[Critical Exponents]]
	- [[Fisher Information]]
	- [[Statistical Mechanics]]
	- [[Learning Dynamics]]
	- [[Noether's Theorem]]
	- [[Analysis]]
	- [[Self-Organization]]
- [[The Illusion Of Control]] alt volumes/titles - 
	- [[Collective Behavior]]
	- [[Emergence]]
	- [[Conservation Laws]]
	- [[Multiplicitous Self]]
	- [[Cultural and Social Capital]]
	- [[Information Flow in Interaction Networks]]
	- [[Gibbs free energy of activation]]
	- [[Scale-Free Networks]]
	- [[Fractal Structures]]
	- [[Statistical Mechanics]]
	- [[Noether's Theorem]]
	- [[Invariants]]
	- [[Geodesics]]
	- [[Free Energy Principle]]
	- [[Generalization]]
	- [[Generative Models]]
	- [[Self-Organization]]
# setup

```
pip install -r .scripts/requirements.txt
```

# Principles

**This is fundamentally for me and from my perspective.**

# Usage


**Tags**
- `root` - Major topical entry points
- `empty-hub` - article with lots of links to non-existent
- `green` - definite include ("The Shape of Data" or whatever)
- `gold` - valuable fringe (to me) topic


... tags could just be its own document.

# TO DO:

* [ ] auto-build readme script
  * [ ] populate tags list
  * [ ] report statistics
  * [ ] benchwarmers-style ToC of `OC`-tagged content
* [ ] compute node clusters (and assign tags)
  * [ ] Label propagation from `root` nodes
* [ ] tagging
  * [x] root
  * [ ] green
* [ ] auto-aliases (this might not be necessary?)
* [ ] .pre-commit-hook to run certain scripts
* [ ] .github/workflow to run certain scripts

also, i need to learn how to use linkable sub headings properly


# Log

## 2024-03-26

Couple of intersecting ideas, can use tags to group them into overlapping volumes

## 2024-03-25

This started when I had a rough idea I was trying to flesh out.

Some recent developments in contrastive learning had me wondering if maybe I could 
concretize my idea by exploring the boundaries of the idea space. I connected the basic dots, 
and then used the LLM to fill in the blanks. I essentially used the LLM as a generative "wikipedia rabbithole",
where the articles I was visiting had the benefit of the context of what had led me to the article and why I was reading it.

After it had expanded a bit, I started tracking it in git, which has the added benefit that I can prune content more aggressively if I want.

Today, I realize how powerful the "tag" function in obsidian is, and plan to a layer a hypergraph over the content.
OLAP. Whatever.

**strategy**: tag some small subset, then visualize a few hops neighborhood graph to connect dots.

AI-assisted brainstorming. What a time to be alive.

**strategy**: use tags to triage work yet to be done.
- `empty-hub`


### Auto STEM Textbook

overlay hypergraph

- user requests a textbook on a given topic
- topic is queried against node set to identify "root" subset of nodes
- graph is expanded out to needed depth, tracking depth from root for each node
- subgraph is persisted as a context for generation
- content is generated/refined based on (conditioned on) level of depth in graph and student provided context (e.g. age, grade level, satisfied pre-requisites, etc.)

### integrate dmarx/bench-warmers

1. pull full contents into graph. shit, just clone the subfolder i guess