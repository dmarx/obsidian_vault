---
tags:
  - OC
  - sod/green
  - OC/strict
created: 2024-03-26
---
see also:
- [[Catalysts]]
- [[_Synthesis - Catalyst Kinetics And Social Behavior]]
- [[Nucleation in Social Dynamics]]
- [[Nucleation Theory]]
- [[Community Nucleation]]
- [[Activation Energy]]

consider some information state from which we are starting

a hypothesis represents a change in the information state, energy put in or out

the resolution of that hypothesis is a new information configuration relative to this change

the optimal new configuration may be inaccessible from our current state due to insufficient [[Activation Energy]] (i.e. we don't have adequate information or representation of the problem to reason about the hypothesis in a single step). 

one way to "get around" barriers of this kind is to catalyze multi-step reaction pathways, where the activation energy of each step is low and the configuration after each step is stable.

stability of a configuration in this context is given by "soundness" of reasoning. if a reasoning jump is consistent with the existing information state, it requires basically no energy to adopt.

the "adoption energy" here is the reconfiguration of the information state.

imagine the information state is an ontology of everything the model "knows", represented as a connected (discrete) graph. if information can be added to this graph without causing significant reconfiguration of the graph layout, it requires low energy to adopt. "unsound" reasoning results in significant reorganization of the information state, because either a) the information state was in a suboptimal configuration which we are now remedying by adding this new information, or b) the new information was wrong and introducing it is increasing the "tension" of our knowledge representation due to its inconsistency 

therefore, rather than dropping gigantic changes into the information space, it is preferable to make smaller, incremental changes that guide us smoothly to the desired new information state making lower energy localized changes rather than inducing higher energy global changes in the [[Knowledge Graph]] (really the [[Latent Semantic Manifold]]).

prompting for [[Chain of Thought]] acts as a "[[Catalysts|Catalyst]]" in this process, specifically encouraging the model to search for multi-step reasoning paths that are consistent with their information step rather than trying to reason about a potentially high energy (relative to the "novelty" of the proposition relative to the current information state) hypothesis 

"novelty" here naturally maps to [[Perplexity]], which models [[Surprise]]. 

Motivating idea from the [[Catalysts]] note:
> **Altering Reaction Mechanisms**: Catalysts can change the steps that occur in a reaction mechanism. By offering a pathway with different intermediate steps, they can avoid high-energy intermediates present in the uncatalyzed pathway, effectively lowering the overall energy barrier to reaction.

Maybe the geodesic in information space without CoT between the prompt and the response has to go through a high energy region, and CoT provides an alternate pathway with much lower energy intermediates.

I guess the "intermediates" here are the autoregressively generated tokens, and the energy is just their likelihood/perplexity. The beginning of the desired response might have a high perplexity relative to the prompt context, but CoT steps have low perplexity, giving us a pathway to the desired outcome that gets around what would otherwise be a barrier to sampling the desired output.

[[Multi-step reasoning]] and [[autoregressive sampling]] as [[Reaction Networks]]

