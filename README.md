Extension to glossaries for inserting the appropriate indefinite article

Consider the following acronym: `\newacronym{mdp}{MDP}{Markov decision process}`.
The appropriate indefinite article for `\ac{mdp}` depends if the acronym is used (an MDP) or not (a Markov decision process).

`ddbdlossaries.sty` adds options to `\newacronym` and new macros to solve this problem.
As an example, the following code produces the output `A Markov decision process (MDP) is created and an MDP is destroyed.`:

```
\newacronym[acronymarticle=an]{mdp}{MDP}{Markov decision process}
\Aac{mdp} is created and \aac{mdp} is destroyed.
```
