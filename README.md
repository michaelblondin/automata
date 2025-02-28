# Automata Theory: An Algorithmic Approach

## Errata

[Add an issue](https://github.com/blondimi/automata/issues) to report a typo, mistake, etc. Please indicate the version of the book you are referring to (and, if it is the online version, please further indicate its compilation date).

The online version of the book maintained by the authors will be updated progressively. The known issues of the printed version published by MIT Press appear here:

* Chap. 3, p. 75, last paragraph: $\mathcal{L}(B) \subseteq \mathcal{L}(B)$ should be $\mathcal{L}(B) \subseteq \mathcal{L}(A)$.
* Chap. 7, p. 170, Example 7.7: There is a missing transition and state. This run:

  $$[1,1,1] \xrightarrow{x=1} [2,1,1] \xrightarrow{y=1} [3,1,1] \xrightarrow{x\gets 0} [4,0,1] \xrightarrow{x = 0 \implies y \gets 1} [5,0,1]$$

  should be:

  $$[1,1,1] \xrightarrow{x=1} [2,1,1] \xrightarrow{y=1} [3,1,1] \xrightarrow{x\gets 0} [4,0,1] \xrightarrow{x = 0 \implies y \gets 1} [1,0,1] \xrightarrow{x\neq 1} [5,0,1]$$

  Accordingly, the accepted word at the end of the example should be

  $$(x=1)(y=1)(x\gets 0)(x= 0 \implies y \gets 1)(x \neq 1)$$

### Acknowledgements

We thank these careful readers for spotting the above mistakes:

* [Pierre Ganty](https://github.com/pierreganty/)
* [Désirée Rentz](https://github.com/desiree-rentz)
* [Matteo Zavatteri](https://github.com/matteozavatteri)
