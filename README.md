CLGPT_Kcr
CLGPT_Kcr: A novel approach based on GPT2 architecture to Predict Protein Lysine Crotonylation.
 Requirement
-	Goolge Colab pro
-	Keras
-	Numpy
-	Pandas
-	Tensorflow
-	Transformers
-	NLPK
Dataset
To construct and evaluate the proposed CLGPT_Kcr model, we surveyed and analyzed datasets from several recent studies that focus on lysine crotonylation (Kcr) site prediction. Most existing approaches, including Deep-Kcr [17], BERT-Kcr [19], Adapt-Kcr [20], and models employing multi-head self-attention mechanisms, have utilized benchmark datasets originally curated and published by the Deep_Kcr study. These datasets are publicly available and have been widely adopted for model training and evaluation in the field.
Specifically, the training dataset comprises 3,734 non-redundant proteins, with an equal number of 6,975 positive samples (i.e., lysine residues experimentally confirmed as crotonylated) and 6,975 negative samples (lysine residues not identified as crotonylated), ensuring a balanced classification setting. For independent performance assessment, a testing set containing 2,989 positive samples and 2,989 negative samples was also constructed, derived from proteins distinct from those in the training set. This dataset partitioning strategy follows the experimental setup of prior works such as Deep_Kcr and BERT-Kcr to facilitate fair comparison.
All protein sequences were preprocessed by extracting fixed-length peptide fragments centered on lysine residues. Each fragment has a window size of 31 amino acids (15 residues upstream and 15 residues downstream of the target lysine), ensuring that contextual sequence information is retained while maintaining input consistency for the transformer-based architecture. Sequences shorter than 31 residues were zero-padded using the special character 'X' to maintain uniform input length.
Redundant sequences were removed using a 40% similarity threshold to prevent model overfitting due to high sequence identity. The final benchmark dataset used in our experiments is identical to the one employed in Deep_Kcr and BERT-Kcr, allowing for a direct and fair comparison of model performance. The dataset was retrieved from publicly available repositories (e.g., GitHub), ensuring reproducibility and transparency.
This comprehensive and well-curated dataset provides a robust foundation for training and evaluating the CLGPT_Kcr model, ensuring that performance improvements stem from architectural advancements rather than data artifacts.
Train model: We use Google colab pro buid this model
⮚	Cross validation: GPT2_Kcr_cross_validation.ipynb
Model saved and named: CLGPT_Kcr.pth. You can use CLGPT_Kcr.pth in the Model folder for predict and independent test.
⮚	Independent test and predict in the GPT2_Kcr_ID.ipynb.
Contact
Please feel free to contact us if you need any help: nvnui@ictu.edu.vn

