# Genetic algorithms advanced topic presentation outline

## Presentation 1

* Topic 1 (Intro) - Genetics in General (10 min)
	* Basic summary of genetics
		* Three core principles
			* Heredity
			* Variation
			* Selection
		* Genes and alleles, genotype vs phenotype
		* Punnett Squares

* Topic 2 - Genetic Algorithms (15 min)
	* A way to “evolve” to a specific solution
		* Steps:
			* Create a population of N random elements
			* Calculate fitness for N elements
				* Based on how close each element is to the target solution.
				* Ex: We’re trying to evolve to the word “Foobar”
					* An element “Fooxyz” would have a fitness score of 0.5 because it is 50% of the desired answer.
			* Reproduce/Selection
				* Pick 2 parents based on the fitness
					* Ex: “Tqwbar”, “xxxxxx”
					
* Topic 3 - Genetics in Video Games (10 min)
	* Animal Crossing: New Horizons genetic system for coloring flowers
		* The games static traits vs. our continuous distribution
	* Football Manager 2021
		* Mentoring System
			* Make the point that these algorithms don't just have to be applied to genetics
	* Pokemon Hidden Stats
		* Different IV's seperate Pokemon that would otherwise be identical

* Topic 4 - Our Implementation (10 min)
	* Use continuous distributions rather than "binary" allele combinations
	* Generating new seeds with random starter genes
		* Use Gaussian distribution to allow randomness and variation while also keeping generated values close to an average
			* (Gaussian distribution has 68% of all values within a single standard deviation of the mean)

...
