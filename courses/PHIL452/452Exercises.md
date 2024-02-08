<head>
<script type="text/javascript" charset="utf-8" 
src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML,
https://vincenttam.github.io/javascripts/MathJaxLocal.js"></script>
</head>


# PHIL 451: Exercises

## Exercises 1

Let $P$ be *God exists*. Consider the argument

1. $\Box (P \to \Box P)$ (Premise)

2. $\Diamond P$ (Premise)

3. $\Diamond \Box P$

4. $P$

Given the possible worlds semantics, does the step from 1 and 2 to 3 seem to be good? What about the step from 3 to 4? 

Draw a possible worlds diagram in which the inference fails: in which there is a world where 1 and 2 are true, and 4 is false.

## Exercise 2

1. Draw all the models over the frame $W=\\{w,v\\}$, $R=\\{(w,v)\\}$ in which every letter is false at every world, except $P$ (which can be true or false at any world). (There should be four.)

2. Prove that $\\{x \mid x\subseteq \\{1\\}\\} = \\{\\{\\}, \\{1\\}\\}$.

3. Suppose that we define $(a,b)$ as $\\{\\{a\\}, \\{a,b\\}\\}$. Prove that this definition satisfies the pairing principle: $(a,b)=(c,d)$ iff $a=c$ and $b=d$.

4. Draw a frame with at least three worlds, and at least three arrows. Represent it as a set $W$ and a relation $R$ using set theoretic notation.

5. Draw the frame with worlds $W=\\{w, u, v\\}$ and accessibility relation $R=\\{(w,u), (u,v), (v,v), (w,w)\\}$. 

## Exercise 3



1. Consider the language $\mathcal{L}(\neg, \wedge)$. Define, by recursion, a function $v:\mathcal{L}(\neg, \wedge) \to \\{0,1\\}$ that 

    (i) "makes the sentence letters true": v(P)=1 for each letter P
	
	(ii) is a valuation valuation for this language: $v(\neg A) = 1-v(A)$ and $v(A\wedge B) = \min (v(A), v(B))$.

2. Prove by induction that the function you defined in question 1 is indeed a valuation.

3. Suppose that $v$ and $u$ are valuations for this language, and that for every letter, $P$, $v(P)=u(P)$. Prove by induction that $v=u$: that is for every sentence $A$, $v(A)=u(A)$.

4. Given a Kripke frame, $(W,R)$, a valuation for the modal language $\mathcal{L}(\neg, \wedge, \Box)$ is a function $v:\mathcal{L}\times W \to \\{0,1\\}$ such that

    (i) $v(A\wedge B, w) = \min(v(A,w),v(B,w))$

	(ii) $v(\neg A, w) = 1-v(A,w)$

	(iii) $v(\Box A, w) = \min_{Rwv} v(A, v)$ (it is 1 iff $v(A,v)=1$ for all $v$ accessible to $w$).

intuitively $v(A,w)$ is the truth value of the sentence $A$ at the possible world $w$. Drawing on the ideas above, show how you would define a valuation on the modal language language in the Kripke frame $(W,R)$ by recursion.

## Exercise 4

1. Prove that $\Gamma \models A$ if and only if $\Gamma \cup \\{\neg A\\}$ is unsatisfiable.

2. Show that any instance of the axiom A2 is valid.

3. Show that $\\{A\to B, A\\}\models B$

4. Prove by induction on proofs that if $\Gamma \vdash A$ then $\Gamma \models A$.

5. Show that $\\{(A\to B), (B\to C)\\}\vdash (A\to C)$, i.e. find a derivation of the formula $(A\to C)$ from the assumptions $(A\to B), (B\to C)$.

## Exercise 5

Suppose that the sentences of $\mathcal{L}(\neg,\to)$ have been enumerated $A_1, A_2, A_3,\ldots$, and suppose that $\Gamma$ is a consistent set of sentences. Let us define a sequence of extensions of $\Gamma$ as follows[^1]:

- $\Sigma_0 = \Gamma$
- $\Sigma_{n+1} = \Sigma_n, A_{n+1}$ if this result is consistent, and = $\Sigma_n$ otherwise.
- $\Sigma = \bigcup_n \Sigma_n$, i.e. $\\{ A \mid A\in \Sigma_n$ for some $n\\}$.

In this question you will show that $\Sigma$ is maximal consistent. In 1 and 2 you'll show that it is consistent. In 4 you'll show that it is maximal-- this means that if $\Sigma, A$ is consistent then $A\in \Sigma$. 

1. Prove by induction on $n$ that $\Sigma_n$ is consistent for every number $n$.

2. Prove that if $\Sigma$ is inconsistent, then $\Sigma_n$ is inconsistent for some $n$. Thus conclude that $\Sigma$ is consistent.

3. Show that if $\Sigma, A$ is consistent then $A\in \Sigma$. (Hint: first show that if $\Sigma, A$ is consistent, then $\Sigma_n, A$ is consistent for any $n$, and use the fact that $A$ appears somewhere in our enumeration.)

4. Using proposition 3.7 in the notes, show how to construct a valuation for any consistent set of sentences $\Gamma$.


[^1] Note that this is slightly simpler than my definition of $\Sigma_n$. Thanks to Arthur for noting that this works too!