---
tags:
  - goal
  - user-story
---
1. type in topic/title at top of note
2. article fills out below
3. select interesting content, macro pastes template that uses clipboard content to emit new prompt for continuation
4. turn phrase into a link, clicking into link creates new article *to be immediately and automatically used as a prompt to generate the new article*
---

For research archive:

1. autoURI plugin thing: grab arxiv URL from clipboard.

---

For development of this wiki:
- extract and dedupe nodeset and skeleton graph
- apply templated prompts over node classes to develop content

prompting ideas
- key terms
- core ideas
- implications
- applications
- modern developments
- mathematical formalization
- important relations (query neighborhood, prompt for elaboration on respective relationships)
- RAG over canonical content
	- wikipedia
	- nlab
	- open textbooks

---

auto page numbers
auto distance from root (level sets of topic "depth")
- assign each root a depth and use those as levelset prototypes
- identify other "prototype" nodes and assign them fixed depths as levelset prototypes (as if they were roots)

---

### Exploration Mode

auto-book/auto-wiki: show local graph, and *propose pages in the local graph*. Add links to proposed nodes to pull them into the 1 step neighborhood. This triggers process to propose the new additions to the two step neighborhood: the 1 step neighborhood around the (previously proposed) newly added node

originally via [[Semantic Space Geometry]]