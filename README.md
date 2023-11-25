# High-Sensitivity-PubMed-Query-Aid
Crafts highly sensitive PubMed queries from Clinical Questions <br>
[High-Sensitivity-PubMed-Query-Aid](https://chat.openai.com/g/g-3Ylvxx5GH-peco-summarizer)

# Background
One concern for clinicians when searching for research papers is whether they are overlooking anything. In other words, the sensitivity of the search formula they created might be low, leading to important papers being missed. Although becoming familiar with the PubMed search formula can reduce these oversights, typically these formulas are very long and require what is known as a craftsman's skill. I created this GPTs to make this process easy for anyone.

# Update History
Nov 25, 2023: ver.1 is now available.

# Input examples and their outputs
**Example 1** <br>
Input  <br>
 Can PDE inhibitors help COPD with pulmonary hypertension? <br>
Output <br>
("phosphodiesterase inhibitors"[Title/Abstract] OR "PDE inhibitors"[Title/Abstract] OR "sildenafil"[Title/Abstract] OR "tadalafil"[Title/Abstract] OR "vardenafil"[Title/Abstract] OR "avanafil"[Title/Abstract]) AND ("pulmonary disease, chronic obstructive"[MeSH Terms] OR ("pulmonary"[All Fields] AND "disease"[All Fields] AND "chronic"[All Fields] AND "obstructive"[All Fields]) OR "chronic obstructive pulmonary disease"[All Fields] OR "COPD"[All Fields]) AND ("hypertension, pulmonary"[MeSH Terms] OR ("pulmonary"[All Fields] AND "hypertension"[All Fields]) OR "pulmonary hypertension"[All Fields])

**Example 2** <br>
Input <br>
Are oral steroids for asthma associated with mortality? <br>
