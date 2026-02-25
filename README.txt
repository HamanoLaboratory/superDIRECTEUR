<Proposed method>
SuperDIRECTEUR

<Introduction> 
SuperDIRECTEUR predicts combinations of small molecules by accounting for dynamic molecular mechanistic changes during direct programming induction. To account for these dynamic changes, the cell conversion process is divided into several stages (e.g., Primal stage, Immature stage, and Mature stage). Combinations of small molecules that induce cell conversion between adjacent stages are then predicted.

# You can run the proposed method with the following procedures:

Run : src/main.py

Output : results/{result}

python main.py -i {} -t {} -n {} -e {} -optD {} -tarD {} -out {} 

# You can change any parameters filling after each arguments.

-i : default = 10 # Maximum number of iterations
-t : default = 60 # Maximum execution time (sec)
-n : default = 5  # Number of elements to include in the combination.
-e : default = 3  # Number of sub objective functions
-optD : # Transcriptome data to optimize
-tarD : # Transcriptome data during Direct Reprogramming
-out : # Output file name


# Data
Transcriptome data can be changed to your own data.
Transcriptome data: Data on expression ratios in each gene before and after Direct Reprogramming

#sub objective functions

sub objective functions can be changed for your analysis.
