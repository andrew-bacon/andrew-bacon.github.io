




<head>
<script type="text/javascript" charset="utf-8" 
src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML,
https://vincenttam.github.io/javascripts/MathJaxLocal.js"></script>
</head>


# Lecture II notes

## Logical framework

The logical framework I have been suggesting.


There is a theoretical term: pure. Means roughly a logical operation, but I will leave it undetermined what counts at present.

Terminology
	- A definition of A is a pair $Q, \bar B$ such that $Q$ is "pure" and $Q\bar B = A$
	- A definition of $A$ in terms of $\bar B$ is a pure operation $Q$.
	- A is the definiendum.
	- $\bar B$ the definiens. 
	
Examples 


	
	Single = not married to anyone. 
		- definition of *single* in terms of *married to*.
		- $Q= \lambda Rx.\neg\exists y.Rxy$
	
	Bachelor = man who is not married to anyone.
		- definition of *bachelor* in terms of *married to* and *man*. 
		- $Q = \lambda RFx.(\neg \exists y.Rxy \wedge Fx)$

In my terminology a single thing can have multiple definitions. Using Leibniz's law alone we can derive another definition of *bachelor*. 
	
	Bachelor = single man. 
		- Definition of *bachelor* in terms of *single* and *man* ($Q = \lambda FGx.(Fx\wedge Gx)$).

However we can ask whether a thing has a unique definition meeting further requires: e.g. a unique definition in terms of the definiens $\seq B$, or in terms that are "logically prior" to the definiendum, or in terms of the fundemental. 

## Linguistic vs. metaphysical definition in Aristotle
	
Posterior Analytics B.10: A definition is an account given in reply to the 'what is ...?' question. 

	- Distinction:
		+ What does "thunder" signify? ("thunder" means noise in the clouds)
		+ What is thunder? (thunder is noise in the clouds)
	- If I ask why is there thunder you would answer: because there is noise in the clouds. Only the latter kind of definition can be used to finish this explanation. 




## Wh questions: context sensitivity and guise sensitivity.

	A definition tells us *what a thing is*. 
	Is this mysterious
	
	
	- Who is John? 
		+ Looking a year book photo: that guy. 
		+ A colleague. So and so's husband. 
	
	What is Hesperus?
		+ Hesperus.
		+ Phosphorus. 
		+ The brightest body to appear in the night sky at morning.
		+ The brightest body to appear in the night sky at morning.

	Is the constraint a meaningful one when applied to metaphysical definition? It seems to be non-vacuous constraint when applied to 
		
	Suppose that $A= Q\bar B$ and $A=P \bar C$. Can the former, but not the latter, tell us what $A$ is?
		+ Leibniz's law: If $A= Q\bar B$ and $A=P \bar C$, then if $A = Q\bar B$ answers the why question, then so does $A = P\bar C$. 
	
	Answering the why question is opaque: sensitive to modes of presentation. 


## A thing has only one true definition.

	- Lots of necessary equivalences, but only one true definition.

	- Related: might there be lots of true identities? (And thus non-fundamental definitions in my sense). Leibniz's law suggests yes, as we saw in the previous section.

## In a proper definition the definiens are logically prior to the definiendum. 

The idea is found in the Topics and Metaphysics:
	"Such things are prior from whose logoi (other) logoi are composed" (trans. Fererjohn)
	
	+ In our framework, one can ask various uniqueness questions. 
	
		- $A$ has a unique definition: $Q, \seq B$.
		- $A$ has a unique definition in terms of $\seq B$: $Q$.
		- $A$ has a unique definition where the definiens are logically prior to $A$.
		- $A$ has a unique definition that answers "what is $A$?". 
		- $A$ has a unique definition that has explanatory unity: features in explanations of why $A$ is necessarily this or that. 
		- $A$ has a unique definition where the definiens are logically basic. 
	
	+ Counterexamples: 
		- Bachelor above. 
		- Great-grandmother has multiple definitinos in terms of mother, father, parent
			+ mother of a parent of a mother or father.
			+ mother of a mother of a parent or mother of a father of a parent.
			+ etc.
		- Same as above. Mother, parent and father all seem prior. 

## Non redundancy.

Topics VI.3: something is superfluous if, when it is removed, what remains still makes the thing defined clear. 



## All necessities follow and are metaphysically explained/caused by definitions. 

