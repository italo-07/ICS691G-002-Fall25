# Transformer-Based Unit Test Generation

**Source:** 2025 IEEE Conference on Artificial Intelligence (CAI)  
**Link:** <https://doi.org/10.1109/CAI64502.2025.00115>

## Summary
**Problem :** The manual authoring of unit test is a very time consuming task and the biggest bottleneck during software development process. AI and NLP can automate and optimize test creation, saving developer time and minimizing errors.

**Approach ):** The authors present transformer models for automatic unit test generation, leveraging textual-based natural language processing of Python functions concatenated with their docstrings to retain code structure and developer intent. The models receive this merged input, and produce full assertions unit tests to check the correctness of the function. Specifically, each model was fine-tuned on a curated dataset and tested for its capability to produce executable test cases that are semantically relevant.

**Models compared :**
- CodeT5 (Salesforce/codet5-base)
- MCodeBERT (huggingface/CodeBERTa-small-v1)
- CodeGen (Salesforce/codegen-350M-mono)


**Evaluation :** The authors considered both linguistic metrics such as BLEU, ROUGE-L, Levenshtein distance, and the vector representation cosine similarity and that of software testing such as code coverage using the tool coverage. py) on a 3,123 functions’ data set where we have the natural language description and unit tests. They further performed statistical significance testing with independent t-tests in order to confirm the performance differences.

**Key results :** All results again showed that CodeT5 outperforms CodeBERT and CodeGen by large margins with 75% code coverage higher than the best performance of CodeBERT (48%) and current state-of-the-art coverage of CodeGen (10%). CodeT5 also scored the best in F1-score (0.8337), BLEU score (0.6646) and for semantic similarity scores. Statistical tests validated that CodeT5's benefits are statistically significant (p < 0.05) in all the metrics.

**Limitations :** It was conducted over a relatively small dataset of 3,123 samples for Python functions as inputs and its results were limited to generalization only on larger codebases or other programming languages. The analysis was based on static metrics (such as BLEU or code coverage) and not dynamic behavior / defect finding.



