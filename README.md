**CLGPT_Kcr: A novel approach based on GPT2 architecture to Predict Protein Lysine Crotonylation.**
  ** Requirement**
  -	Goolge Colab pro
  -	Keras
  -	Numpy
  -	Pandas
  -	Tensorflow
  -	Transformers
  -	NLPK

**Dataset**

 **Training dataset** comprises 3,734 non-redundant proteins, with an equal number of 6,975 positive samples (i.e., lysine residues experimentally confirmed as crotonylated) and 6,975 negative samples (lysine residues not identified as crotonylated), ensuring a balanced classification setting.
**Testing set** containing 2,989 positive samples and 2,989 negative samples was also constructed, derived from proteins distinct from those in the training set. This dataset partitioning strategy follows the experimental setup of prior works such as Deep_Kcr and BERT-Kcr to facilitate fair comparison.
  All protein sequences were preprocessed by extracting fixed-length peptide fragments centered on lysine residues. Each fragment has a window size of 31 amino acids (15 residues upstream and 15 residues downstream of the target lysine), ensuring that contextual sequence information is retained while maintaining input consistency for the transformer-based architecture. Sequences shorter than 31 residues were zero-padded using the special character 'X' to maintain uniform input length.
  Redundant sequences were removed using a 40% similarity threshold to prevent model overfitting due to high sequence identity. 

**Train model: We use Google colab pro buid this model**

  ⮚	Cross validation: GPT2_Kcr_cross_validation.ipynb
  Model saved and named: CLGPT_Kcr.pth. You can use CLGPT_Kcr.pth in the Model folder for predict and independent test.
  ⮚	Independent test and predict in the GPT2_Kcr_ID.ipynb.

**Contact**
  Please feel free to contact us if you need any help: nvnui@ictu.edu.vn

