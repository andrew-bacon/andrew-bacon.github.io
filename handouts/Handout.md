<head>
<script type="text/javascript" charset="utf-8" 
src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML,
https://vincenttam.github.io/javascripts/MathJaxLocal.js"></script>
</head>

# Vague Evidence


## Inexact evidence

Consider the following case

> You see a tree in the distance, and this provides you with some evidence about the trees height. You learn, for instance, that it is at least 100cm and that it's less than 1000cm, but the precise height of the tree in cm is unknown to you.

Williamson identifies such cases as involving what he calls inexact knowledge. A parallel phenomenon arises with evidence: we'll call it *inexact evidence*. Imperfect sensory experiences, hazy memories, and so on usually provide us with inexact evidence.

I don't have a precise non-question begging definition, but here are a couple of things it is not: (i) inaccurate evidence (your evidence may well all be true), (ii) unspecific evidence (if someone measured the tree and informed you it was between 300 and 500cm you evidence would be exact but unspecific).

> *Question* (i) What happens to your credences when you obtain inexact evidence? and (ii) What must your theory of evidence be like in order to predict that?

A similar question can be asked about evidential support.

I will take an answer to part (i) as my starting point, without much argument. I take it that upon seeing the tree,  our credences should be symmetrically and smoothly distributed over the possible heights of the tree with a peak that's usually around the actual height of the tree. (Actually one argument we might consider: plausible betting behaviour seems to track this curve.)


## Some important choice points in epistemology

### Externalism or internalism about evidence?

> Could two people be in the same internal state (possessing the same experiences, etc) have different evidence?

Internalists say no. Externalists say yes. Standard example: brains in vats.

### Is evidence propositional? 

> Is evidence always a proposition (or a set of propositions)? Or might it consist of something else, e.g. a visual experience?

Note that all four possible answers to these two questions are consistent, although externalists often take evidence to be propositional. 

Suppose you're an internalist and a propositionalist: what sort of propositions might be be examples of evidence? What sort of thing might a different sort of internalist count as non-propositional evidence?

### Updating: conditioning and Jeffrey conditioning

Suppose evidence is propositional. What should you do when you obtain new evidence? One of the things you might do is change your degrees of belief (the things that control your betting behaviour). Standard theory:

> **Bayesian conditioning**: you should condition on your total evidence. If you start off with credences $P$, and you learn $E$, then your credences should be $P(\cdot \mid E)$.

Perhaps other things happen: the degrees to which various propositions are supported by your evidence changes, also in accordance with Bayesian conditioning. 

Another idea brought up in this context is the idea that you should "Jeffrey condition". It's harder to say what this is a theory of, but let's start with a motivating example. You catch a glimpse of a gem in strange lighting: it's probably red (0.7), but there's a chance that it's purple (0.2) and even a small chance that it's blue (0.1). Now, what's your credence that the gem is very valuable? Conditional on it blue it's very likely to be a sapphire which is very valuable, but conditional on the other two options it's less likely to be valuable: your credence that it is very valuable should be a weighted sum of these three conditional probabilities, weighted by 0.7, 0.2 and 0.1 respectively. So in this particular example

> **Jeffrey conditioning** In this case, your credence in a proposition $A$ after this experience is $0.7\times P(A\mid R) + 0.2\times P(A\mid P) + 0.1\times P(A\mid B)$.

Note: Jeffrey conditioning nowhere mentions evidence. Unlike Bayesian conditioning, it doesn't tell you what to do with your evidence: it just tells you how to redistribute your credences in other propositions when.

> Fact worth knowing: provided you remain certain in things you were previously certain of, any change of credences is obtained by some form of Jeffrey conditioning.

Moral: the claim that you should always update via Jeffrey conditioning is close to vacuous, unless you supplement it with some theory connecting it to evidence.

### Combining Jeffrey conditioning with a theory of evidence

Internalist example: your evidence consists of experiences. Each possible experience you could have comes with the information needed to Jeffrey condition (a partition of logical space and weights). 

Field-Garber exchange: a natural way of doing this (Field 19??) has the unwelcome consequence that repeatedly having the same experience (in this case looking at the ball over and over again) will very quickly raise your credences that the ball is red to near 1.

Other solutions may have the same problem, depending on how they are spelled out. Consider, e.g., the theories Morrison 2016, Munton 2016 in which visual experiences include contents + a confidence relation to that content. 

