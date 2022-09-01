# Cricket-Team-Selection-Using-LSTM-Model
# Dataset
Datasets of english doemstic cricket, australian domestic cricket and international cricket was scraped from ESPNcricinfo using scrapy. 

Datasets included batting, bowling, matches and players records from 2010 till present. 

After collection, datasets were cleaned and pre-processed for further analysis.

Pre-processed datasets are in attached raw folder and cleaned datasets and trained models were saved in attached results folder. 
# Key Parameters
key parameters based on which player performance were rated:

For batsmens: runs, man of the match, Century, Chase, half-century, winning factor, not out, strike rate.

For bowlers: wickets, man of the match, ten wicket haul, five wicket haul, winning factor, economy rate. 

Details of weigthatges of these parameters in rating are given in jupytor notebooks. Players were given rating based on these factors. 
# Training the LSTM model
LSTM model with four hidden layers were trained on cleaned datasets. 

Then trained model was used to predict top rated squad of 19 for England and Australia. 

Model only considered player performance from previous 14 tests for England and 9 tests for Australia. 

And international players were given 90% preferrence over domestic performance. 

# Structure of Squads
For England: Model predicted top 10 batsmens (including wicket keepers), 2 all-rounders, 3 spinners and 4 fast bowlers in the squad of 19. 

For Australia: Model predicted top 8 batsmens (including wicket keepers), 4 all-rounders, 3 spinners and 4 fast bowlers in the squad of 19. 
# Note
This model not only for tests, this model can be used to predict any team and any format. 
