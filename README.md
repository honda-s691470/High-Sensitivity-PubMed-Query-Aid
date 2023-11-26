# High-Sensitivity-PubMed-Query-Aid
Crafts high-sensitivity PubMed queries from Clinical Questions <br>
[High-Sensitivity-PubMed-Query-Aid](https://chat.openai.com/g/g-1ruVUSGPy-high-sensitivity-pubmed-query-aid)

# Background
One concern for clinicians when searching for research papers is whether they are overlooking anything. In other words, the sensitivity of the search formula they created might be low, leading to important papers being missed. Although becoming familiar with the PubMed search formula can reduce these oversights, typically these formulas are very long and require what is known as a craftsman's skill. I created this GPTs to make this process easy for anyone.

# Update History
Nov 25, 2023: ver.1 is now available.

# Input examples and their outputs
**Example 1** <br>
- Input  <br>
 Can PDE inhibitors help COPD with pulmonary hypertension? <br>
- Output <br>
("phosphodiesterase inhibitors"[Title/Abstract] OR "PDE inhibitors"[Title/Abstract] OR "sildenafil"[Title/Abstract] OR "tadalafil"[Title/Abstract] OR "vardenafil"[Title/Abstract] OR "avanafil"[Title/Abstract]) AND ("pulmonary disease, chronic obstructive"[MeSH Terms] OR ("pulmonary"[All Fields] AND "disease"[All Fields] AND "chronic"[All Fields] AND "obstructive"[All Fields]) OR "chronic obstructive pulmonary disease"[All Fields] OR "COPD"[All Fields]) AND ("hypertension, pulmonary"[MeSH Terms] OR ("pulmonary"[All Fields] AND "hypertension"[All Fields]) OR "pulmonary hypertension"[All Fields])

**Example 2** <br>
- Input/High-Sensitivity-PubMed-Query-Aid <br>
Is BEL effective in SLE complicated by pulmonary hypertension and interstitial pneumonia? <br>
- Output/High-Sensitivity-PubMed-Query-Aid <br>
("belimumab"[Title/Abstract] OR "Benlysta"[Title/Abstract]) AND 
("lupus erythematosus, systemic"[MeSH Terms] OR ("lupus"[All Fields] AND "erythematosus"[All Fields] AND "systemic"[All Fields]) OR "systemic lupus erythematosus"[All Fields] OR "SLE"[All Fields]) AND 
("hypertension, pulmonary"[MeSH Terms] OR ("hypertension"[All Fields] AND "pulmonary"[All Fields]) OR "pulmonary hypertension"[All Fields]) AND 
("pneumonia, interstitial"[MeSH Terms] OR ("pneumonia"[All Fields] AND "interstitial"[All Fields]) OR "interstitial pneumonia"[All Fields])



**Example 3** <br>
- Input <br>
Correlation between serum procalcitonin levels and severity of illness in community acquired pneumonia. <br>
- Output <br>
("procalcitonin"[Title/Abstract] OR "PCT"[Title/Abstract] OR "serum procalcitonin"[Title/Abstract]) AND ("severity of illness index"[MeSH Terms] OR ("severity"[All Fields] AND "illness"[All Fields]) OR "severity of illness"[All Fields]) AND ("pneumonia, bacterial"[MeSH Terms] OR ("pneumonia"[All Fields] AND "bacterial"[All Fields]) OR "community-acquired pneumonia"[All Fields] OR "CAP"[All Fields])
- number of results<br>
174 results (Nov 26 2023) <br>

- Input/GPT4 <br>
Please provide a highly sensitive Pubmed query that will help us find articles on the following CQs: Correlation between serum procalcitonin levels and severity of illness in community acquired pneumonia.
- Output/GPT4 <br>
"Procalcitonin"[MeSH] AND "Community-Acquired Infections"[MeSH] AND "Pneumonia"[MeSH] AND ("severity of illness index"[MeSH] OR "disease severity"[Title/Abstract])
- number of results<br>
14 results (Nov 26 2023) <br>

| **Example 3** | Input                                                                                                                         | Output                                                                                                                                                                                                                                                                                   |
|-------------|-------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Input/MyModel | Correlation between serum procalcitonin levels and severity of illness in community acquired pneumonia.                         | ("procalcitonin"[Title/Abstract] OR "PCT"[Title/Abstract] OR "serum procalcitonin"[Title/Abstract]) AND ("severity of illness index"[MeSH Terms] OR ("severity"[All Fields] AND "illness"[All Fields]) OR "severity of illness"[All Fields]) AND ("pneumonia, bacterial"[MeSH Terms] OR ("pneumonia"[All Fields] AND "bacterial"[All Fields]) OR "community-acquired pneumonia"[All Fields] OR "CAP"[All Fields]) |
| Input/GPT4   | Please provide a highly sensitive Pubmed query that will help us find articles on the following CQs: Correlation between serum procalcitonin levels and severity of illness in community acquired pneumonia. | "Procalcitonin"[MeSH] AND "Community-Acquired Infections"[MeSH] AND "Pneumonia"[MeSH] AND ("severity of illness index"[MeSH] OR "disease severity"[Title/Abstract])                                                                                                                                                                                   |

