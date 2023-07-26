# resnick-similarity
```resnick-similarity``` implements a program to perform word sense disambiguation based on noun groups using Resnick's method and WordNet-based similarity measure, and then compares the output to a set of human judgement. 

Args: 
* ```<information_content_file>```: path to information content file (cf. mc_similarity.txt)
* ```<wsd_test_filename>```: path to file which contains "probe-word, noun group words" pairs (cf. wsd_contexts.txt)
* ```<judgment_file>```: path to file with human judgments (cf. wsd_contexts.txt.gold)

Returns: 
* ```<output_filename>```: path to output file with results

To run: 
```
src/hw8_resnick_wsd.sh input/mc_similarity.txt input/wsd_contexts.txt input/wsd_contexts.txt.gold output/<output_filename>
```

HW8 OF LING571 (12/06/2021)