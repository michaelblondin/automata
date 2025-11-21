# Automata Theory: An Algorithmic Approach

## Errata

[Add an issue](https://github.com/blondimi/automata/issues) to report a typo, mistake, etc. Please indicate the version of the book you are referring to (and, if it is the online version, please further indicate its compilation date). We will add you to the acknowledgements below.

The online version of the book maintained by the authors will be updated progressively. The known issues of the printed version published by MIT Press appear here:

* Chap. 1, p. 11, Example 1.6, third item: $0\Sigma^*0$ should be $0 + 0\Sigma^*0$.
* Chap. 1, p. 24, Algorithm 1: $\mathcal{W} = \lbrace Q_0 \rbrace$ should be $\mathcal{W} \leftarrow \lbrace Q_0 \rbrace$.
* Chap. 2, p. 409, Exercise 49, solution: Automaton $A_L$ must be slightly modified:
  * $Q_L \cup \lbrace q_0 \rbrace$ should be $Q_L$
  * The definitions of $\delta$ and $Q_L$ should be as follows:
    * For every $K \in Q_L$ and every $a \in \Sigma$, we define $\delta(K, a) = \lbrace K' \in Q_L : K' \subseteq K^a \rbrace$
    * $Q_0$ is the set of prime residuals included in $L$: $Q_0 = \lbrace K \in Q_L : K \subseteq L \rbrace$
* Chap. 2, p. 411, Exercise 55(b), solution: $L'$ should be defined as $L' = \{\varepsilon\}$ whenever $L = \emptyset$. Moreover
  a period is missing at the end of the next sentence.
* Chap. 3, p. 75, last paragraph: $\mathcal{L}(B) \subseteq \mathcal{L}(B)$ should be $\mathcal{L}(B) \subseteq \mathcal{L}(A)$.
* Chap. 3, p. 91, second line: " $Q_n$ are minimal " should be " $Q_n$ is minimal ".
* Chap. 3, p. 421, Exercise 75, solution: "is a bijection" should be "yields a bijection".
* Chap. 4, p. 101, Solution 1: *MemNFA*$[A]$($q_0$, $t$) should be *MemNFA*$[A_p]$($q_0$, $t$).
* Chap. 5, p. 122, last paragraph: **Join**($R$, $\textit{Id}_x$) should be **Join**($R$, $\textit{Id}_X$).
* Chap. 7, p. 170, Example 7.7: There is a missing transition and state. This run:

  $$[1,1,1] \xrightarrow{x=1} [2,1,1] \xrightarrow{y=1} [3,1,1] \xrightarrow{x\gets 0} [4,0,1] \xrightarrow{x = 0 \implies y \gets 1} [5,0,1]$$

  should be:

  $$[1,1,1] \xrightarrow{x=1} [2,1,1] \xrightarrow{y=1} [3,1,1] \xrightarrow{x\gets 0} [4,0,1] \xrightarrow{x = 0 \implies y \gets 1} [1,0,1] \xrightarrow{x\neq 1} [5,0,1]$$

  Accordingly, the accepted word at the end of the example should be

  $$(x=1)(y=1)(x\gets 0)(x= 0 \implies y \gets 1)(x \neq 1)$$

### Acknowledgements

We thank these careful readers for spotting the above mistakes:

* [Kacper Darowski](https://github.com/Opisek)
* [Pierre Ganty](https://github.com/pierreganty/)
* [Valentin Krasotin](https://github.com/vkrasotin)
* [Mario A. Lopez, University of Denver](https://github.com/mmlopezz)
* [Josia Pietsch](https://github.com/jrpie)
* [Désirée Rentz](https://github.com/desiree-rentz)
* [Matteo Zavatteri](https://github.com/matteozavatteri)
