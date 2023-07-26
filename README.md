# resnick-similarity
```resnick-similarity``` implements a program to perform word sense disambiguation based on noun groups using Resnick's method and WordBet-based similarity measure, and then compares the output to a set of human judgement. 

Load information content values for WordNet from a file. 
* Read in a file of (probe word, noun group) pairs 
* For each (probe word, noun group) pair: 
    a. Use "Resnik similarity" based on WordNet and information content to compute the preferred WordNet sense for the probe word given the noun group context. 
    b. On a single line, for each (probe word, noun group word) pair: 
        * print the similarity between the probe word and each noun group word in the format 0 (probe word, noun group word, Resnik similarity score) 
        * On a separate line, print out the preferred sense, by synsetlD, of the word. 
        * Read in a file of human judgments of similarity between pairs of words. • For each word pair in the file: 
            * Compute the similarity between the two words, using the Resnik similarity measure 
            * Print out the similarity as: 0 wdl,wd2:similarity 
* Lastly, compute and print the Spearman correlation between the similarity scores you have computed and the human-generated similarity scores in the provided file as: 
* Correlation:computed correlation. 

HW8 OF LING571 (12/06/2021)