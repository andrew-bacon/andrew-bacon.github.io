<head>
<script type="text/javascript" charset="utf-8" 
src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML,
https://vincenttam.github.io/javascripts/MathJaxLocal.js"></script>
</head>

# Inductive Structures

## The natural numbers.

There are two rules for building numbers.

1.  $0$ is a number.

2.  If $n$ is a number, so in $sn$.

We can represent these two rules as follows:
$\frac{\qquad}{0}\qquad \frac{\qquad n \qquad}{sn}$
This notation is
read as follows: if you can build everything above the line, then you
can build the thing under the line. When nothig appears above the line,
this means you can always build the thing underneath the line.


**Exercise 1.1** (Tuesday 17th Jan). *Which of the following are natural
numbers that can be built with our rules? For the ones that are, show
that they are using the two rules, 1 and 2, or as a derivation using
horizontal lines.*

1.  *$0s$*

2.  *$0$*

3.  *$sn$*

4.  *$sss0$*

5.  *$s0s$*
:::


**Exercise 1.2** (Tuesday 17th Jan). *Try to think up some rules that
will generate *expressions* for natural numbers in Arabic notation. Show
how to generate $148$ using your rules.*
:::

## Sentences of Propositional Logic

We write propositional letters with the following letters:
$P,Q, R, S, P_1, P_2,P_2, ...$. We use $Let$ to stand for the set of
propositional letters.

The rules for making sentences.
$$\frac{\qquad}{P_i} \qquad \frac{A \qquad B}{(A\wedge B)} \qquad \frac{\qquad A \qquad}{\neg A} \qquad \frac{A \qquad B}{(A\vee B)} \qquad \frac{A \qquad B}{(A\to B)}$$


**Exercise 1.3** (Tuesday 17th Jan). *Which of the following are
sentences of propositional logic? If it is a sentence give a derivation
of it.*

1.  *$P\vee Q$*

2.  *$((\neg P\to Q)\vee R)$*

3.  *$(P\vee R)\wedge Q)$*

4.  *$(\neg P)$*
:::

## Trees

Binary branching trees are built by two rules.

1.  The simple tree $\circ$ is a tree.

2.  If $t_1$ and $t_2$ are trees, then so is $(t_1 \bullet t_2)$

In class we also gave these trees a pictorial representation.


**Exercise 1.4**. *Build four different trees using these rules. You may
represent them pictorially, as we did in class.*
:::


**Exercise 1.5**. *Come up with a new set of rules from which you can
build trees that can branch two or three times at each node.*
:::

## Sequences (strings, lists)


**Exercise 1.6**. *Give examples of elements of the following sets. For
sequences, use the above notation (i.e. $(1,4)$ for the sequence *one
and then four*, etc.).*

1.  *$\mathbb{N}$*

2.  *$\mathbb{N}^*$*

3.  *$\{$Alice, Bob, Carol$\}^*$*

4.  *$(\mathbb{N}^*)^*$*

5.  *$(\emptyset^*)^*$*
:::

There are two rules for constructing sequences of numbers:

1.  $\epsilon$ is a sequence.

2.  If $n$ is a number and $s$ is a sequence, then $n:s$ is a sequence.

we may represent these rules as follows:
$$\frac{\qquad}{\epsilon} \qquad \frac{\qquad s \qquad}{(n:s)} \mbox{when } n \in \mathbb{N}$$


**Exercise 1.7**. *Which of the following can be built from the rules?
For those that can, give the derivations of their constructions:*

1.  *$\epsilon$*

2.  *$(\epsilon :\epsilon)$*

3.  *$(5:\epsilon)$*

4.  *$(\epsilon:5)$*

5.  *$(1:(2:3))$*

6.  *$(1:(2:\epsilon))$*

7.  *$((1:2):\epsilon)$*
:::


**Exercise 1.8**. *Translate the following into the simple
representation of sequences, (where e.g. *four and then seven and then
two* is $(4,7,2)$.)*

-   *$(2:\epsilon)$*

-   *$(2:(3:\epsilon))$*

*translate the following sequences in the simple notation into the $:$
notation.*

1.  *$(4,7,2)$*

2.  *$(1)$*
:::

# Definition by Recursion

## Definition by recursion on $\mathbb{N}$

When defining $f$ by recursion you will in general need to fill out two
equations:

