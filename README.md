# filler-gaps
unable to upload any .pt models from zenodo due to size limits 

/scripts/: use the output from -load_data- as input to -analyses-. 

-extraction_templates-: contains full table of all stimuli used in experiments. acceptability 1 = grammatically unacceptable. acceptability 5 = grammatically acceptable. 

-extraction_toks-: contains all stimuli sentences. later separated into dev and test sets in /dev_toks/ and /test_toks/. 

/outputs/: the most relevant files are the ones named in the following way: (shuffled)_adapted_type1_type2_letter.csv_
--> shuffled prefix refers to baseline experiments where stimuli tokens where shuffled.
--> type1 refers to the structure that the model was adapted/trained on
--> type 2 refers to the structure that the model was tested on
--> letter (a/b/c/d/e) corresponds to one of the five zenodo models used in training.
