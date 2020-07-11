# Definitions

SCM
* Graph of M G(M)
* Observation VS Intervention
* (perfect) intervention


Markov property
* (conditional) independence: in terms of prob.
* d-separation (visual graph example)
* Markov equivalence (covered edge reversal)

Tasks:
* Global inference -> MEC
* Local inference -> feature of SCM

* Identifiable?, Total causal effect?, cause & direct cause



# Principles of causal inference

## Assumptions: causal knowledge/assumptions
(example how it can be exploited? example method?; image to visualize assumptions in graph?)
Reichenbach's principle
* Selection bias (unbiased data selection)
- LCD: combination of (in)dependences only works if they cannot be the cause of conditioning on a hidden variable
Faithfulness
* Independence oracle
* causal minimality (follow from faithf.)
* identifiability 
- ASD: add (in)dep. as soft constraints in an ASP solver
Causal sufficiency (absence of Latent Confounders)
- IC: infer edge if there is no set of variables that makes a dependence a conditional independence
Acyclicity
* Topological order (reference)
- SP: restrict the search space of DAGs
Exogeneity
- ICP: exploit invariance to the exogenous variables of the conditional distribution of a variable given it's parents


Focus here on independence, but there are other patterns that can be exploited, such as 
* “Verma constraints” (Shpitser et al.,2014), 
* algebraic constraints in the linear-Gaussian case (van Ommen and Mooij, 2017),
* non-Gaussianity in linear models (Kano and Shimizu, 2003), and 
* non-additivity of noise in nonlinear models (Peters et al., 2014) can also be exploited.


ADD/REWRITE RElATED WORK:
- disadvantages of constraint-based
- other constraints







Backdoor criterion?

% SECTIONS
% Definitions of concepts (including topological ordering)
% Causal principles (Reichenbach, independence (correlation), …)
% Related methods
%   Width: categories
%   Depth: SotA on Kemmeren

% NOTES
% SCMs
% Cycles, latent confounding, selection bias, interventions, constraint VS score-based, faithfulness, causal sufficiency (Markov properties), graph types, evt. independence oracle (Chickering et al., 2004? [according to \citeauthor{claassen2013learning}])

\subsection{Mathematical Definitions}
% TODO: list of priorities in concepts/definitions/propositions


\subsection{Principles of Causal Inference}
% Assumptions: faithfulness, selection bias, confounding
