# Machine Teaching Causal Propositions Across Model Equivalence Classes

**Fletcher Scott, Danula Hettiachchi, Damiano Spina, and Lauren Saling**  
RMIT University

Companion repository for the ADM+S research poster and associated paper on teaching causal judgements through the selection and ordering of observational examples.

> **Update — 21 October 2026:** The current paper contains new results and analyses developed after this poster was prepared. The poster summarises the original teaching comparisons. The paper extends these comparisons with globally optimal teaching benchmarks and separates differences between teaching objectives from greedy search limitations and choices among tied solutions. Please use the current paper for the expanded methods, results, and conclusions.

## The question

If answering a complete set of causal questions and recovering the causal graph share the same endpoint, do the same examples help learners get there?

A learner can answer a particular causal question without identifying the entire graph: it needs to distinguish models that disagree about that answer. Across a battery containing every possible directed-edge question, however, the complete set of true answers distinguishes every candidate graph. We examine whether teaching the graph and teaching its propositions also favour the same observations along the way.

## The benchmark

Teachers select or order genuine observational records from a fixed pool. We compare teaching directed at graph recovery, teaching directed at proposition judgements, and random presentation, while holding the causal world and available observations constant within each comparison.

| Component | Setting |
| --- | --- |
| Causal worlds | 19,935 canonical Boolean structural causal models over three variables and 25 directed acyclic graphs |
| Questions | 24 structural propositions: direct causes, directed paths, two-edge chains, common parents, and common children |
| Evidence | A 32-record pool reproducing each world's observational distribution exactly |
| Learners | Exact Bayes; Soft MDL, which favours simpler explanations; Window 4, which retains the last four records; and Single-Graph, which revises one graph at a time |
| Original selection comparisons | Budgets of 4, 8, and 16 records |
| Original ordering comparisons | Different orders of the same complete 32-record pool |
| Evaluation | Proposition Brier loss, graph-recovery measures, and observational-identification checks |

The poster labels these learners **Ideal Inference (II)**, **Prefers simpler explanations (SE)**, **Remembers Last four (R4)**, and **Revises one graph at a time (RG)**. These correspond to Exact Bayes, Soft MDL, Window 4, and Single-Graph, respectively. The results concern simulated learners.

## Findings shown on the poster

- **The teaching objective matters.** Improving graph recovery and improving proposition judgements can favour different examples, with limited transfer between the two outcomes.
- **The learner matters.** At 16 records, proposition-directed teaching produced lower proposition error than graph-directed teaching for three of the four learners. The simplicity-biased learner showed the reverse pattern under the original greedy procedures.
- **The order matters for some learners.** Ordering affected bounded learners. Cumulative learners gave the same final judgements after receiving the complete pool.
- **The question matters.** Some questions could be resolved without recovering the entire graph. Selected observations could also improve judgements when the full observational distribution left the answer unresolved.

## New results in the current paper

The expanded paper evaluates random, greedy, and globally optimal teaching across budgets from 0 to 32 records, including single-question, proposition-battery, and graph objectives. Single-Graph optima are conditional on the specified fixed update schedules.

These analyses distinguish genuine conflict between objectives from shortfalls of the search procedure and the choice among equally good solutions. In particular, the poster's simplicity-bias reversal describes the tested greedy procedures; its interpretation is refined by the optimal-teaching analysis.

The paper also examines finite evidence supply, memory constraints, and the teacher's knowledge of stochastic learner updates. It distinguishes improved learner judgements, information conveyed by a teacher's choices, and what passive observations identify. A teacher who knows the target can convey information through the choice of genuine records, so passive observational equivalence alone does not determine the information available in a teaching history.

## Poster references

[References_APA7.txt](References_APA7.txt) contains the full APA 7 references for citations **[1]–[13]** printed on the poster. It includes a numbered citation key followed by an alphabetical reference list.

For enquiries, contact Fletcher Scott at [fletcher.scott@student.rmit.edu.au](mailto:fletcher.scott@student.rmit.edu.au), or visit [fletcher-scott.com](https://fletcher-scott.com).
