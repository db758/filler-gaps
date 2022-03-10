# filler-gaps
unable to upload any .pt models from zenodo due to size limits 

/scripts/: use the output from -load_data- as input to -analyses-. 

-extraction_templates-: contains full table of all stimuli used in experiments. acceptability 1 = grammatically unacceptable. acceptability 5 = grammatically acceptable. 

-extraction_toks-: contains all stimuli sentences. later separated into dev and test sets in /dev_toks/ and /test_toks/. dev tok sets were used to train/adapt zenodo models. 

/outputs/: the most relevant files are the ones named in the following way: (shuffled)_adapted_type1_type2_letter.csv_ e.g. shuffled_adapted_adjunct_wh_a.csv.  
--> shuffled prefix refers to baseline experiments where stimuli tokens where shuffled before model training.  
--> type1 refers to the structure that the model was adapted/trained on e.g. adjunct in the above example.  
--> type 2 refers to the structure that the model was tested on e.g. wh in the above example.  
--> letter (a/b/c/d/e) corresponds to one of the five zenodo models used in training.  

can ignore files in /test_results/ within /outputs/ to start. these are non-adapted surprisals. will be used in -load_data-.

can ignore files in /outputs/ named in the following way: (shuffled)_adapted_type_letter.csv e.g. adapted_adjunct_a.csv

-all_commands-: contains all the terminal commands used in experiments (preprocessing stimuli, training models, testing models)
