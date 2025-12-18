# Datasheet for BBO Capstone Project Dataset

## Motivation
This dataset was created to support a black-box optimisation (BBO) capstone project focused on iterative query selection under incomplete information. The goal is to optimise unknown objective functions by learning from past query–response pairs and refining strategies across multiple rounds. The dataset supports experimentation with exploration–exploitation trade-offs, surrogate modelling, and decision-making under uncertainty. It was created as part of a postgraduate Machine Learning & Artificial Intelligence programme capstone project.

## Composition
The dataset consists of sequential query inputs and corresponding function evaluations collected across ten optimisation rounds. Each round contains one query per function, covering eight unknown functions with dimensionalities ranging from 2D to 8D. Each data point is represented as a vector of continuous values in the range [0, 1], specified to six decimal places, along with the returned scalar performance value. The dataset is relatively small by design, reflecting realistic constraints in black-box optimisation scenarios. No personally identifiable or sensitive information is included.

## Collection Process
Data was collected iteratively through a capstone project portal that evaluates submitted queries against hidden objective functions. Query points were generated using adaptive strategies informed by results from previous rounds, including random exploration in early stages and increasingly structured exploitation in later rounds. The collection process spanned ten weekly iterations, allowing progressive refinement of optimisation strategies. All data was generated synthetically by the evaluation system; no human subjects were involved.

## Preprocessing and Uses
Minimal preprocessing was applied beyond formatting inputs to a consistent numerical representation and recording outputs. Queries were normalised to the [0, 1] range by design. The dataset is intended for analysing optimisation strategies, surrogate model behaviour, and decision-making under uncertainty. It is not suitable for supervised learning benchmarks, real-world prediction tasks, or applications requiring large-scale or representative datasets.

## Distribution
The dataset is stored locally within the project repository and is not distributed as a standalone public dataset. Access is provided through the associated GitHub repository for academic review and reproducibility purposes only. There are no licensing restrictions beyond educational use.

## Maintenance
The dataset is maintained by the project author as part of the capstone repository. Updates occur only when new optimisation rounds are completed. Version control is handled through GitHub commits, ensuring traceability of changes. No long-term updates beyond the scope of the capstone project are planned.