-   $f(0) = \ldots$

-   $f(sn)= \ldots f(n) \ldots$


**Exercise 2.1** (Tuesday January 31st). *Define the following functions
by recursion. You may appeal to any functions you have defined in
previous questions. (NOTE: if you sign up for this exercise you will
only present the last answer, as we did the other two in class.)*

1.  *$add2:\mathbb{N} \to \mathbb{N}$, the operation that adds 2 to a
    number $n$.*

2.  *$double:\mathbb{N}\to \mathbb{N}$, the operation that doubles a
    number: $double(n)=2n$.*

3.  *$power2:\mathbb{N}\to \mathbb{N}$, the operation that doubles 1 $n$
    times (i.e. $power2(n)=2^n$).*

*HINT: Remember that you can use $s$ and $0$, as well as any definitions
you've made in previous questions.*
:::


**Exercise 2.2** (Tuesday January 31st). *Given your above definitions,
simplify $add2(ss0)$, $double(ss0)$ and $power2(ss0)$. (An expression is
fully simplified when it is a natural number, i.e. a sequence of $s$s
followed by a $0$. In the last case, you may need to appeal to your
equations for $double$ as well as $power2$.)*
:::

## Definition by recursion on sentences

Example: if you want to define the length of a sentence it is sufficient
to define the length of a propositional letter, and the length of
$\neg A$, $(A\wedge B)$ and $(A\vee B)$ in terms of the lengths of $A$
and $B$. Why? Because every sentence is built from these rules, and thus
the length of an arbitrary sentence things.

More generally, a definition of an operation $f$ must specify two
things:

-   $f(P) = \ldots$

-   $f(\neg A) = \ldots f(A) \dots$

-   $f((A \wedge B)) = \ldots f(A)\ldots f(B) \ldots$

-   $f((A \vee B)) = \ldots f(A)\ldots f(B) \ldots$

-   $f((A \to B)) = \ldots f(A)\ldots f(B) \ldots$

when defining a function by recursion on strings you should always have
two equations like this.

We can also consider more restricted languages in which one can only
build certain. For instance we will write $\mathcal{L}(\neg,\wedge)$ for
the inductive structure that consists of only the rule for introducing
propositional letters, and $\neg$ and $\wedge$. The rules for defining
operations by recursion on these restricted languages are given by the
first three rules about. In order to get practice working with languages
it is often convenient to work in a restricted language because there
are fewer clauses to write down.


**Exercise 2.3** (Tuesday January 31st). *Define a function
$length:\mathcal{L}(\neg,\wedge)\to \mathbb{N}$ that maps a sentence to
the length of the sentence.*
:::

## Definition by recursion on $A^*$

Example: if you want to define the length of a sequence it is sufficient
to define the length of the empty sequence, $\epsilon$, and the length
of $(n:s)$ in terms of the length of $s$. Why? Because every string is
built from these two rules, and thus the length of these two things.

More generally, a definition of an operation $f$ must specify two
things:

-   $f(\epsilon) = \ldots$

-   $f((n:t)) = \ldots f(t)\ldots$

when defining a function by recursion on strings you should always have
two equations like this.


**Exercise 2.4** (Tuesday January 31st). *Define the following functions
by recursion on sequences.*

1.  *$length:\mathbb{N}^*\to \mathbb{N}$ that maps a sequence to the
    length of the sequence.*

2.  *Define (by recursion) the operation
    $post(3):\mathbb{N}^*\to \mathbb{N}^*$ that takes a sequence $s$ of
    natural numbers and puts $3$ at the end.*

3.  *$s^*:\mathbb{N}^*\to \mathbb{N}^*$ that takes a sequence of numbers
    and returns the sequence you get by adding 1 to each element of the
    sequence.*
:::

## Defining binary functions by recursion


**Exercise 2.5**. *Define the following unary and binary functions by
recursion. You may appeal to any functions you have defined in previous
questions*

1.  *For a fixed $m$, define using recursion
    $addm:\mathbb{N} \to \mathbb{N}$ of adding $m$ . Then define the
    binary operation of addition
    $add:\mathbb{N}\times \mathbb{N}\to \mathbb{N}$*

2.  *For a fixed $m$, define using recursion
    $multm:\mathbb{N}\to \mathbb{N}$ of multiplication by $m$ (i.e.
    $multm(n) = mn$). Now define the binary operation
    $mult:\mathbb{N}\times\mathbb{N}\to \mathbb{N}$ of multiplication.*

