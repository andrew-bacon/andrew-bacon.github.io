<head>
<script type="text/javascript" charset="utf-8" 
src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML,
https://vincenttam.github.io/javascripts/MathJaxLocal.js"></script>
</head>

# Errata for *A Philosophical Introduction to Higher-Order Logics*

## $$\beta$$, $$\eta$$ and $\beta\eta$-equivalence


Rohan Sud and Daniel Hoek notified me of an error in the definitions leading up to the notion of $\beta$-equivalence. 

In my Definition 3.7 of "free for x" on page 70 I intended clause 3 to have the additional qualificatino that $x\ne y$. I.e. clause 3 should read:

	- $N$ is free for $x$ in $\lambda y.P$ if $x\ne y$, $y\notin FV(N)$ and $N$ is free for $x$ in $P$.

Without this clause, it follows that a constant, $a$ is free for $x$ in $\lambda x.(\lambda x.Fx)$, and we would obtain the erroneous result that $(\lambda x.(\lambda x.Fx))a$ is $\beta$-equivalent to $\lambda x.Fa$. Many thanks to Rohan Sud for spotting this. Sud and Hoek also note that instead of the notion of "naive substitution" in definition 3.4 (p.65) one could have a definition that prevents substitution of a term for $x$ in contexts where $x$ is bound. Thus, to definition 3.4:
    - Add “and x is distinct from M” to clause 4.
    - Add clause 5: λx.P[N/M]=λx.P when x=M.


