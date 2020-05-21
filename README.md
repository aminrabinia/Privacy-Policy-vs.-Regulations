# Privacy-Policy-vs.-Regulations
This project deals with comparisons between legal texts and privacy policy texts. It uses an NLI model to find the entailments (or contradictions) relation between legal requirements and privacy policies. The model uses fixed glove.6B.300d for the embeddings and trainable bidirectional LSTM layers. 

The model is trained on Multi-NLI dataset and then applied on privacy policies of phone apps and few rule from Europian privacy regulations (GDPR). For example, the legal statement: "The data subject shall have the right to withdraw his or her consent at any time" compared with a random policy statement: "Data processed on the basis of consent will generally be stored until the given consent is withdrawn" has the following results: 

Contradiction: 0.11 neutral 0.17 entailment 0.72
