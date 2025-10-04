Heredity Model using Bayesian Probability

📌 Project Overview

This project implements a Bayesian Network–style model to analyze the probability of individuals inheriting genetic traits.
It calculates the likelihood of each person having 0, 1, or 2 copies of a gene, and whether they exhibit a trait, based on:
	•	Unconditional probabilities (if parents are unknown).
	•	Conditional probabilities (inheritance from parents).
	•	Trait probabilities (given gene count).

The model iterates through all possible gene/trait distributions, computes joint probabilities, and produces normalized distributions for each person.


🧪 Example

For a simple family:
	•	Alice (no parents)
	•	Bob (no parents)
	•	Charlie (child of Alice and Bob)

The program outputs probabilities like:
{'Alice': {'gene': {2: 0.01, 1: 0.03, 0: 0.96},
           'trait': {True: 0.02, False: 0.98}},
 'Bob':   {'gene': {...}, 'trait': {...}},
 'Charlie': {'gene': {...}, 'trait': {...}}}

⚙️ How It Works
	1.	Define Base Probabilities
	•	Prior probabilities for genes (0/1/2).
	•	Conditional probabilities for traits given genes.
	2.	Joint Probability Calculation
	•	Considers parent → child inheritance rules.
	•	Uses mutation probabilities (1% chance gene is passed incorrectly).
	3.	Update & Normalize
	•	Aggregates results across all possible configurations.
	•	Normalizes so each distribution sums to 1.


🚀 How to Run
	1.	Clone or download this repository.
	2.	Open the notebook or Python file in your environment.
	3.	Run the script — results will be printed in the console.


📂 Files
	•	heredity.py or heredity.ipynb → Main code.
	•	README.md → Project documentation.


📖 Concepts Used
	•	Bayesian Probability
	•	Joint Probability Distribution
	•	Inheritance Rules & Mutation
	•	Normalization of Probabilities


✅ Future Improvements
	•	Extend to larger family datasets (CSV input).
	•	Visualize Bayesian Network graphically.
	•	Compare results with real-world genetic probabilities.


✨ This project demonstrates how Bayesian inference can be applied to model genetic inheritance and traits without needing external datasets.