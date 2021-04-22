# Replication Package for "An Empirical Study of the Effectiveness of an Ensemble of Stand-alone Sentiment Detection Tools for Software Engineering Datasets"

- The file "SentiseadCode.zip" contains the source code of Sentisead using Random Forest.
- https://www.kaggle.com/giasuddin/hybridsentiment contains the code we used to experiment with advanced language-based pre-trained transformer models (PTM)
- The file "Results in Invididual Datasets.docx" shows performance of individual and hybrid tools on the entire datasets as well as the six datasets.
- The file "ResultsConsolidatedWithEnsambleAssessment_BERTLabeledFinal.xlsx" contains all the data we used to answer RQ1-RQ8. The following columns are necessary in the above file to understand the data:

  1. "File" colmun shows the six studied datasets. This column also shows the folds per file that we used. For example, "DatasetLinJIRA_Cleaned_test_0" denotes the fold 0 in the Lin et al. JIRA dataset, "DatasetLinJIRA_Cleaned_test_1" denotes fold 1, etc. 
  2. "Sentence" column shows the raw sentence 
  3. "ManualLabel" column shows the grouth turth sentiment polarity label of the sentence
  4. "DsoLabelFullText" shows the polarity label of Opiner on the sentence
  5. "POME" shows the polarity label of POME on the sentence
  6. "Senti4SD" shows the polarity label of Senti4SD on the sentence after 10-fold cross validation per dataset
  7. "SentiCR" shows the polarity label of SentiCR on the sentence after 10-fold cross validation per dataset
  8. "SentistrengthSE" shows the polarity label of SentistrengthSE on the sentence
  9. "Shannon" shows the entropy score of the sentence based on all texts
  10. "ShannonAdjective" shows the entropy score of the sentence based on all adjectives
  11. "Ensemble_RF" shows the polarity label of a sentence from Sentiead_B (RQ4) after 10-fold cross validation per dataset
  12. 'BERT', 'ROBERTA', 'XLNET', 'ALBERT' show the polarity label of a sentence from stand-alone PTMs (RQ6) after 10-fold cross validation per dataset
  13. 'SentiseadBert', 'SentiseadRoberta', 'SentiseadXlnet', 'SentiseadAlbert' show the polarity label of a sentence from Sentiead_{PTM} (RQ7) after 10-fold cross validation per dataset
  14. 'SentiseadBertPlus', 'SentiseadRobertaPlus', 'SentiseadXlnetPlus', 'SentiseadAlbertPlus' show the polarity label of a sentence from Sentiead_{PTM}+ (RQ8) after 10-fold cross validation per dataset
