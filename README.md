# Misogyny Detection

This project sought out with a goal of detecting misogyny in song lyrics, with a goal of assessing whether the level or type of misogyny has changed meaningfully over time. After exploration, a staged BERT model was chosen, and trained on labeled data from Twitter and Reddit posts (as these were the highest quality datasets that could be found with subclassifications of misogyny). This model was then run on chunked song lyrics for final measures.

## Table of Contents

This project repo contains the following:

* final_labels.csv - The Reddit dataset, made publically available by Ella Guest and team.
* billboardHot100_1999-2019.csv - Dataset of song lyrics from Kaggle.
* Clean Data.ipynb - Notebook used to clean the datasets, and harmonize the subclassifications from the two training sets.
* reddit_labels.pkl - Cleaned and reclassified Reddit file for model training.
* song_data_2000s.pkl - Cleaned and selected song data for model evaluation.
* Model Training and Running.ipynb - Training the models, running on the song data.
* Project Write-up.pdf - A more in detail write-up of the project, why particular assumptions/decisions were made, error analysis, conclusions, etc.

The repo is notably missing the following:
* en_training.tsv and en_testing.tsv - Dataset of labeled Tweets, as this dataset is not publically available. This dataset was used in the Autonomous Misogyny Identification task at the IBEREVAL 2018 evaluation campaign, and used with permission by that team. For those who wish to gain access to the data themselves, more information can be found [here](https://amiibereval2018.wordpress.com/).
* twitter_labels.pkl - Project reclassified version of the data.

## Further Information

Please see the project write-up for details on why particular assumptions/decisions were made, how the model performed on the training data, an error analysis, project conclusions, etc.

Any further questions can be directed to luke.verdi@gmail.com.
