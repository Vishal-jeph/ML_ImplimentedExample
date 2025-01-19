# ML_ImplimentedExample
## Topic 1 - Pre-Pruning and Post-Pruning 

Pre-pruning and post-pruning are techniques used in decision tree algorithms to prevent overfitting and improve generalization:

- Pre-pruning (Early Stopping): This involves halting the tree growth early, before it reaches its maximum size. Constraints like a maximum depth, minimum number of samples per leaf, or a minimum information gain threshold are applied during tree construction to stop splitting nodes. While it reduces overfitting, it risks underfitting by stopping the tree too early.

- Post-pruning (Prune After Full Growth): The tree is fully grown, and then unimportant branches are removed. This involves evaluating nodes and pruning them if their removal doesn't significantly decrease performance (e.g., based on cross-validation or statistical tests). Post-pruning balances complexity and performance better but is computationally more intensive.