3.  *For a fixed $m$, define using recursion
    $powerm(n): \mathbb{N}\to \mathbb{N}$ where $powerm(n)=m^n$. Define
    $power:\mathbb{N}\times \mathbb{N}\to \mathbb{N}$.*

4.  *Define by recursion a function $fact:\mathbb{N}\to \mathbb{N}$
    where $fact$ is the factorial function, i.e. $fact(0)=1$ and
    $fact(n) = 1\times 2\times ...\times n$.*
:::


**Exercise 2.6**. *Define the following unary functions by recursion.
You may appeal to any functions you have defined in previous questions*

1.  *$ladd:\mathbb{N}^*\to \mathbb{N}$ that takes a sequence of numbers
    and adds them together.*

2.  *$lmust:\mathbb{N}^*\to \mathbb{N}$ that takes a sequence of numbers
    and multiplies them together.*
:::

Definition by recursion on trees is similar. To define an operation
$f:T\to A$ on the set of trees $T$, you must say what $f$ does to each
leaf (the simple tree $\circ$), and you must say what it does to
$(t_1 \bullet t_2)$ in terms of what it does to $t_1$ and $t_2$.


**Exercise 2.7**. *Define the following operations on trees.*

1.  *$leaf:T\to \mathbb{N}$ mapping a tree to the number of leaves.*

2.  *$node:T\to \mathbb{N}$ mapping a tree to the total number of nodes
    (both $\circ$ and $\bullet$)*

3.  *$depth::T\to \mathbb{N}$ mapping a tree to the longest path you can
    take from its top node. You may assume the you have defined the
    maximum operation $max:\mathbb{N}\times \mathbb{N}\to \mathbb{N}$.*
:::

## Defining properties and relations by recursion

To define a property $F$ on natural numbers you must do two things:

1.  Say whether $0$ has the property.

2.  Say whether $sn$ has the property, in terms of whether $n$ has the
    property.


**Exercise 2.8**. *Define the following properties:*

1.  *Being an odd number.*

2.  *being greater than or equal to 7.*

3.  *Define the binary relation $\geq$, where $n\geq k$ means '$n$ is
    greater or equal to $k$'. (Recall how we defined binary functions:
    you will fix $k$ and do a recursive definition of the unary property
    $\geq k$.)*
:::

# Proof by Induction

## Proof by induction on the natural numbers

When attempting a proof by induction the first thing to do is figure out
what property you are attempting to show all numbers possess.

Definition of add: $add(k,0)=k$, $add(k,sn)=s\, add(k,n)$


**Exercise 3.1** (Tuesday 7th February: when you sign up sign up for
part a), b) or c)).

1.  *Show by induction that $add(0,m)=m$. (Note that $add(m,0)=m$ is
    true by the definition of add, but this claim needs to be shown by
    induction.)*

2.  *Show, by holding $m$ fixed and doing an induction on $n$, that
    $add(sm,n) = s(add(m,n))$ (note that $add(m,sn)=s(add(m,n)$ falls
    directly out of the inductive definition of $add$, whereas the claim
    in this question has to be proved manually).*

3.  *Show, by holding $m$ fixed and doing an induction on $n$, that
    addition is commutative: for all $n$, $add(m,n) = add(n,m)$. (You
    should may appeal to what has already been proved in the previous
    question.)*
:::

Recall the definition of $mult$: $mult(k, 0)=0$,
$mult(k,sn)=add(mult(k,n),k)$


**Exercise 3.2** (Tuesday 7th February: when you sign up sign up for
part a), b) or c)).

1.  *Show by induction that $mult(0,n)=0$.*

2.  *Show that $mult(sm,n) = add(mult(m,n), n)$ (fix $m$ and do
    induction on $n$)*

3.  *Show that $mult(m,n) = mult(n,m)$ (fix $m$, and do induction on
    $n$. Use the previous two exercises.)*
:::


**Exercise 3.3** (Practice Exercises). *Show the following are true for
any $n$ and $m$ (using induction)*

1.  *Every number is either 0 or a successor (is $sn$ for some $n$)*

2.  *$sn = n+1$*

3.  *$0+n = n$*

4.  *$sn + m = n+sm$*