## Some theories of inexact evidence

### Jeffrey conditioning

We should Jeffrey condition with respect to the partition of tree heights, and weights that reflect the smooth curve we'd expect.

Since Jeffrey conditioning is neutral about what evidence is, there are various ways we could attempt to make this answer compatible with externalism, internalism, propositional evidence, and non-propositional evidence.

Problems? We have discussed some general problems above. Crucially, Jeffrey conditioning is not really a theory of what do to with your evidence, only how to change your credences in other propositions once you've decided to adopt certain credences in the tree heights. It does not predict the curvy view, that was put in by hand.


### Internalism, propositional evidence and conditioning

A natural internalist picture: your total new evidence is a proposition about what experiences I have had, and this proposition makes various hypotheses about the height of the tree more or less likely in a way that conforms to the desired curve.

A standard problem for this sort of view is that it seems to lead to skepticism: we can't come to know anything about the height of the tree if our evidence is only ever about our experiences. For propositions solely about our experiences  are compatible with what we know *a priori* with various skeptical hypotheses. Maybe the correct response to this is that we should think of evidence as much rarer than knowledge.

This also means that the curve isn't the one we were aiming for, since the ends never reach zero on one side, not symmetric.

### Externalism, propositional evidence and conditioning

A natural externalist picture: your total new evidence about the tree is a proposition about the height of the tree. 

Propositions about the height of the tree include the proposition that the tree is exactly $n$cm, for each $n$, and propositions you can get from these using disunction, conjunction and negation. Let us suppose that these are in fact all the propositions about the height of the tree. Then we seem to have a problem:

The only plausible candidates for your evidence are propositions of the form: the tree is been $N$cm and $N+K$cm. These form a square.

Betting behaviour? People with different eyesight may be equally good at discriminating.

### A hybrid view?

You learn the conjunction of a proposition about the height of the tree, and something about your experiences. But this still seems to give the wrong sort of curve: it doesn't have cliffs, but it's still non-smooth at the extremities.


## Interlude: Vagueness

Is vagueness purely linguistic, or is there propositional vagueness? If the latter, what is the role of vagueness in thought.

How should ones credences in *The nth guy is bald* be distributed in a sorites sequence for baldness?

## Vague propositions

A central thesis of *Vagueness and Thought* is the following claim about vagueness

> Vagueness is propositional. When your evidence about a subject matter is inexact, your total evidence is a vague proposition.

Your total evidence is the *conjunction* of all of your evidence. We will assume, for simplicity, that this conjunction is also part of your evidence.


## Conditioning on a vague proposition

Let us consider what would happen to our credences if we were to condition on the proposition *the tree is about 500cm*. Call this proposition $E$.

> **Bayes theorem** $P(A\mid E) = P(E\mid A)\times \frac{P(A)}{P(E)}$

So to figure out how our credences in some precise propositions (about how tall the tree is in cm) conditional on a vague proposition (say, *the tree is about 500cm*) it suffices to consult our judgments about the probability of the vague proposition on the different precise propositions. And these judgments fall out of the general intuition about credences and sorites sequences.

**Note**: The proposition we in fact learn when looking at the tree may depend on our eyesight, the conditions etc: it's very unlikely to be the very same vague proposition as the one expressed by the sentence "The tree is about 500cm". Perhaps it isn't easily expressed by any sentence of English.

## Jeffrey conditioning again

Now we can finally see that our theory of conditioning is actually not inconsistent with Jeffrey's rule, and provides exactly the sort of supplement needed to turn it into a theory for updating on evidence:

> Conditioning on a vague proposition about the tree is equivalent, with respect to the precise propositions, to a Jeffrey conditioning on the partition of maximally specific precise height claims (the tree is *ncm*) 




## A principle of Plenitude for vague propositions

Evidential role: a function mapping each maximally strong consistent precise proposition, $w$, to a number between 1 and 0. 

Example:

> The max con precise propositions are all of the form: the tree is $n$cm. The evidential role of the tree 

Then we can state:

> *The Principle of Plenitude* Every evidential role is realized by some vague proposition: If $f$ is an evidential role, then there exists some vague proposition $q$ such that $P(q\mid w) = f(w)$ for every maximally strong consistent precise proposition.

