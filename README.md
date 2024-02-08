[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/wM4-KOzy)
# Little-o

In addition to the big-O, big-$\Omega$, and big-$\Theta$ notation that
we covered at the beginning of this class, a few other notations are sometimes
used in asymptotic analysis.  For example, "little-$o$" notation.

Prove (i.e.\ give a formal mathematical proof) that $f(n)\in o(g(n))$ implies
that $f(n)\in O(g(n))$.

Hint: The proof will be *very* short and *very* easy. You can start by
identifying the differences between the definitions of O and o.

I have started with the formal definition of $o$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$

To format the proof correctly for GitHub, you need to use Markdown syntax. Here's the proof formatted for GitHub:

```markdown
# Proof that $f(n) \in o(g(n))$ implies $f(n) \in O(g(n))$

To prove that $f(n) \in o(g(n))$ implies that $f(n) \in O(g(n))$, we need to show that for any function $f(n)$ and $g(n)$, if $f(n) \in o(g(n))$, then $f(n)$ is also in $O(g(n))$.

The formal definition of $f(n) \in o(g(n))$ states that for any positive constant $c > 0$, there exists a threshold $n_0$ such that for all $n \geq n_0$, $f(n) < cg(n)$.

Now, let's recall the definition of $O(g(n))$. A function $f(n)$ is in $O(g(n))$ if there exist positive constants $c'$ and $n_0'$ such that for all $n \geq n_0'$, $f(n) \leq c'g(n)$.

From the definition of $o(g(n))$, we observe that it is a stricter condition than $O(g(n))$ since it requires $f(n)$ to be strictly less than $cg(n)$ for all sufficiently large $n$.

Given that $f(n) \in o(g(n))$, we can choose $c' = c$ and $n_0' = n_0$ to fulfill the condition of $O(g(n))$.

Therefore, $f(n) \in o(g(n))$ implies that $f(n) \in O(g(n))$.
```

This Markdown code will render correctly on GitHub, presenting the proof with proper formatting.