5.  *$m+n = n+m$ (fix $m$ and do induction on $n$. Use the previous two
    exercises.)*

6.  *$(k+m)+n = k+(m+n)$ (fix $k$ and $m$ and do induction on $n$.*

7.  *$0.n = 0$*

8.  *$sn.m = n.m + m$ (fix $n$ and do induction on $m$)*

9.  *$m.n = n.m$ (fix $m$, and do induction on $n$. Use the previous two
    exercises.)*

10. *$d(n+m) = dn + dm$*

11. *$n+n$ is even. (Recall the recursive definition of even: 0 is even.
    $sn$ is even if and only if $n$ is not even.)*

12. *If $n$ is even, then for some $m$, $n=m+m$.*

13. *$n\leq n+2$. (Recall the recursive definition of $\leq$: $m\leq 0$
    iff $m=0$. $m\leq sn$ iff $m\leq n$ or $m = sn$.)*

14. *$m = n$ or $sm \leq n$ or $n\leq m$.*

15. *If $n\leq m$ and $m\leq k$ then $n\leq k$.*
:::

## Induction on sequences

Recall the recursive definition of $\oplus$:

-   $\epsilon \oplus t = t$

-   $(a:s)\oplus t = a:(s\oplus t)$

and the recursive definition of on $rev$:

-   $rev(\epsilon)=\epsilon$

-   $rev(a:t) = rev(t)\oplus (a:\epsilon)$


**Exercise 3.4** (Thursday February 9). *Show the following by induction
on sequences*

1.  *$t\oplus \epsilon = t$*

2.  *$(t\oplus s)\oplus u = t\oplus (s\oplus u)$ (fix $s$ and $u$ and do
    induction on $t$)*

3.  *$rev(t\oplus s)=rev(s)\oplus rev(t)$*

4.  *$rev(rev(t)) = t$ (you will need to use previous questions.)*
:::

# Propositional Logic

## The Propositional Calculus (Propositional Logic)


**Exercise 4.1** (Thursday 16th of Feb). *A sentence is balanced if it
has the same number of $($ symbols as $)$ symbols.*

1.  *Define two functions by recursion, $leftcount$ and $rightcount$,
    that map a sentence to the number of left parentheses and right
    parentheses respectively.*

2.  *Prove by induction that every sentence is balanced.*
:::


**Exercise 4.2** (Thursday 16th Feb). *Suppose that $v_0$ is a truth
assignment: a function that maps each sentence letter to a $0$ or a $1$.
Define by recursion a function
$v:\mathcal{L}(\neg,\vee,\wedge,\to)\to \{0,1\}$ that assigns to every
sentence it's truth value, assuming that the propositional letters have
truth values given by $v_0$.*
:::

If $v_0$ is a truth assignment, we call $v$ the corresponding valuation.


**Exercise 4.3** (Thursday 16th). *Suppose that $v_0$ is a truth
assignment, and $v$ is a corresponding valuation. Prove the following by
induction*

1.  *For every sentence $A$, $v(A)=1$ or $v(A)=0$. (You should prove
    this by induction).*

2.  *For every sentence $A$, $v(A\vee \neg A)=1$ (you do not need to use
    induction, you can use the previous question.*

3.  *For every sentence $A$, $v(A\wedge \neg A)=0$ (you do not need to
    use induction, you can use question 1).*
:::

## Truth tables

The symbols $\wedge, \vee,\neg, \to$ are called *connectives*. The main
connective of a sentence is the connective that is introduced in the
final step, when it is constructed explicitly from the rules for
building sentences.


**Exercise 4.4** (Do this exercise for practice). *Consider the
following sentences:*

-   *$((P\wedge Q)\vee \neg R)$*

-   *$\neg P$*

-   *$((P\vee Q)\to \neg R)$*

-   *$\neg (P\vee Q)$*

-   *$((P\wedge Q)\wedge R)$*

-   *$(P\wedge (Q\wedge R))$*

1.  *For each of the above sentences, see if you can identify the main
    connective without explicitly constructing the sentence using the
    rules. Write out each sentence and identify your choice by circling
    the connective.*

2.  *Now explicitly construct each of the above sentences using the
    rules, and check your answers to part 1.*
:::


**Exercise 4.5** (Thursday 23rd Feb). *Show that tho following
entailments hold:*

1.  *$A \models (A\vee B)$*

2.  *$(A\wedge B) \models A$*

3.  *$A, B\models (A\wedge B)$*
:::


**Exercise 4.6** (Tuesday 28th Feb). *Show the following:*

1.  *If $A\models B$ and $B\models C$ then $A\models C$.*

2.  *If $A\models (P\wedge \neg P)$ then $A$ is a contradiction.*

3.  *If $A\models B$ then $\neg B\models \neg A$*
:::


**Exercise 4.7** (Tuesday 28th Feb).

1.  *Prove by induction on sentences that if $v$ and $u$ are two
    valuations that agree on the letters in $A$, then $v(A)=u(A)$.*

2.  *Show that if $P\models A$ and $P$ doesn't appear in $A$, then $A$
    is a tautology.*

3.  *Find an example where $P$ does appear in $A$, $P\models A$ but $A$
    is not a tautology.*
:::


**Exercise 4.8** (Revision exercise). *Using the truth table method, or
otherwise, evaluate the following:*

1.  *$\models P$*

2.  *$P\models P$*

3.  *$P \models Q\vee \neg Q$*

4.  *$\models (P\to (Q\to P))$*

5.  *$(P\to (Q\to R)), (P\to Q)\models (P\to R)$*

6.  *$(P\to \neg Q)\models (Q\to \neg P)$*
:::

## Truth-functional completeness

If you know the truth value of $A$ and of $B$ you can always work out
the truth value of $(A\wedge B)$. Similarly, if you know the truth value
of $A$ you can work out the truth value of $\neg A$. By contrast, it's
not possible to determine the truth value of 'John believes that $A$'
even if you know the truth value of $A$. 'and' and 'not' are *truth
functional*, whereas 'John believes that' is not.

So far we have looked at both unary connectives and binary connectives:

-   Unary connectives: $\neg$

-   Binary connectives: $\wedge, \vee, \to$.

The *arity* of a connective is the number of arguments it needs to make
a sentence. Binary operations have an arity of two, unary have arity
one, ternary have arity three, and so on.


**Exercise 4.9** (Tuesday 28th March).

1.  *Make up your own unary truth functional connective. This involves
    making up a symbol for it, and saying what its truth table is. It
    must be different from negation.*

2.  *Make up your own binary truth functional connective, as above. Its
    truth table must be different from $\wedge$, $\vee$ and $\to$.*

3.  *Make up your own ternary connective.*
:::


**Exercise 4.10** (Tuesday 28th March). *For each of the connectives you
made up, try to define it in terms of $\wedge$, $\neg$ and $\vee$.*
:::


**Exercise 4.11** (Thursday 30 (not for presentation -- we did this in
class already)). *Let $v_0$ be the truth assignment that makes every
propositional letter true. Let $v$ be the extension of $v_0$ to
sentences (see section 6).*

1.  *Prove by induction that $v(A)=1$ for every sentence of
    $\mathcal{L}(\wedge)$. (Recall that $\mathcal{L}(\wedge)$ is the
    sublanguage whose only rules are the rule for letters and for
    $\wedge$.)*

2.  *Explain why this means that $\{\wedge\}$ is not truth-functionally
    complete: there are truth functional connectives that cannot be
    defined from $\wedge$ alone.*

3.  *Using a similar strategy, show that $\{\vee,\wedge, \to\}$ is not
    truth functionally complete.*
:::


**Exercise 4.12** (Thursday 30).

1.  *Prove by induction that if $A$ is a sentence of
    $\mathcal{L}(\neg)$, then there exists a letter, $P$, such that for
    any valuations $v$ and $u$, if $v(P)=u(P)$ then $v(A)=u(A)$. (Recall
    that $\mathcal{L}(\neg)$ is the sublanguage whose only rules are the
    rule for letters and for $\neg$.)*

2.  *Explain why this means that $\{\neg\}$ is not truth-functionally
    complete: there are truth functional connectives that cannot be
    defined from $\neg$ alone.*
:::

It turns out that every truth functional connective can be defined from
$\wedge$, $\neg$ and $\vee$. Suppose that $C$ is an $n$-ary truth
functional connective, with the truth table for $C(P_1,...,P_n)$ written
in terms of the letters $P_1...P_n$. There is a general recipe for
defining $C$ from $\neg$, $\wedge$ and $\vee$:

1.  Look at the truth table for $C$ and take note of which lines have a
    $T$.

2.  For each line with a $T$ you will make a conjunction as follows:

    1.  Take note of the truth values of $P_1...P_n$ on that line.

    2.  If $P_i$ is true, include $P_i$ as a conjunct

    3.  if $P_i$ is false, include $\neg P_i$ as a conjunct.

3.  Now you should have a conjunction for each row for $C$ that has a
    $T$. Take the disjunction of these conjunctions, and the result will
    define .


**Exercise 4.13** (April 11). *There exists two binary connectives,
$\uparrow$ and $\downarrow$, that are each truth-functionally complete
all on their own (thus, for instance, every truth functional connective
can be defined from just $\uparrow$. Attempt to find one of these?*
:::


**Exercise 4.14** (April 11). *This exercise is very challenging, but
have a go anyway.*

*$A\leftrightarrow B$ is a connective that is true exactly when $A$ and
$B$ have the same truth value (i.e. it has T in the TT and FF part of
the truth table, and F in the TF and FT parts). Show that
$\{\neg, \leftrightarrow\}$ is not truth functionally complete.*
:::

# Soundness and completeness

## Deductions

The Hilbert system for classical logic has three axioms and one rule.

A1.

:   $A\to (B\to A)$

A2.

:   $(A\to (B\to C))\to ((A\to B)\to (A\to C))$

A3.

:   $(\neg A\to \neg B)\to (B\to A)$

Modus Ponens

:   From $A$ and $A\to B$ infer $B$

A *proof* from a set of assumptions $\Gamma$ consists of a sequence of
sentences subject to the following constraints:

1.  $\epsilon$, the empty sequence, is proof.

2.  If $t$ is a proof, and $A$ is an axiom or an assumption, then
    $(A:t)$ is a proof.

3.  If $t$ is a proof which contains $A$ and $A\to B$ as elements,
    $(B:t)$ is a proof.

A proof *of* a sentence $A$ is a sequence with $A$ as the last element.
The empty sequence is a proof of nothing. We can represent proofs as
inductive structures as follows:
$$\frac{\qquad}{\epsilon}\qquad \frac{t}{(A:t)}\mbox{provided }A\mbox{ is an axiom or }A\in \Gamma\qquad \frac{t}{(B:t)}\mbox{provided }A\to B\mbox{ and }A\mbox{ appear in }t$$

In practice you can write a proof as a numbered sequence of sentences
going down the page. For instance, to show that we can prove $A\to C$
from the assumptions $A\to (B\to C)$ and $A\to B$ we would write a proof
as follows:

1.  $A\to (B\to C)$ Ass.

2.  $(A\to (B\to C))\to ((A\to B) \to  (A\to C))$ by A2.

3.  $(A\to B)\to (A\to C)$ from 1 and 2 by modus ponens.

4.  $A\to B$ by assumption.

5.  $A\to C$ from 4 and 5 by modus ponens.

If you can prove $B$ from the assumptions $A_1...A_n$ you write
$A_1...A_n\vdash B$.


**Exercise 5.1** (Tuesday April 18). *The following sentences are
instances of axioms A1-A3. For each sentence, say which axiom it is an
instance of, and say what $A$, $B$ (and $C$ if applicable) refer to in
that instance.*

1.  *$(\neg \neg P\to \neg \neg Q)\to (\neg Q\to\neg P)$*

2.  *$(P\to \neg P)\to ((\neg P\to P)\to (P\to \neg P))$*

3.  *$(P \to ((Q\to P)\to Q)) \to ((P\to (Q\to P)) \to (P\to Q))$*
:::


**Exercise 5.2** (Tuesday April 18). *Show the following*

1.  *$B \vdash (A\to B)$*

2.  *$(\neg A\to \neg B), B\vdash A$*

3.  *$A\to B, B\to C\vdash A\to C$ (hint: first try to show
    $A\to (B\to C)$ using A1.)*
:::


**Exercise 5.3** (Tuesday April 18). *This is question is slightly more
challenging. Show $\vdash (P\to P)$. You do not need to use A3 in this
proof.*
:::

## Soundness and Completeness


**Exercise 5.4** (Thursday 30th March). *In this exercise you will
create your own axiom system. It must be different than the ones we
discussed in class on Thursday.*

1.  *Come up with your own axiom system. It will have the same rule of
    modus ponens, but you may replace axioms A1-A3 with your own axioms:
    there should be at least one axiom and at most three. They can be
    any sentences you like.*

2.  *Prove something non-trivial in your axiom system.*

3.  *Is your axiom system sound?*

4.  *Do you think your axiom system is complete?*
:::


**Exercise 5.5** (Thursday 30th March). *The axiom systems you provide
for these questions must be different from the ones we discussed in
class.*

1.  *Make up an axiom system that is not sound. Give an example where
    you can prove a sentence from some assumptions (possibly no
    assumptions) where that sentence doesn't follow from those sentences
    (as established by a truth table).*

2.  *Make up an axiom system that is not complete. Give an example of a
    sentence that follows from some assumptions (possibly 0 assumptions)
    which you suspect cannot be derived. (In this question you do not
    need to prove that the sentence cannot be derived -- that is a
    harder task.)*
:::


**Exercise 5.6** (Thursday 30th March). *Assume that the system A1-A3 is
sound.*

1.  *Show that there is no proof from A1-A3 of $P\wedge Q$ from $P$.
    That is $P\not\vdash P\wedge Q$.*

2.  *Show similarly that you cannot prove $P\to Q$ from $P$. I.e.
    $P\not\vdash P\to Q$*
:::


**Exercise 5.7**. *In this question you will prove the soundness of the
axiom system A1-A3.*

1.  *Using the formal inductive definition of a derivation on p13 --- in
    which derivations are treated a certain sorts of sequences --- give
    three examples of a derivation from the assumptions
    $P, (P\to Q), (Q\to R)$ in the axiom system A1-A3. It should have
    the form $(C:(B:(A:\epsilon)))$*

2.  *Let $v$ be valuation and $\{A_1...A_n\}$ a set of assumptions such
    that $v(A_1)=...=v(A_n)=1$. Prove by induction that if $t$ is a
    derivation from the assumptions $\{A_1...A_n\}$ then all of the
    elements of $t$ are true. (You should consult the rules constructing
    derivations on p13).*

3.  *Using the previous question, explain why it follows that if
    $A_1...A_n\vdash B$ then $A_1...A_n\models B$.*
:::

## Proof of the soundness theorem

The following is a sample proof of soundness. It proves that the system
with axioms A1, A2 and A3 is sound. You might be asked to consider a
slightly different system, with different axioms and different rules.
The soundness proof would proceed exactly in the same way: you would
need a lemma showing that every instance of an axiom is a tautology, and
another lemma showing that the rules preserve truth in a valuation (for
example, if the new rule was: you may write $(A\wedge B)$ provided $A$
and $B$ have appeared earlier in the proof, you would need to show that
every valuation that makes $A$ and $B$ true make $(A\wedge B)$ true.)

::: lemma
**Lemma 5.1** (The axioms are tautologies). *Every instance of A1, A2
and A3 is a tautology.*
:::

::: proof
*Proof.* This can be proved, for example, by using the truth table
method. ◻
:::

::: lemma
**Lemma 5.2** (The rules preserve truth). *If $v$ is a valuation,
$v(A)=1$ and $v(A\to B)=1$ then $v(B)=1$. (In other words
$A,A\to B \models B$.)*
:::

::: proof
*Proof.* If $v(A\to B)=1$ then either $v(A)=0$ or $v(B)=1$. But
$v(A)\not= 0$ since $v(A)=1$, so $v(B)=1$. ◻
:::

::: lemma
**Lemma 5.3**. *Let $v$ be a fixed valuation such that
$v(A_1)=...=v(A_n) = 1$. If $t$ is a derivation from the premises
$A_1...A_n$ (i.e. a sequence of sentences given by the rules), then
every sentence in $t$ is true in $v$.*
:::

::: proof
*Proof.* Assume that $v$ is avaluation and that $v(A_1)=...=v(A_n) = 1$.
We will show by induction that any proof using only assumptions from
$A_1...A_n$ will be a sequence of sentences that are all true in $v$.

Base: $\epsilon$ is the empty proof, containing no sentences. It's
trivial that all of the sentences in it are true.

Step: Assume that $t$ is a proof and that all of the sentences in $t$
are true in $v$.

We want to show that every sentence in $(A:t)$ is true in $v$ when $A$
is either a premise or an instance of an axiom. If $A$ is an instance of
an axiom then it is a tautology, by the first lemma, and so true in
every valuation including $v$. If $A$ is a premise then it is one of
$A_1...A_n$, and thus is true in $v$ by assumption.

Step: Assume that $t$ is a proof and that all of the sentences in $t$
are true in $v$.

We want to show that every sentence in $(B:t)$ is true in $v$, where $A$
and $A\to B$ appear in $t$. Since $t$ consistent of sentences that are
true in $v$, $v(A)=1$ and $v(A\to B)=1$. By the second lemma, it follows
that $v(B)=1$, so every sentence in $(B:t)$ is true in $v$. ◻
:::

::: theorem
**Theorem 5.4** (The soundness theorem). *If $A_1...A_n\vdash B$ then
$A_1...A_n\models B$.*
:::

::: proof
*Proof.* Suppose that $A_1...A_n\vdash B$. We want to show that any
valuation that makes $A_1...A_n$ true makes $B$ true.

Let $v$ be an arbitrary valuation such that $v(A_1)=1$ and \... and
$v(A_n)=1$. We want to show that $v(B)=1$. Since $A_1...A_n\vdash B$ we
know that there is a derivation, $t$, using the premises $A_1...A_n$,
such that $B$ is the last sentence in $t$. By the previous lemma, every
sentence appearing in $t$ is true in $v$, so $v(B)=1$.

Since $v$ was arbitrary, every valuation that makes $A_1...A_n$ true
must make $B$ true. Thus $A_1...A_n\models B$. ◻
:::

::: theorem
**Theorem 5.5** (The deduction theorem). *If $A_1,...,A_n,B\vdash C$
then $A_1,...,A_n\vdash (B\to C)$.*
:::

::: proof
*Proof.* Proof sketch: roughly, by prefixng $A\to$ to each line of a
proof of $C$ from $A_1...,A_n,B$ we get a sequence of sentences all of
which can be proven from $A_1...A_n$.

Proof is by induction on proofs. ◻
:::


**Exercise 5.8** (Practice questions). *Establish the following using
the completeness theorem*

1.  *$\vdash (P\to Q) \to ((P\to \neg Q) \to \neg P)$*

2.  *$(P\to (P\to Q))\vdash (P\to Q)$*

*Establish the following using the deduction theorem*

1.  *$\vdash (A\to B) \to ((B\to C)\to (A\to C)$ (recall that you
    previous showed $A\to B, B\to C\vdash A\to C$).*

2.  *$\vdash (A\to ((A\to B) \to ((B\to C) \to C)$.*
:::


**Exercise 5.9** (Practice questions). *Determine whether the following
arguments may be proven in the standard system (with axioms A1-A3). If
can be, give the proof, if not show that there doesn't exist a proof by
appealing to the soundness theorem.*

1.  *$\vdash (P\to (P\to Q))\to (P\to Q)$.*

2.  *$\vdash (P\to Q)\to Q$.*

3.  *$\vdash (P\to Q)\to (P\to (R\to Q))$.*

4.  *$\vdash (P\to (R\to Q)) \to (P\to Q)$.*
:::

(ANSWER for part a:

Ideas: first prove $P\to P)$ and use that to get the result.

1.  $(P\to ((P\to P) \to P) \to (P\to (P\to P)) \to (P\to P)$ A2

2.  $(P\to ((P\to P) \to P)$ A1

3.  $(P\to (P\to P)) \to (P\to P)$ MP, by 1 and 2

4.  $P\to (P\to P)$ A1

5.  $P\to P$ MP, on 3 and 4

6.  $(P\to P) \to ((P\to (P\to Q)) \to (P\to P))$ A1.

7.  $((P\to (P\to Q)) \to (P\to P)$ MP, by 5,6

8.  $((P\to (P\to Q)) \to ((P\to P) \to (P\to Q))) \to (((P\to (P\to Q)) \to (P\to P))  \to ((P\to (P\to Q)) \to (P\to Q)))$
    A2

9.  $(P\to (P\to Q)) \to ((P\to P) \to (P\to Q))$ A2

10. $(((P\to (P\to Q)) \to (P\to P))  \to ((P\to (P\to Q)) \to (P\to Q))$
    MP, by 8 and 9

11. $((P\to (P\to Q)) \to (P\to Q)$ MP by 7, 10.
