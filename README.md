### Project Title: Query-Guided Multi-Perspective Answer Summarization
### Team-6: Phrase Phantoms
- Akshit Sharma
- Rudransh Agarwal
- Sai Asrith Devisetti

### Files Submitted:

- Report.pdf: Report containing explanation for all the approaches that we experimented with along with comparison of metrics.

- BartPT_AllAns.ipynb: Code and cell outputs for running inference on test set with pre-trained BART for end-to-end summarization, with only all the concatenated answers as input to model.
- BartPT_Query+AllAns.ipynb: Code and cell outputs for running inference on test set with pre-trained BART for end-to-end summarization, with query followed by all the concatenated answers as input to model.

- BartFT_AllAns.ipynb: Code and cell outputs for fine-tuning BART on AnswerSumm dataset and running inference on test set. The input to the model, for a sample, is all the answers for it concatenated together. 
- BartFT_Query+AllAns.ipynb: Code and cell outputs for fine-tuning BART on AnswerSumm dataset and running inference on test set. The input to the model, for a sample, is query followed by all the answers for it concatenated together.
- RelReg.ipynb: Code and cell outputs to train the RelReg model, run inference on test-set samples, generate summaries (using fine tuned BART) and calculate the ROUGE metrics for it.
- RelRegTT.ipynb: Code and cell outputs to run the RelRegTT model on test-set, generate the summaries (using fine tuned BART) and caluclate the ROUGE metrics.
- RelClass.ipynb: Code and cell outputs to train the RelClass model and run inference on test-set of Answersumm and calculate ROUGE metrics using the generated summaries (using fine tuned BART).
- Clustering.ipynb: Code and cell outputs for running the DBSCAN algorithm for clustering on the test-set of AnswerSumm dataset, generating summaries (using fine tuned BART) and calculating ROUGE metrics.

### BART Fine-Tuning Details:
- No. of epochs: 5
- Learning Rate= 5e-5
- Optimizer= AdamW
- No. of training samples: 2700
- Max. Output Length= 256 tokens
- Max. Input Length= 1024 tokens
- Max. target length= 256 tokens

### RelReg and RelClass Training Details:
- No. of epochs= 5
- Learning Rate= 2e-5
- Optimizer= AdamW
- Criterion (RelReg)= MSE Loss, Criterion (RelClass)= Binary Cross Entropy Loss
- No. of training samples= 10,000
- Max. Output Length (BART)= 256 tokens
- Max. Input Length= 1024 tokens

#### [OneDrive link for trained model files](https://iiitaphyd-my.sharepoint.com/:f:/g/personal/akshit_sharma_students_iiit_ac_in/EtA4rsz1I7NAmXppVgKOAAEBAcqzQ0b6NfZkvOU7RILTUg?e=esqgVM)

#### [Link to final presentation](https://www.canva.com/design/DAGW8D4K9Oc/MoRzI8N5G9jwZcDhBNwueA/edit?utm_content=DAGW8D4K9Oc&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)
