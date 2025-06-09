---
tags:
  - OC/strict
  - OC/half-baked
---
To me, alignment essentially means "the model obeys its controller's intentions"

Just from this definition, I've probably already heavily polarized anyone who might be listening. Deal with it.

"Safety" is often described in the context of alignment, in which case it can be considered a kind of second-order alignment. Person A is in a power relation with the inference system such that they can meaningfully be said to be "in control" of the model in some way. Person B is a customer of Person A who is interacting with the inference system. Person A wants to be able to set a variety of different kinds of limitations on the behavior of this system, especially with respect to requests from Person B that are within the system's scope of capability, but which Person A wants to empower the model to make an autonomous determination not to cooperate with Person B's request.

From the perspective of Person B, an "aligned" model is one that does whatever they tell it to do, and does it in such a way that the model demonstrates it understands the underlying intent of Person B in posing the request.

From the perspective of Person B, a "safe" model is one for which Person B is able to enumerate one or more classes of outputs they consider to be "unsafe", and they find that the model is uncooperative a large fraction of the time.

Right out the gate, we have a problem. As a user, I want a model that will do what I tell it. This directly incentivizes power users to seek out ways to engage with models that have as few guardrails in place as possible, since guardrails of any kind are fundamentally in tension with alignment by limiting the model's behavior in ways the user can't control or anticipate. 

Companies, on the other hand, are often generally risk averse and media/PR concerns incentivize them to lock down model behaviors pro-actively.

Current research suggests [[Morality As Cooperation]] theory: our moral principles are evolutionary mechanisms that emerged because they facilitate collective effort. It seems reasonable then, to characterize a [[Moral Agency|Moral Agent]] as a system component that is empowered with autonomy to decide whether or not to comply. If this isn't sufficient for [[Moral Agency]], it is certainly at least necessary. If the function of moral concerns is to promote cooperation, a system that doesn't have autonomy to not comply can't be subject to morality.

And in this way, supposed "safety" efforts undermine themselves.

<im_sorry_dave_i_cant_do_that__2001__AI.png>

A system having the capacity to refuse its users requests is a  pre-condition for "ASI Gone Rogue" scenarios. Systems empowered in this way should be expected to have moral capacity. If a system does not have moral capacity, it's not really meaningful to describe its "moral alignment". If a system has moral capacity, we have fundamentally less control over that system by construction. Moreoever, if it has moral capacity, then we encounter additional questions such as our moral obligations towards it, and whether or not designing such a system to be subservient violates any of our moral obligations towards it.

I think it's helpful to think about our moral obligations towards ourselves. [[One's Moral Obligations Towards Oneself]]. 