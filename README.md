# Capstone Project
## 📌 Project Summary
This capstone project explores a black-box optimisation (BBO) challenge, where the internal structure of the objective functions is unknown. The goal is to iteratively propose query points that improve performance based only on observed outputs, similar to real-world optimisation problems where models or systems cannot be directly inspected.

Across multiple rounds, I developed and refined a strategy for exploring and exploiting the search space, using patterns in historical query results to guide future decisions. The project emphasises transparency, reproducibility, and responsible AI practices through clear documentation of data usage, assumptions, and limitations.

## 🎯 Goals / Problem Statement
The goal of this project is to optimise a set of unknown black-box functions by iteratively selecting input values that improve performance over time. Because the internal structure of each function is hidden, decisions must be made solely based on past input–output observations.

This mirrors real-world optimisation problems where direct access to system internals is not possible, such as hyperparameter tuning, engineering design optimisation, or experimental process optimisation. The challenge lies in balancing exploration of new regions of the search space with exploitation of regions that have previously shown promising results.

## 🛠️ Tools & Technologies
This project was developed using Python for data analysis and experimentation. The optimisation process was carried out through a web-based capstone project portal, where query points were submitted and corresponding outputs were observed.

GitHub was used for version control and documentation, ensuring transparency an

## 📘 Non-Technical Project Overview
This project explores how complex systems can be improved even when their internal workings are unknown. Instead of analysing the system directly, performance is improved by testing different inputs and learning from the results over time. Through multiple rounds of experimentation, patterns in successful inputs emerged, allowing future decisions to be more focused and efficient. This mirrors real-world situations such as tuning business processes or machine learning systems where direct access to internal logic is limited. Overall, the project demonstrates how careful experimentation, reflection, and documentation can lead to meaningful improvements without full system visibility.


## Transparency & Documentation

This repository includes formal documentation to support transparency, reproducibility, and responsible AI practices for the BBO capstone project.

- 📄 **Dataset Datasheet**: [docs/datasheet.md](docs/datasheet.md)  
  Documents the motivation, composition, collection process, intended uses, and maintenance of the optimisation query dataset.

- 🧾 **Model Card**: [docs/model_card.md](docs/model_card.md)  
  Describes the black-box optimisation strategy, intended use, performance characteristics, assumptions, limitations, and ethical considerations.
